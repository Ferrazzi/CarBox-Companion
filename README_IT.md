<p align="center"><img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/LogoOrizzontale.png" alt="CarBox Companion" width="600"/></p>

</p>
<p align="center">
  <a href="https://www.facebook.com/profile.php?id=61558018811329">
    <img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/facebookLogo.jpg" alt="Facebook" width="200"/>
  </a>
  <a href="https://t.me/carlinkit_box_possessori_italia ">
    <img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/TelegramButton.jpg" alt="Donate with PayPal" width="200"/>
  </a>
</p>

<p align="center">
    <ins><strong>SE TI VA OFFRIMI UN CAFFE PER SOSTENERE LO SVILUPPO DELL'APPLICAZIONE</strong></ins>
</p>
<p align="center">
  <a href="https://www.paypal.com/donate/?business=3LPTNPJ2RV6U8&no_recurring=0&item_name=Offrimi+un+caff%C3%A8+se+ti+va+per+contribuire+allo+sviluppo+dell%27applicazione&currency_code=EUR">
    <img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/DonaPayPal.png" alt="Donate with PayPal" width="200"/>
  </a>
</p>


Tocca [qui](https://github.com/Ferrazzi/CarBox-Companion/releases) per scaricare l'ultima versione di CarBox Companion

<strong>CarBox Companion</strong> è un assistente vocale per dispositivi box auto (tipo Carlinkit, Ottocast, ecc..) ed autoradio Android che consente di effettuare delle azioni che solitamente si fanno toccando lo schermo dell'infotainment ma con comandi vocali.

Il sistema è formato da due applicazioni principali, <strong>CarBox Companion</strong> e <strong>CarBox Voice</strong>.
Durante l'installazione verrà richiesto di installare un applicazione aggiuntiva: [AutoInput](https://play.google.com/store/apps/details?id=com.joaomgcd.autoinput) prelevabile da GooglePlay in versione gratuita con limitazioni oppure a pagamento nella versione completa, <strong>consiglio di acquistarla per evitare varie limitazioni nell'uso dei vari comandi che CarBox Companion esegue</strong>.

<img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/CarBoxCompanionIcon.png" alt="" width="50"/> <strong>CarBox Companion</strong>

<strong>CarBox Companion</strong> va installato sul telefono da utilizzare in abbinata al box auto o all'autoradio Android, serve da ricevitore per l'applicazione master <strong>CarBox Voice</strong> che andrà installata sul box auto o autoradio Android.

- Quando <strong>CarBox Companion</strong> è stato installato sul telefono basterà aprirlo e vi troverete sulla schermata di LOGIN. Se avete già un'utenza attiva eseguite l'accesso altrimenti createne una toccando l'apposito pulsante. Registrati e Loggati correttamente passerete alla seconda schermata relativa all'installazione dellì applicazione <strong>AutoInput</strong> e del plugin <strong>CarBoxPlugin</strong>.

- Fatto tutto questo si può premere sul pulsante <strong>AVANTI</strong> per passare alla schermata di <strong>configurazione dei permessi</strong>.
- Abilitare tutti i permessi toccando i vari tasti e premere il pulsante <strong>INDIETRO</strong>.
- Ora siamo arrivati finalmente alla schermata di configurazione di CarBox Companion.
- Toccando i pulsanti <strong>Seleziona Box 1</strong> e <strong>Seleziona Box 2</strong> verrà aperta una finestra che farà selezionare la connessione bluetooth del <strong>Primo CarBox</strong> oppure del <strong>Secondo CarBox</strong>, se ne avete un'altro in un'altra auto. È obbligatorio selezionare la connessione bluetooth perchè serve per abilitare la funzione oltre di tethering anche di scambio informazioni per la corretta funzionalità. Abilitare lo switch sulla destra, questo serve per permettere l'attivazione del tethering automaticamente alla rilevazione del box acceso cosi da dare connessione internet senza doverlo fare manualmente.
- Abilitare lo switch dell'abilitazione comandi vocali se si vogliono attivare le funzioni del box verso il telefono esempio le telefonate.
- Abilitare lo switch per le notifiche di parcheggio automatico, questo serve a ricevere una notifica quando il collegamento bluetooth viene interrotto al telefono e quindi il box è spento presupponendo di avere l'auto in parcheggio. Verrà visualizzata nel pannello notifiche appunto una notifica con le informazioni di parcheggio, una mappa con coordinate apribile con GoogleMaps ed eventualmente la possibilità di inserire una nota esempio numero parcheggio centro commerciale.
- Uscire da <strong>CarBox Companion</strong>
- Per l'utilizzo delle telefonate i contatti del dispositivo Companion devono essere sincronizzati con il dispositivo voice, consiglio di abilitare la condivisione tramite account Google visto che questo viene utilizzato sui due dispositivi.
- A questo punto abbiamo finito di configurare la parte <strong>CarBox Companion</strong> e possiamo continuare a configurare <strong>CarBox Voice</strong>.

<img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/CarBoxVoiceIcon.png" alt="" width="50"/> <strong>CarBox Voice</strong>

CarBox Voice va installato sul box o autoradio Android.

-  Quando <strong>CarBox Voice</strong> è stato installato sul box basterà aprirlo ed eseguire l'accesso con le credenziali registrate <strong>CarBox Companion</strong>.

- Abbiamo finito di configurare tutto il sistema, manca solo da attivare l'assistente vocale alla pressione del tasto fisico dell'auto.

<strong>Per fare questo faccio un esempio con il Carlinkit siccome io posseggo questo:</strong>

- Aprire le impostazioni del box e andare alla voce <strong>Configurazione della navigazione</strong> ed impostare come <strong>Configurazione dell'app di navigazione</strong> una qualsiasi app che non sia il navigatore e così fate anche per <strong>Impostazione del widget di navigazione nel Launcher</strong>.

- Sempre nelle impostazioni andate alla voce <strong>Altre Impostazioni</strong> e impostate come <strong>Assistenza vocale CarBox Voice</strong>.

<h2><p align="center"><strong>Abilitare permessi ADB su CarBox Companion</strong></p></h2>

<strong>Attivazione permessi da Windows o Mac</strong>

- Installate e configurate tutte le applicazioni si può procedere con la guida per attivare i permessi ADB per la scrittura delle impostazioni sicure, questo serve per permettere l'attivazione del tethering automaticamente alla rilevazione del box acceso cosi da dare connessione internet senza doverlo fare manualmente e ad AutoInput per permettere varie azioni normalmente non consentite senza root del telefono.

  - <strong>Abilita nelle impostazioni del telefono la modalità sviluppatore:</strong> Vai nelle impostazioni Android -> Informazioni sul telefono -> Informazioni software e cerca 

  - <strong>Versione build</strong>. Toccalo più volte fino all'attivazione della modalità sviluppatore.

  - <strong>Abilita Debug USB:</strong> Vai nelle impostazioni Android -> e cerca <strong>Opzioni sviluppatore</strong>. Dentro questo menu, abilita l'opzione di <strong>debug USB</strong>.

  - <strong>Installa ADB sul tuo PC:</strong> Controlla [qui](https://github.com/Ferrazzi/CarBox-Companion/blob/main/InstallaADB.md) per un modo rapido per farlo.

  - <strong>Connetti il dispositivo al PC:</strong> Connetti il tuo dispositivo al PC e guarda sul tuo telefono. Dovrebbe venire visualizzato un messaggio che ti chiede di consentire il debug del telefono da parte del PC. <strong>Accettalo</strong>.
  - Apri il prompt dei comandi dalla cartella dei file che contiene i file scaricati in precedenza nel link alla voce <strong>Installa ADB sul tuo PC</strong> ed estratti. Per fare ciò, premi il tasto Windows e digita cmd. Quando si apre il prompt, digita cd seguito dalla cartella in cui hai scaricato l'ADB.
  - <strong>Concedere l'autorizzazione:</strong> Apri una riga di comando sul tuo PC e scrivi i comandi necessari (uno alla volta)
    
    - <strong>Se usi Windows:</strong>
      - adb shell pm grant com.joaomgcd.autoapps android.permission.WRITE_SECURE_SETTINGS
      - adb shell pm grant com.joaomgcd.autoinput android.permission.WRITE_SECURE_SETTINGS

    - <strong>Se usi Mac:</strong>
      - ./adb shell pm grant com.joaomgcd.autoapps android.permission.WRITE_SECURE_SETTINGS
      - ./adb shell pm grant com.joaomgcd.autoinput android.permission.WRITE_SECURE_SETTINGS

<strong>Note:</strong>

Sui dispositivi MIUI potrebbe essere necessario aprire le opzioni sviluppatore e abilitare l'impostazione Debug USB (Impostazioni di sicurezza) (e l'impostazione Disattiva monitoraggio 

<strong>Attivazione permessi da android</strong>

<h2><p align="center"><strong>Comandi Vocali disponibili su CarBox Voice</strong></p></h2>

- <strong>APRI</strong> nome applicazione
  - Apre l'applicazione richiesta, esempio <strong>APRI YOUTUBE</strong> per aprire YouTube.
 
- <strong>ARDUINO</strong> comando
  - Esegue un comando arduino impostato nella lista comandi raggiungibile da CarBox Voice nella schermata Impostazioni.

- <strong>ASSISTENTE GOOGLE</strong>
  - Avvia l'assistente Google

- <strong>CHIAMA CONTATTO</strong> nome contatto
  - Chiama un contatto disponibile in rubrica, esempio <strong>CHIAMA CONTATTO MARIO ROSSI</strong> avvia la telefonata dal telefono abbinato.
  - La nuova rubrica contatti interna permette di selezionare tutti i numeri all'interno del contatto ricercato. Quando viene visualizzata la lista del contatto ricercato se si tiene premuto du uno dei numeri presenti nello stesso contatto  si può inserire nei preferiti facendo in modo che alla prossima ricerca venga visualizzato come primo della lista.

- <strong>CHIAMA NUMERO</strong> numero di telefono
  - Chiama un numero di telefono, esempio <strong>CHIAMA NUMERO 1234567890</strong> avvia la telefonata dal telefono abbinato.

- <strong>COMANDI</strong>
  - Apre la schermata di tutti i comandi disponibili in CarBox Voice.

- <strong>IMPOSTAZIONI</strong>
  - Apre la schermata delle impostazioni.

- <strong>MAPS VAI A</strong> indirizzo
  - Apre navigazione GPS con GoogleMaps all'indirizzo impostato, esempio <strong>MAPS VAI A VIA CARDUCCI 3 MILANO</strong>.

- <strong>MESSAGGIO WHATSAPP</strong> indirizzo
  - Invia un messaggio WhatsApp, esempio <strong>WHATSAPP "NOME CONTATTO" E ALLA RICEZIONE DELL'AVVISO DETTARE IL MESSAGGIO</strong>.

- <strong>SPOTIFY</strong> nome canzone o nome artista
  - Apre Spotify con la ricerca della canzone richiesta, esempio <strong>SPOTIFY nome canzone o artista</strong>.

- <strong>TASKER</strong> comando
  - Esegue un comando tasker impostato nella lista comandi raggiungibile da CarBox Voice nella schermata Impostazioni.

- <strong>YOUTUBE</strong> nome video
    - Apre YouTube con la ricerca del video richiesto, esempio <strong>YOUTUBE LIGABUE</strong>.

- <strong>WAZE VAI A</strong> indirizzo
  - Apre navigazione GPS con Waze all'indirizzo impostato, esempio <strong>WAZE VAI A VIA CARDUCCI 3 MILANO</strong>.

<h2><p align="center"><strong>Comandi Tasker personalizzati su CarBox Voice</strong></p></h2>

Per impostare dei comandi personalizzati di [Tasker](https://play.google.com/store/apps/details?id=net.dinglisch.android.taskerm&hl=it&gl=US) su CarBox Voice bisogna come prima cosa entrare nelle impostazioni di CarBox Voice.
Premere sul pulsante <strong>Comandi Tasker</strong> e si aprirà la schermata con la lista dei comandi creati disponibili.
Premere su <strong>AGGIUNGI</strong> per aggiungere un nuovo comando.
Nei vari campi di testo da compilare aggiungere in sequenza:
- Nella casella <strong>Inserisci nome</strong>
  - Inserire un nome a scelta, questo sarà il nome e comando dell'azione es. quando a CarBox Voice viene detto Tasker e il comando sarà appunto il nome dell'azione e quindi quello inserito in questo campo
- Nella casella <strong>Inserisci descrizione</strong>
  - Inserire una descrizione a scelta per l'azione, questa sarà visibile nella lista azioni sotto al nome ed è utile per ricordarsi cosa fa quella determinata azione.
- Nella casella <strong>Inserisci azione</strong>
  - Inserire qui il comando azione vero e proprio che riceverà tasker esempio <strong>com.carboxvoice.send.command</strong>
- Nella casella <strong>Inserisci variabile</strong>
  - Inserire qui il nome di una variabile a scelta che riceverà Tasker insieme al comando esempio <strong>text</strong>
- Nella casella <strong>Inserisci testo</strong>
  - Inserire qui un testo che servirà a riempire la variabile sopra impostata e che Tasker ricevera esempio <strong>received</strong>

Compilati tutti i campi premere su <strong>SALVA</strong> per salvare l'azione e tornare alla lista azioni.
Non i resta che configurare Tasker per la ricezione dell'azione che abbiamo creato.

Installare e aprire [Tasker](https://play.google.com/store/apps/details?id=net.dinglisch.android.taskerm&hl=it&gl=US) dal box, se è la prima volta che lo aprite seguirà configurazione guidata dell'applicazione.
Completata tutta la configurazione e quindi Tasker è pronto all'utilizzo configuriamo la ricezione della nostra azione creata su CarBox Voice.
- Andare su <strong>PROFILI</strong> e toccare il stasto <strong>+</strong> in basso a destra.
- Toccare <strong>CREARE</strong> e selezionare dal menù visibile la voce <strong>Evento</strong>
- Nella casella di testo <strong>Fltri</strong> cercare <strong>intent</strong> e toccare la voce <strong>Ricevi Intent</strong>
- Nella asella di testo azione bisogna inserire l'azione creata su CarBox Voice quindi nel nostro caso <strong>com.carboxvoice.send.command</strong> e tornare indietro.
- Toccare <strong>Nuovo Task</strong> e dare un nome al nuovo task creato cosi da entrare nella pagina di creazione del task.
- A questo punto si da il via alla fantasia per creare qualsiasi comando vi serva, farò un esempio molto semplice dove alla ricezione vocale del comando verrà mostrato un messaggio a viedeo con il testo della variabile impostata.
- Premere sul pulsante <strong>+</strong> in basso a destra
- Cercare <strong>Flash</strong> nella casella di test dei filtri e premere sul tasto <strong>Flash</strong>
- Nella casella di testo <strong>Testo</strong> inserire la variabile creata nell'azione con il simbolo <strong>%</strong> davanti nel nostro caso sarà <strong>%text</strong>.
- Tornare nella schermata <strong>PROFILI</strong> ed assicurarsi che il profilo sia attivato con lo switch accanto al nome del profilo.

Finita tutta la configurazione quando si aprirà CarBox Voice e si dirà Tasker e si pronuncerà il nome dell'azione, Tasker mostrerà a video un popup con la nostra variabile. Modificando questo piccolo esempio si possono creare automazioni di qualsiasi tipo, dall'aprire cancello automatico vocalmente se domotizzato a varie azioni che può svolgere Tasker sul box.

<h2><p align="center"><strong>Comandi Arduino personalizzati su CarBox Voice</strong></p></h2>

Per impostare dei comandi personalizzati di Arduino su CarBox Voice bisogna come prima cosa entrare nelle impostazioni di CarBox Voice.
Premere sul pulsante <strong>Comandi Arduino</strong> e si aprirà la schermata con la lista dei comandi creati disponibili.
Premere su <strong>AGGIUNGI</strong> per aggiungere un nuovo comando.
Nei vari campi di testo da compilare aggiungere in sequenza:
- Nella casella <strong>Inserisci nome</strong>
  - Inserire un nome a scelta, questo sarà il nome e comando dell'azione es. quando a CarBox Voice viene detto Arduino e il comando sarà appunto il nome dell'azione e quindi quello inserito in questo campo
- Nella casella <strong>Inserisci descrizione</strong>
  - Inserire una descrizione a scelta per l'azione, questa sarà visibile nella lista azioni sotto al nome ed è utile per ricordarsi cosa fa quella determinata azione.
- Nella casella <strong>Inserisci azione</strong>
  - Inserire qui il comando azione vero e proprio che riceverà Arduino esempio <strong>TestComando</strong>
- Seleziona dalla lista il bluetooth del tuo Arduino

Compilati tutti i campi premere su <strong>SALVA</strong> per salvare l'azione e tornare alla lista azioni.
Non i resta che configurare Arduino per la ricezione dell'azione che abbiamo creato.

- Scaricare il file [Arduino_Template](https://github.com/Ferrazzi/CarBox-Companion/blob/main/Arduino/Arduino_Template.ino)
