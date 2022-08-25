# Wallets
 
## Official client implementation

Once you install official Reddcoin client from reddcoin.com or redd.love, you’ll have access to three executables: reddcoind, reddcoin-qt, and reddcoin-cli.

### Reddcoin Wallet

'reddcoin-qt' provides a combination full Reddcoin network client and wallet. Reddcoin-qt is highly portable application written in QT5 framework. From the Help menu, you can access a console where you can enter the RPC commands so power-user features are still available.
 
### reddcoind
'reddcoind' provides a full peer which you can interact with through JSON-RPC interface on port 9902 (9904 for testnet).
 
reddcoin-cli
reddcoin-cli allows you to send JSON-RPC commands to running instance of reddcoind from the command line. For example:
 
reddcoin-cli help
reddcoin-cli getinfo
 
All three programs get settings from reddcoin.conf in the Reddcoin application directory:
 
Windows: %APPDATA%\Reddcoin\
OSX: $HOME/Library/Application Support/ReddCoin/
Linux: $HOME/.reddcoin/
 
To use reddcoind  and reddcoin-cli, you will need to add a RPC password to your reddcoin.conf file. Both programs will read from the same file if both run on the same system as the same user, so any long random password will work:
 
         	rpcpassword=change_this_to_a_long_random_password
You should also make the reddcoin.conf file only readable to its owner. On Linux, Mac OSX, and other Unix-like systems, this can be accomplished by running the following command in the Reddcoin application directory:
 
chmod 0600 reddcoin.conf
 
 
 
Reddcoin Core Wallet     	
 
Windows Installation
 
To install on Windows, you can find the download files here: https://www.reddcoin.com/reddwallet.html#rddwallet or https://redd.love/technology/ . Once download is complete, extract the contents of the folder. Depending on if your system is x32 or x64 bits, choosing the relevant folder. Run the reddcoin-win_setup.exe and you will be guided through the installation process. Once finishes, the client can be launched by running "reddcoin-qt.exe" from the appropriate folder.
 
Mac Installation
To install for MacOS, you can find the download files here:
https://www.reddcoin.com/reddwallet.html#rddwallet or https://redd.love/technology/ . Once the download is complete, extract the contents of the folder. Inside the extracted folder, double click the "Reddcoin-Qt.dmg" file to open the client.
 
Debian Installation
As of 20XX, Reddcoin has official Debian repository hosted at https://... . Repository is serving .deb packages for latest Debian stable, for amd64, arm64 and armhf hardware architectures……….
 
Adding the GPG key
wget -O - https://reddcoin.github.io/deb-repo/peercoin.apt.key | sudo apt-key add –
 
Adding the repository in the sources
sudo sh -c "echo 'deb https://reddcoin.github.io/deb-repo/ buster main' >> /etc/apt/sources.list.d/reddcoin.list"
sudo apt update
 
Installing the packages
sudo apt install reddcoin-qt
 
 
 
 
General Notes
Wallet Encryption
When a wallet is first generated, it will be unencrypted. In order to encrypt the wallet, one must go to Settings > Encrypt Wallet. The client will then prompt the user for a password which will then be used to verify transactions and unlock the wallet for staking in the future. It is important to make sure this password is remembered as losing access means losing access to any coins held in that wallet. A wallet must be encrypted in order to participate in staking.
Backups
It is strongly recommended that a backup of the wallet.dat is made and kept in a separate location in the event of hardware failure or similar disaster. Choosing File > Backup Wallet, will present the user with the option of where to export this file.
 
 
Wallet Overview
 
From this tab you can see the "Available", "Pending", and "Total" balance of your Reddcoin wallet. On the right side, you can see your "Recent transactions" as well which will show the most recent transactions that have come into the wallet recently.
 
Send
The send tab is used to send Reddcoin. The "Pay To" section is where a target address can be entered. If you wish to label the address for future use, such as an exchange, you may add it to your address book. Amount determines the quantity of Reddcoin which will be sent in the transaction. If the wallet is encrypted, the secure password must be entered before the send transaction can be finalized.
Receive
The Receive tab lists all wallet addresses attached to the Reddcoin client. Generating a new address is as simple as clicking the "New Address" button at the bottom of the screen. The "Sign Message" button can also be used to verify ownership of a wallet. [There is a tutorial on signing messages with the Reddcoin client here. The example addresses have been removed from the image for privacy sake.]
Transactions
The Transactions tab gives a full history of recent transactions that have come in and out of the wallet since its creation. It will list the Date, Type, Address, and Amount. This information can be exported as a .csv using the "Export" button on the bottom right of the screen. The amounts have been removed from the image for privacy sake.
Staking
Will be written later… !!!
 
Addresses
Addresses is the final tab and displays the addresses saved to the Address Book from the Send tab. This is handy for managing repeat use addresses such as exchanges. The example address has been removed from the image for privacy sake.
 
Creating a New Address
Creating a new address is very simple. Navigate to the "Receive" tab and select the "New Address" button. A window with a "Label" and "Address" field will appear. Enter the name you want in the "Label" field. You will be able to change this later. Leave the "Address" field blank. Click "Ok" to continue. If you have already encrypted your wallet, you will need to enter your wallet password.
You can see the new address now available. If you want to change the name of the label of the address, double click the name and you will be able to enter a new one.
 
 
Sending Reddcoin
If you want to send Reddcoin, navigate to the "Send" tab. We are going to send some Reddcoins to the address we created above. This page has three fields: "Pay To", "Label", and "Amount". Paste the address you want to send Reddcoins to into the "Pay To" field. Make sure to verify that this address is correct. If you already have a label for this wallet, it will automatically fill in the "Label" field. If not, you can write your own in and it will be saved in your address book (Under the "Address" tab). In the amount field, insert the number of Reddcoins you would like to send. There is a drop down menu which allows you to determine if you want to send in denominations of "Reddcoins", "MilliReddcoins", "MicroReddcoins". Make sure that you have enough to pay for the transaction fee. When everything is finalized, press the "Send" button to confirm the transaction. You will be prompted to confirm the transaction and must enter your wallet password to verify the transaction. Once this is completed, you can view the transaction under the "Transactions" tab.
