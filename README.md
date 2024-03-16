# kb42
Split 42 key keyboard utilizing Redragon low profile keys

It is heavily inspired by the [Budgy](https://github.com/doesntfazer/Budgy)
while also being heavily influenced in design my the
[Cheapino](https://github.com/tompi/cheapino).

Build guides coming soon. Source code for the firmware
for the keyboard can be found in my [qmk fork](https://github.com/TyGuy60401/qmk_firmware).
In the assets folder you can find some pics and the
.uf2 firmware files that you can download to flash the
board yourself without having to build the entire qmk
compilation suite. One of the firmware files is a via
compatible version of the firmware for the keyboard,
and the other uses a very basic layout which is quite
limited.

Via firmware guide
------------------

Because my firmware isn't in the official via firmware
repo, in order to use via with this keyboard you will
need to follow a few extra steps the first time you
use it.


After flashing the [via specific firmware](https://github.com/TyGuy60401/kb42/blob/3ecddecb2256828aa2ff203ea3fbf5516b5cc939/assets/firmware/kb42_via.uf2)
to the keyboard and connecting the keyboard to your computer
navigate to the [via website](usevia.app) and press `authorize
device`.  Select kb42 in the dropdown that appears and
you'll enter the app.


Usually you can start changing the keymaps to the board
at this point but we need an extra step. Go to the settings
icon in the top center and select enable the option
that says `Show Design Tab`. Now a new paintbrush icon
has appeared above. Select that tab and click `Load
Draft Definition`. That will prompt you to upload a
json file that corresponds to some via specific definitions
for this keyboard. Upload [this json file](https://github.com/TyGuy60401/kb42/blob/dc6ad67e50948e26156101fd82f4def80222cbb4/assets/firmware/kb42_via-definition.json)
which can be found in this repo -> assets -> firmware
-> kb42_via-definition.json

Once that file is uploaded and the via app accepts it
you'll be able to change all of the configuration for
the board. You can see the configuration that I'm using
for the board by uploading configuration file called
[`kb42_TyGuy60401_layout.json`](https://github.com/TyGuy60401/kb42/blob/dc6ad67e50948e26156101fd82f4def80222cbb4/assets/firmware/kb42_TyGuy60401_layout.json) which can be found in
the firmware folder.

