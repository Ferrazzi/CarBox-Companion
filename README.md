<h1><p align="center"><strong>Assistente vocale CarBox</strong></p></h1>


<strong>CarBox Companion</strong> è un assistente vocale per dispositivi box auto (tipo Carlinkit, Ottocast, ecc..) ed autoradio Android che consente di effettuare delle azioni che solitamente si fanno toccando lo schermo dell'infotainment ma con comandi vocali.

Il sistema è formato da due applicazioni principali, <strong>CarBox Companion</strong> e <strong>CarBox Voice</strong>.
Durante l'installazione verrà richiesto di installare applicazioni aggiuntive quali: [Autovoice](https://play.google.com/store/apps/details?id=com.joaomgcd.autovoice), [AutoContacts](https://play.google.com/store/apps/details?id=com.joaomgcd.autocontacts), [AutoShare](https://play.google.com/store/apps/details?id=com.joaomgcd.autoshare) e [Join](https://play.google.com/store/apps/details?id=com.joaomgcd.join) tutte prelevabili da GooglePlay in versione gratuita con limitazioni oppure a pagamento nella versione completa.

<img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/CarBoxCompanionIcon.png" alt="" width="50"/> <strong>CarBox Companion</strong>

<strong>CarBox Companion</strong> va installato sul telefono da utilizzare in abbinata al box auto o all'autoradio Android, serve da ricevitore per l'applicazione master <strong>CarBox Voice</strong> che andrà installata sul box auto o autoradio Android.

- Quando <strong>CarBox Companion</strong> è stato installato sul telefono basterà aprirlo e sarete guidati nell'installazione delle due applicazioni <strong>Join</strong> e <strong>AutoContacts</strong>.
- Installate le due applicazioni si può procedere con la guida per attivare i permessi ADB per la scrittura delle impostazioni sicure.

  - <strong>Abilita nelle impostazioni del telefono la modalità sviluppatore:</strong> Vai nelle impostazioni Android -> Informazioni sul telefono -> Informazioni software e cerca 

  - <strong>Versione build</strong>. Toccalo più volte fino all'attivazione della modalità sviluppatore.

  - <strong>Abilita Debug USB:</strong> Vai nelle impostazioni Android -> e cerca <strong>Opzioni sviluppatore</strong>. Dentro questo menu, abilita l'opzione di <strong>debug USB</strong>.

  - <strong>Installa ADB sul tuo PC:</strong> Controlla [qui](https://github.com/Ferrazzi/CarBox-Companion/blob/main/InstallaADB.md) per un modo rapido per farlo.

  - <strong>Connetti il dispositivo al PC:</strong> Connetti il tuo dispositivo al PC e guarda sul tuo telefono. Dovrebbe venire visualizzato un messaggio che ti chiede di consentire il debug del telefono da parte del PC. <strong>Accettalo</strong>.
  - Apri il prompt dei comandi dalla cartella dei file che contiene i file scaricati in precedenza nel link alla voce <strong>Installa ADB sul tuo PC</strong> ed estratti. Per fare ciò, premi il tasto Windows e digita cmd. Quando si apre il prompt, digita cd seguito dalla cartella in cui hai scaricato l'ADB.
  - <strong>Concedere l'autorizzazione:</strong> Apri una riga di comando sul tuo PC e scrivi i comandi necessari (uno alla volta)
    
    - <strong>Se usi Windows:</strong> adb shell pm grant net.dinglisch.android.taskerm android.permission.WRITE_SECURE_SETTINGS
    - <strong>Se usi Mac:</strong> ./adb shell pm grant net.dinglisch.android.taskerm android.permission.WRITE_SECURE_SETTINGS


<strong>Note:</strong>

Sui dispositivi MIUI potrebbe essere necessario aprire le opzioni sviluppatore e abilitare l'impostazione Debug USB (Impostazioni di sicurezza) (e l'impostazione Disattiva monitoraggio 
autorizzazioni in alcuni casi) per poter eseguire il comando precedente.

