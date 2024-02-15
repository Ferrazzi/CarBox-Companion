<h1><p align="center"><strong>Assistente vocale CarBox</strong></p></h1>


<strong>CarBox Companion</strong> è un assistente vocale per dispositivi box auto (tipo Carlinkit, Ottocast, ecc..) ed autoradio Android che consente di effettuare delle azioni che solitamente si fanno toccando lo schermo dell'infotainment ma con comandi vocali.

Il sistema è formato da due applicazioni principali, <strong>CarBox Companion</strong> e <strong>CarBox Voice</strong>.
Durante l'installazione verrà richiesto di installere applicazioni aggiuntive quali: [Autovoice](https://play.google.com/store/apps/details?id=com.joaomgcd.autovoice), [AutoContacts](https://play.google.com/store/apps/details?id=com.joaomgcd.autocontacts), [AutoShare](https://play.google.com/store/apps/details?id=com.joaomgcd.autoshare) e [Join](https://play.google.com/store/apps/details?id=com.joaomgcd.join) tutte prelevabili da GooglePlay e in versione gratuita con limitazioni oppure a pagamento nella versione completa.

<img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/CarBoxCompanionIcon.png" alt="" width="50"/> <strong>CarBox Companion</strong>

<strong>CarBox Companion</strong> va installato sul telefono da utilizzare in abbinata al box auto o all'autoradio Android, serve da ricevitore per l'applicazione master <strong>CarBox Voice</strong> che andrà installata sul box auto o autoradio Android.

- Quando <strong>CarBox Companion</strong> è stato installato sul telefono basterà aprirlo e sarete guidati nell'installazione delle due applicazioni [Join](https://play.google.com/store/apps/details?id=com.joaomgcd.join) e [AutoContacts](https://play.google.com/store/apps/details?id=com.joaomgcd.autocontacts).
- Installate le due applicazioni si può procedere con la guida per attivare i permessi ADB per la scrittura delle impostazioni sicure.

  - <strong>Abilita nelle impostazioni del telefono la modalità sviluppatore:</strong> Vai nelle impostazioni Android -> Informazioni sul telefono -> Informazioni software e cerca 

  - <strong>Versione build</strong>. Toccalo più volte fino all'attivazione della modalità sviluppatore.

  - <strong>Abilita Debug USB:</strong> Vai nelle impostazioni Android -> e cerca <strong>Opzioni sviluppatore</strong>. Dentro questo menu, abilita l'opzione di <strong>debug USB</strong>.

  - <strong>Installa ADB sul tuo PC:</strong> Controlla [qui](https://github.com/Ferrazzi/CarBox-Companion/blob/main/InstallaADB.txt) per un modo rapido per farlo.

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
- A questo punto abbiamo finito di configurare la parte <strong>CarBox Companion</strong> e possiamo continuare a configurare <strong>CarBox Voice</strong>.

<img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/CarBoxVoiceIcon.png" alt="" width="50"/> <strong>CarBox Voice</strong>


<p align="center">
    <ins><strong>SE TI VA OFFRIMI UN CAFFE PER SOSTENERE LO SVILUPPO DELL'APPLICAZIONE</strong></ins>
</p>
<p align="center">
  <a href="https://www.paypal.com/donate/?business=3LPTNPJ2RV6U8&no_recurring=0&item_name=Offrimi+un+caff%C3%A8+se+ti+va+per+contribuire+allo+sviluppo+dell%27applicazione&currency_code=EUR">
    <img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/DonaPayPal.png" alt="Donate with PayPal" width="300"/>
  </a>
</p>
