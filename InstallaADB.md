<h1>Come installare comandi ADB su Windows</h1>

I seguenti passaggi chiariranno come installare ADB su Windows.

La procedura mostrata è stata eseguita su Windows 11 ma si può applicare tranquillamente su Windows 10 e Windows 8. Le differenze sono minime in termini di interfaccia grafica.

Scaricare il file ZIP di [Android SDK Platform Tools](https://dl.google.com/android/repository/platform-tools-latest-windows.zip) per Windows.

Estrarre il contenuto di questo file ZIP in una cartella facilmente accessibile del proprio PC Windows.

Aprire la cartella in cui è stato estratto il contenuto di questo file ZIP.

Quindi aprire una finestra di comando dalla stessa directory.

Questo può essere fatto tenendo premuto Maiusc e facendo clic con il pulsante destro del mouse all'interno della cartella, quindi fare clic sull'opzione "Apri finestra di comando qui".

(Alcuni utenti di Windows 10 potrebbero visualizzare "PowerShell" invece di "finestra di comando").

Collegare lo smartphone o tablet al PC con un cavo USB.

Modificare la modalità USB in modalità "trasferimento file (MTP)".

Alcuni OEM potrebbero richiederlo o meno, ma è meglio lasciarlo in questa modalità per compatibilità generale.

Nella finestra del prompt dei comandi, immettere il seguente comando per avviare il demone ADB: adb devices
Alcuni PC potrebbero richiedere un comando di livello superiore, per ragioni di sicurezza.

In questo caso sarà sufficiente inviare il comando: ./adb devices

Sullo schermo dello smartphone, si dovrebbe vedere una richiesta per consentire o negare l'accesso al debug USB.

Concedere tale accesso al debug USB.

Come vedete dallo screenshot finale in basso si dovrebbe visualizzare la dicitura "authorized" a conferma che tutto è andato a buon fine nel collegamento.

<img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/ADB1.jpg" alt="" width="300"/> <img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/ADB2.jpg" alt="" width="100"/> <img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/ADB3.jpg" alt="" width="300"/>