Se hai problemi di errore che il tuo dispositivo non è autorizzato, controlla [qui](https://www.addictivetips.com/android/fix-adb-device-unauthorized-message-android/).

- Fatto tutto questo si può premere sul pulsante <strong>AVANTI</strong> per passare alla schermata di <strong>configurazione dei permessi</strong>.
- Abilitare tutti i permessi toccando sui vari testi come da schermata e premere il pulsante <strong>AVANTI</strong>.
- Ora siamo arrivati finalmente alla schermata di configurazione di CarBox Companion.
- Toccando i pulsanti <strong>Seleziona Box 1</strong> e <strong>Seleziona Box 2</strong> verrà aperta una finestra che farà selezionare la connessione bluetooth del <strong>Primo CarBox</strong> oppure del <strong>Secondo CarBox</strong>, se ne avete un'altro in un altra auto. Abilitare lo switch sulla destra per attivare la funzione. Questo serve per permettere l'attivazione del tethering automaticamente alla rilevazione del box acceso cosi da dare connessione internet senza doverlo fare manualmente.
- Abilitare lo switch dell'abilitazione comandi vocali se si vogliono attivare le funzioni del box verso il telefono esempio le telefonate.
- Abilitare lo switch per le notifiche di parcheggio automatico, questo serve a ricevere una notifica quando il collegamento bluetooth viene interrotto al telefono e quindi il box è spento presupponendo di avere l'auto in parcheggio. Verrà visualizzata nel pannello notifiche appunto una notifica con le informazioni di parcheggio, una mappa con coordinate apribile con GoogleMaps ed eventualmente la possibilità di inserire una nota esempio numero parcheggio centro commerciale.
- Uscire da <strong>CarBox Companion</strong> e aprire <strong>Join</strong> dare consenso ad eventuali permessi e loggarsi con il proprio account di Google e chiudere Join.
- Aprire <strong>AutoContacts</strong> dare consenso ad eventuali permessi e tocare la voce <strong>Contacts</strong>. Entrati nella schermata Contacts toccare la voce <strong>Force Refresh Contacts</strong>, questo importerà tutti i tuoi contatti da poter usare per le telefonate ed eventuali messaggi. <strong>IMPORTANTE, ripetere questa operazione tutte le volte che viene aggiunto un nuovo contatto in rubrica senò non sarà accessibile per l'utilizzo</strong>.
- A questo punto abbiamo finito di configurare la parte <strong>CarBox Companion</strong> e possiamo continuare a configurare <strong>CarBox Voice</strong>.

<img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/CarBoxVoiceIcon.png" alt="" width="50"/> <strong>CarBox Voice</strong>

CarBox Voice va installato sul box o autoradio Android.

  -  Quando <strong>CarBox Voice</strong> è stato installato sul box basterà aprirlo e sarete guidati nell'installazione delle tre applicazioni <strong>AutoVoice</strong>, <strong>Join</strong> e <strong>AutoShare</strong>.
  -  Appena installate tutte e tre le applicazioni toccare i tasti a schermo per aprirne una alla volta e configurarla.
  -  Aprire AutoVoice e dare tutti i permessi richiesti. Toccare la voce <strong>AutoVoice Devices</strong> e loggarsi con il proprio account Google, a questo punto dovresti vedere il tuo dispositivo. Torna indietro alla schermata precedente di AutoVoice e tocca su <strong>Toasts And Logs</strong>, in questa schermata disabilita tutte le spunte di tutte le voci. Chiudi AutoVoice e passa al prossimo passo.
  -  Aprire AutoShare e dare tutti i permessi richiesti.
  -  Aprire Join, dare tutti i permessi richiesti e loggarsi con il proprio account Google. Nel menu <strong>Dispositivi</strong> troverai tutti i dispositivi in cui hai installato e loggato Join, ricordati il nome del tuo telefono con maiuscole e minuscole corrette e riapri CarBox Voice.
- Fatto tutto questo si può premere sul pulsante <strong>AVANTI</strong> per passare alla schermata di <strong>configurazione dei permessi</strong>.
- Abilitare tutti i permessi toccando sui vari testi come da schermata e premere il pulsante <strong>AVANTI</strong>.
- Arrivati alla schermata di configurazione scrivere nella casella di testo il nome del telefono correttamente com'era scritto in Join e toccare <strong>CHIUDI</strong>.
- Abbiamo finito di configurare tutto il sistema, manca solo da attivare l'assistente vocale alla pressione del tasto fisico dell'auto.

<strong>Per fare questo faccio un esempio con il Carlinkit siccome io posseggo questo:</strong>

- Aprire le impostazioni del box e andare alla voce <strong>Configurazione della navigazione</strong> ed impostare come <strong>Configurazione dell'app di navigazione</strong> una qualsiasi app che non sia il navigatore e così fate anche per <strong>Impostazione del widget di navigazione nel Launcher</strong>.

- Sempre nelle impostazioni andate alla voce <strong>Altre Impostazioni</strong> e impostate come <strong>Assistenza vocale</strong> CarBox Voice.

<h2><p align="center"><strong>Comandi Vocali disponibili su CarBox Voice</strong></p></h2>

- <strong>APRI</strong> nome applicazione
  - Apre l'applicazione richiesta, esempio <strong>APRI YOUTUBE</strong> per aprire YouTube.

- <strong>CHIAMA CONTATTO</strong> nome contatto
  - Chiama un contatto disponibile in rubrica, esempio <strong>CHIAMA CONTATTO MARIO ROSSI</strong> avvia la telefonata dal telefono abbinato.

- <strong>CHIAMA NUMERO</strong> numero di telefono
  - Chiama un numero di telefono, esempio <strong>CHIAMA NUMERO 1234567890</strong> avvia la telefonata dal telefono abbinato.

- <strong>CHIUDI</strong>
  - Manda in background l'applicazione aperta tornando alla schermata iniziale del box.

- <strong>COMANDI</strong>
  - Apre la schermata di tutti i comandi disponibili in CarBox Voice.

- <strong>IMPOSTAZIONI</strong>
  - Apre la schermata delle impostazioni di CarBox Voice.

- <strong>SPOTIFY</strong> nome canzone o artista
    - Apre Spotify con la ricerca della canzone o artista richiesto, esempio <strong>SPOTIFY LIGABUE</strong>.

- <strong>VAI A</strong> indirizzo
  - Apre navigazione GPS con GoogleMaps all'indirizzo impostato, esempio <strong>VAI A VIA CARDUCCI 3 MILANO</strong>.

- <strong>YOUTUBE</strong> nome video
    - Apre YouTube con la ricerca del video richiesto, esempio <strong>YOUTUBE LIGABUE</strong>.

<p align="center">
    <ins><strong>SE TI VA OFFRIMI UN CAFFE PER SOSTENERE LO SVILUPPO DELL'APPLICAZIONE</strong></ins>
</p>
<p align="center">
  <a href="https://www.paypal.com/donate/?business=3LPTNPJ2RV6U8&no_recurring=0&item_name=Offrimi+un+caff%C3%A8+se+ti+va+per+contribuire+allo+sviluppo+dell%27applicazione&currency_code=EUR">
    <img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/DonaPayPal.png" alt="Donate with PayPal" width="300"/>
  </a>
</p>
