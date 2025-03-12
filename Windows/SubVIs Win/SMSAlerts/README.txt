   _____       _______       _____ ______ _   _    =
  / ____|   /\|__   __|/\   / ____|  ____| \ | |   =
 | |       /  \  | |  /  \ | |  __| |__  |  \| |   = 
 | |      / /\ \ | | / /\ \| | |_ |  __| | . ` |   =
 | |____ / ____ \| |/ ____ \ |__| | |____| |\  |   =
  \_____/_/  __\_\_/_/    \_\_____|______|_| \_|   =
  / ____|  \/  |/ ____|                            =
 | (___ | \  / | (___                              =
  \___ \| |\/| |\___ \                             =
  ____) | |  | |____) |                            =
 |_____/|_|_ |_|_____/__ _____ _______             =
     /\   | |    |  ____|  __ \__   __|            =
    /  \  | |    | |__  | |__) | | |               =
   / /\ \ | |    |  __| |  _  /  | |               =
  / ____ \| |____| |____| | \ \  | |               =
 /_/____\_\______|______|_|__\_\_|_|_ __  __       =
  / ____\ \   / / ____|__   __|  ____|  \/  |      =
 | (___  \ \_/ / (___    | |  | |__  | \  / |      =
  \___ \  \   / \___ \   | |  |  __| | |\/| |      =
  ____) |  | |  ____) |  | |  | |____| |  | |      =
 |_____/ __|_|_|_____/   |_|  |______|_|  |_|      =
 \ \    / / |__ \       / _ \       / _ \          =
  \ \  / /     ) |     | | | |     | | | |         =
   \ \/ /     / /      | | | |     | | | |         =
    \  /     / /_   _  | |_| |  _  | |_| |         =
     \/     |____| (_)  \___/  (_)  \___/   	   =
====================================================
This is version 2.0.0 of the Catagen SMS alert system. The previous version (developed circa March - April 2019) is now incompatible with the Twillio API.

This is the readme for the Catagen SMS alert sysem. The system uses a DLL file (SMSAlerts.dll) written in C# which takes two parameters:
A1 - A string array of phone numbers and;

A2 - A string of the text to be sent

The program will iterate through each number in the array and send the number through to all of them. Each number will receive the same text.

The SMSAlerts.dll file calls the Twillio.dll file which connects the SMSAlerts application to the online API and POSTs 5 variables;
B1: A string which must be a phone number which is the sender, this has been set to 'CATAGEN'

B2: A string which must be a phone number that is the reciever which the API will send a text to (refer to A1)

B3: A string which is the text to be sent

B4: 