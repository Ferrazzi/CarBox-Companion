[CLICCA QUI PER LA GUIDA IN ITALIANO](https://github.com/Ferrazzi/CarBox-Companion/blob/main/README_IT.md)

<h1><p align="center"><strong>CarBox Voice Assistant</strong></p></h1>

</p>
<p align="center">
  <a href="https://www.facebook.com/profile.php?id=61558018811329">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/Facebook_icon.svg/2048px-Facebook_icon.svg.png" alt="Facebook" width="100"/>
  </a>
</p>
</p>
<p align="center">
  <a href="https://t.me/carlinkit_box_possessori_italia ">
    <img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/TelegramButton.jpg" alt="Donate with PayPal" width="200"/>
  </a>
</p>

<p align="center">
    <ins><strong>IF YOU LIKE, BUY ME A COFFEE TO SUPPORT THE APP DEVELOPMENT</strong></ins>
</p>
<p align="center">
  <a href="https://www.paypal.com/donate/?business=3LPTNPJ2RV6U8&no_recurring=0&item_name=Buy+me+a+coffee+if+you+like+to+contribute+to+the+app+development&currency_code=EUR">
    <img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/DonaPayPal.png" alt="Donate with PayPal" width="200"/>
  </a>
</p>


Tap [here](https://github.com/Ferrazzi/CarBox-Companion/releases) to download the latest version of CarBox Companion.

<strong>CarBox Companion</strong> is a voice assistant for in-car box devices (like Carlinkit, Ottocast, etc.) and Android car radios that allows you to perform actions usually done by touching the infotainment screen with voice commands.

The system consists of two main applications, <strong>CarBox Companion</strong> and <strong>CarBox Voice</strong>.
During installation, you will be asked to install an additional application: [AutoInput](https://play.google.com/store/apps/details?id=com.joaomgcd.autoinput) available on Google Play for free with limitations or for a fee in the full version. <strong>I recommend purchasing it to avoid various limitations in the use of the various commands that CarBox Companion executes</strong>.

<img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/CarBoxCompanionIcon.png" alt="" width="50"/> <strong>CarBox Companion</strong>

<strong>CarBox Companion</strong> needs to be installed on the phone to be used in combination with the car box or Android car radio, it serves as a receiver for the master application <strong>CarBox Voice</strong> which must be installed on the car box or Android car radio.

- Once <strong>CarBox Companion</strong> is installed on the phone, simply open it and you will find yourself on the LOGIN screen. If you already have an active account, log in, otherwise create one by tapping the appropriate button. After registering and logging in correctly, you will proceed to the second screen for the installation of the <strong>AutoInput</strong> application and the <strong>CarBoxPlugin</strong> plugin.

- After all this is done, you can press the <strong>NEXT</strong> button to go to the <strong>permissions configuration</strong> screen.
- Enable all permissions by tapping the various buttons and press the <strong>BACK</strong> button.
- Now we finally arrive at the CarBox Companion configuration screen.
- By tapping the <strong>Select Box 1</strong> and <strong>Select Box 2</strong> buttons, a window will open allowing you to select the Bluetooth connection of the <strong>First CarBox</strong> or the <strong>Second CarBox</strong>, if you have another one in another car. It is mandatory to select the Bluetooth connection because it is used to enable not only the tethering function but also the exchange of information for correct functionality. Enable the switch on the right, this is used to enable tethering automatically when the box is detected to be turned on, so as to provide internet connection without having to do it manually.
- Enable the switch for voice command activation if you want to activate box functions towards the phone, such as making calls.
- Enable the switch for automatic parking notifications, this is used to receive a notification when the Bluetooth connection to the phone is interrupted and therefore the box is turned off, assuming the car is parked. A notification will be displayed in the notification panel with parking information, a map with coordinates that can be opened with Google Maps, and possibly the ability to enter a note, for example, the parking spot number at the mall.
- Exit CarBox Companion.
- For making calls, the contacts on the Companion device must be synchronized with the voice device. I recommend enabling sharing via Google account since it is used on both devices.
- At this point, we have finished configuring the <strong>CarBox Companion</strong> part and we can continue to configure <strong>CarBox Voice</strong>.

<img src="https://github.com/Ferrazzi/CarBox-Companion/blob/main/Assets/CarBoxVoiceIcon.png" alt="" width="50"/> <strong>CarBox Voice</strong>

CarBox Voice needs to be installed on the car box or Android car radio.

-  Once <strong>CarBox Voice</strong> is installed on the box, simply open it and log in with the registered credentials from <strong>CarBox Companion</strong>.

- We have finished configuring the entire system, only activating the voice assistant when pressing the car's physical button is left.

<strong>To do this, I'll give an example with Carlinkit since I own this:</strong>

- Open the box settings and go to <strong>Navigation Configuration</strong> and set any app other than the navigator for <strong>Navigation App Configuration</strong>, and do the same for <strong>Navigation Widget Setting in Launcher</strong>.

- Still in the settings, go to <strong>Other Settings</strong> and set <strong>CarBox Voice Assistant</strong>.

<h2><p align="center"><strong>Enable ADB Permissions on CarBox Companion</strong></p></h2>

<strong>Activating permissions from Windows or Mac</strong>

- After installing and configuring all applications, you can proceed with the guide to activate ADB permissions for writing secure settings. This is necessary to enable tethering automatically when the box is detected to be turned on, so as to provide internet connection without having to do it manually, and for AutoInput to allow various actions normally not allowed without rooting the phone.

  - <strong>Enable developer mode on the phone settings:</strong> Go to Android settings -> About phone -> Software information and look for 

  - <strong>Build number</strong>. Tap it several times until developer mode is activated.

  - <strong>Enable USB Debugging:</strong> Go to Android settings -> and look for <strong>Developer options</strong>. Inside this menu, enable the <strong>USB debugging</strong> option.

  - <strong>Install ADB on your PC:</strong> Check [here](https://github.com/Ferrazzi/CarBox-Companion/blob/main/InstallaADB.md) for a quick way to do it.

  - <strong>Connect the device to the PC:</strong> Connect your device to the PC and check your phone. You should see a message asking you to allow debugging of the phone by the PC. <strong>Accept it</strong>.
  - Open the command prompt from the folder containing the downloaded files from the link to the voice <strong>Install ADB on your PC</strong> and extracted. To do this, press the Windows key and type cmd. When the prompt opens, type cd followed by the folder where you downloaded ADB.
  - <strong>Grant permission:</strong> Open a command line on your PC and enter the necessary commands (one at a time)
    
    - <strong>If using Windows:</strong>
      - adb shell pm grant com.joaomgcd.autoapps android.permission.WRITE_SECURE_SETTINGS
      - adb shell pm grant com.joaomgcd.autoinput android.permission.WRITE_SECURE_SETTINGS

    - <strong>If using Mac:</strong>
      - ./adb shell pm grant com.joaomgcd.autoapps android.permission.WRITE_SECURE_SETTINGS
      - ./adb shell pm grant com.joaomgcd.autoinput android.permission.WRITE_SECURE_SETTINGS

<strong>Note:</strong>

On MIUI devices, you may need to open developer options and enable USB Debugging (Security Settings) (and the Turn off monitoring setting)

<strong>Activating permissions from android</strong>

<h2><p align="center"><strong>Voice Commands available on CarBox Voice</strong></p></h2>

- <strong>OPEN</strong> app name
  - Opens the requested application, for example, <strong>OPEN YOUTUBE</strong> to open YouTube.

- <strong>GOOGLE ASSISTANT</strong>
  - Launches Google Assistant

- <strong>CALL CONTACT</strong> contact name
  - Calls a contact available in the phonebook, for example, <strong>CALL CONTACT JOHN SMITH</strong> initiates the call from the paired phone.
  - The new internal contact book allows you to select all the numbers within the searched contact. When the list of the searched contact is displayed, if you press and hold one of the numbers present in the same contact, you can add it to favorites so that it is displayed as the first in the list the next time it is searched.

- <strong>CALL NUMBER</strong> phone number
  - Calls a phone number, for example, <strong>CALL NUMBER 1234567890</strong> initiates the call from the paired phone.

- <strong>COMMANDS</strong>
  - Opens the screen with all available commands in CarBox Voice.

- <strong>SETTINGS</strong>
  - Opens the settings screen.

- <strong>MAPS GO TO</strong> address
  - Opens GPS navigation with GoogleMaps to the set address, for example, <strong>MAPS GO TO 123 Main Street</strong>.

- <strong>SPOTIFY</strong> song name or artist name
  - Opens Spotify with the requested song search, for example, <strong>SPOTIFY song name or artist</strong>.

- <strong>TASKER</strong>
  - Executes a tasker command set in the commands list accessible from CarBox Voice in the Settings screen.

- <strong>YOUTUBE</strong> video name
    - Opens YouTube with the requested video search, for example, <strong>YOUTUBE LIGABUE</strong>.

- <strong>WAZE GO TO</strong> address
  - Opens GPS navigation with Waze to the set address, for example, <strong>WAZE GO TO 123 Main Street</strong>.

<h2><p align="center"><strong>Custom Tasker Commands on CarBox Voice</strong></p></h2>

To set up custom commands using [Tasker](https://play.google.com/store/apps/details?id=net.dinglisch.android.taskerm&hl=en&gl=US) on CarBox Voice, you first need to enter the CarBox Voice settings.
Press the <strong>Tasker Commands</strong> button, and the screen with the list of available created commands will appear.
Press <strong>ADD</strong> to add a new command.
In the various text fields to be filled in, add in sequence:
- In the <strong>Enter name</strong> box:
  - Enter a name of your choice this will be the name and command of the action, e.g. when Tasker is said to CarBox Voice, the next command will be the name of the action and therefore what is entered in this field.
- In the <strong>Enter description</strong> box:
  - Enter a description of your choice for the action this will be visible in the actions list below the name and is useful to remember what that particular action does.
- In the <strong>Enter action</strong> box:
  - Enter the actual action command here that Tasker will receive, for example <strong>com.carboxvoice.send.command</strong>.
- In the <strong>Enter variable</strong> box:
  - Enter here the name of a variable of your choice that Tasker will receive along with the command, for example <strong>text</strong>.
- In the <strong>Enter text</strong> box:
  - Enter here a text that will be used to fill the variable set above and that Tasker will receive, for example, <strong>received</strong>.

Once all the fields are filled, press <strong>SAVE</strong> to save the action and return to the actions list.
Now, you just need to configure Tasker to receive the action we created.

Install and open [Tasker](https://play.google.com/store/apps/details?id=net.dinglisch.android.taskerm&hl=en&gl=US) from the box if it's the first time you open it, it will follow the application's guided setup.
After completing all the setup and Tasker is ready to use, configure the reception of our action created on CarBox Voice.
- Go to <strong>PROFILES</strong> and tap the <strong>+</strong> button at the bottom right.
- Tap <strong>CREATE</strong> and select from the visible menu item <strong>Event</strong>.
- In the text box <strong>Filter</strong>, search for <strong>intent</strong> and tap on the item <strong>Receive Intent</strong>.
- In the action text box, you need to enter the action created on CarBox Voice, so in our case <strong>com.carboxvoice.send.command</strong>, and go back.
- Tap <strong>New Task</strong> and give a name to the new task created to enter the task creation page.
- At this point, let your imagination run wild to create any command you need. I'll make a very simple example where upon receiving a vocal command, a message will be displayed on the screen with the text of the variable set.
- Press the <strong>+</strong> button at the bottom right.
- Search for <strong>Flash</strong> in the filter text box and press the <strong>Flash</strong> button.
- In the <strong>Text</strong> text box, enter the variable created in the action with the <strong>%</strong> symbol in front; in our case, it will be <strong>%text</strong>.
- Return to the <strong>PROFILES</strong> screen and make sure the profile is activated with the switch next to the profile name.

After all the configuration is done, when CarBox Voice is opened and Tasker is said, and the name of the action is pronounced, Tasker will display a popup with our variable on the screen. By modifying this small example, you can create automations of any kind, from opening the automatic gate vocally if domotized to various actions that Tasker can perform on the box.
