<h1><p align="center"><strong>CarBox Voice Assistant</strong></p></h1>

</p>
<p align="center">
  <a href="https://t.me/carlinkit_box_possessori_italia ">
    <img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/TelegramButton.jpg" alt="Donate with PayPal" width="200"/>
  </a>
</p>

<p align="center">
    <ins><strong>IF YOU FEEL LIKE IT, BUY ME A COFFEE TO SUPPORT THE DEVELOPMENT OF THE APPLICATION</strong></ins>
</p>
<p align="center">
  <a href="https://www.paypal.com/donate/?business=3LPTNPJ2RV6U8&no_recurring=0&item_name=Buy+me+a+coffee+if+you+feel+like+it+to+contribute+to+the+development+of+the+application&currency_code=EUR">
    <img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/DonaPayPal.png" alt="Donate with PayPal" width="200"/>
  </a>
</p>


Click [here](https://github.com/Ferrazzi/CarBox-Companion/releases) to download the latest version of CarBox Companion.

<strong>CarBox Companion</strong> is a voice assistant for in-car box devices (such as Carlinkit, Ottocast, etc.) and Android car radios that allows you to perform actions that are usually done by touching the infotainment screen, but with voice commands.

The system consists of two main applications, <strong>CarBox Companion</strong> and <strong>CarBox Voice</strong>.
During installation, you will be prompted to install additional applications such as: [AutoContacts](https://play.google.com/store/apps/details?id=com.joaomgcd.autocontacts) and [AutoInput](https://play.google.com/store/apps/details?id=com.joaomgcd.autoinput), which can be obtained from GooglePlay in a free version with limitations or for a fee in the full version. <strong>I recommend purchasing them to avoid various limitations in the use of voice commands</strong>.

<img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/CarBoxCompanionIcon.png" alt="" width="50"/> <strong>CarBox Companion</strong>

<strong>CarBox Companion</strong> should be installed on the phone to be used in conjunction with the car box or Android car radio. It serves as a receiver for the master application <strong>CarBox Voice</strong>, which should be installed on the car box or Android car radio.

- Once <strong>CarBox Companion</strong> is installed on the phone, simply open it and you will find yourself on the LOGIN screen. If you already have an active account, log in; otherwise, create one by touching the appropriate button. If you register and log in correctly, you will move on to the second screen related to the installation of the two applications <strong>AutoInput</strong> and <strong>AutoContacts</strong>.

- After completing all this, you can press the <strong>NEXT</strong> button to move to the <strong>permissions configuration</strong> screen.
- Enable all permissions by touching the various buttons and press the <strong>BACK</strong> button.
- Now we have finally reached the CarBox Companion configuration screen.
- By tapping the <strong>Select Box 1</strong> and <strong>Select Box 2</strong> buttons, a window will open to select the Bluetooth connection of the <strong>First CarBox</strong> or the <strong>Second CarBox</strong>, if you have another one in another car. It is mandatory to select the Bluetooth connection because it is needed to enable not only tethering function but also information exchange for proper functionality. Enable the switch on the right, this is used to allow automatic tethering activation when the box is detected to be turned on, so as to provide internet connection without having to do it manually.
- Enable the switch for voice command activation if you want to activate box functions towards the phone, for example, calls.
- Enable the switch for automatic parking notifications, this is used to receive a notification when the Bluetooth connection to the phone is interrupted and therefore the box is turned off, assuming that the car is parked. A notification will be displayed in the notification panel with parking information, a map with coordinates that can be opened with GoogleMaps, and possibly the ability to add a note, for example, parking lot number at the mall.
- Exit <strong>CarBox Companion</strong>.
- Open <strong>AutoContacts</strong>, grant any permissions and touch the <strong>Contacts</strong> option. Once in the Contacts screen, touch the <strong>Force Refresh Contacts</strong> option, this will import all your contacts to be used for calls and messages. <strong>IMPORTANT, repeat this operation every time a new contact is added to the address book, otherwise it will not be accessible for use</strong>.
- At this point, we have finished configuring the <strong>CarBox Companion</strong> part and we can continue to configure <strong>CarBox Voice</strong>.

<img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/CarBoxVoiceIcon.png" alt="" width="50"/> <strong>CarBox Voice</strong>

CarBox Voice should be installed on the car box or Android car radio.

- Once <strong>CarBox Voice</strong> is installed on the box, simply open it and log in with the credentials registered in <strong>CarBox Companion</strong>.

- We have finished configuring the entire system, all that remains is to activate the voice assistant by pressing the car's physical button.

<strong>To do this, I'll give an example with Carlinkit since I own this:</strong>

- Open the box settings and go to <strong>Navigation Configuration</strong> and set <strong>Navigation App Configuration</strong> to any app other than the navigation app, and do the same for <strong>Navigation Widget Setting in Launcher</strong>.

- Still in the settings, go to <strong>Other Settings</strong> and set <strong>CarBox Voice Voice Assistance</strong>.

<h2><p align="center"><strong>Enable ADB permissions on CarBox Companion</strong></p></h2>

<strong>Activating permissions from Windows or Mac</strong>

- Once all applications are installed and configured, you can proceed with the guide to activate ADB permissions for writing secure settings, which is necessary to enable automatic tethering when the box is detected to be turned on, providing internet connection without having to do it manually, and for AutoInput to allow various actions normally not allowed without rooting the phone.

  - <strong>Enable developer mode on the phone:</strong> Go to Android settings -> About phone -> Software information and look for

  - <strong>Build number</strong>. Tap it several times until developer mode is activated.

  - <strong>Enable USB Debugging:</strong> Go to Android settings -> and search for <strong>Developer Options</strong>. Inside this menu, enable <strong>USB debugging</strong>.

  - <strong>Install ADB on your PC:</strong> Check [here](https://github.com/Ferrazzi/CarBox-Companion/blob/main/InstallaADB.md) for a quick way to do it.

  - <strong>Connect the device to the PC:</strong> Connect your device to the PC and look at your phone. A message should appear asking you to allow the phone to be debugged by the PC. <strong>Accept it</strong>.
  - Open the command prompt from the folder containing the downloaded files from the link to <strong>Install ADB on your PC</strong> and extracted. To do this, press the Windows key and type cmd. When the prompt opens, type cd followed by the folder where you downloaded ADB.
  - <strong>Grant permission:</strong> Open a command line on your PC and enter the necessary commands (one at a time)
    
    - <strong>If using Windows:</strong>
      - adb shell pm grant com.joaomgcd.autoapps android.permission.WRITE_SECURE_SETTINGS
      - adb shell pm grant com.joaomgcd.autoinput android.permission.WRITE_SECURE_SETTINGS

    - <strong>If using Mac:</strong>
      - ./adb shell pm grant com.joaomgcd.autoapps android.permission.WRITE_SECURE_SETTINGS
      - ./adb shell pm grant com.joaomgcd.autoinput android.permission.WRITE_SECURE_SETTINGS

<strong>Note:</strong>

On MIUI devices, it may be necessary to open the developer options and enable the USB Debugging setting (Security Settings) (and the Turn off Monitoring setting).

<strong>Activating permissions from Android</strong>

<h2><p align="center"><strong>Voice Commands available on CarBox Voice</strong></p></h2>

- <strong>OPEN</strong> app name
  - Opens the requested application, for example <strong>OPEN YOUTUBE</strong> to open YouTube.

- <strong>GOOGLE ASSISTANT</strong>
  - Launches the Google Assistant.

- <strong>CALL CONTACT</strong> contact name
  - Calls a contact available in the address book, for example <strong>CALL CONTACT MARIO ROSSI</strong> initiates the call from the paired phone.

- <strong>CALL NUMBER</strong> phone number
  - Calls a phone number, for example <strong>CALL NUMBER 1234567890</strong> initiates the call from the paired phone.

- <strong>COMMANDS</strong>
  - Opens the screen with all available commands in CarBox Voice.

- <strong>SETTINGS</strong>
  - Opens the settings screen.

- <strong>MAPS GO TO</strong> address
  - Opens GPS navigation with GoogleMaps to the set address, for example <strong>MAPS GO TO VIA CARDUCCI 3 MILANO</strong>.

- <strong>WHATSAPP MESSAGE</strong> contact name
  - Sends a WhatsApp message, for example <strong>WHATSAPP "CONTACT NAME" AND UPON RECEIVING THE NOTIFICATION DICTATE THE MESSAGE</strong>.

- <strong>SPOTIFY</strong> song name or artist name
  - Opens Spotify with the search for the requested song, for example <strong>SPOTIFY song name or artist name</strong>.

- <strong>TASKER</strong>
  - Executes a Tasker command set in the command list reachable from CarBox Voice in the Settings screen.

- <strong>YOUTUBE</strong> video name
    - Opens YouTube with the search for the requested video, for example <strong>YOUTUBE LIGABUE</strong>.

- <strong>WAZE GO TO</strong> address
  - Opens GPS navigation with Waze to the set address, for example <strong>WAZE GO TO VIA CARDUCCI 3 MILANO</strong>.
