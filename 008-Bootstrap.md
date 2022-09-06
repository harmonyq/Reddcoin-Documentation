# Bootstrapping


## What is it?

> Blockchain data synchonization, using archive files of the original decentralized network.
Syncing a blockchain is always a time consuming and painful process. Fortunately, with the Reddcoin Core Bootstrap, you can speed up the syncing of the blockchain on a fresh install or not of Reddcoin Core as uploading all. This process is not mandatory, but will cut synchronization times down dramatically when used.


## Instructions

#### Video instructions:
> *   For macOS: [https://www.youtube.com/watch?v=KeBJWRNWTZY](https://www.youtube.com/watch?v=KeBJWRNWTZY)

> *   For Windows: [https://www.youtube.com/watch?v=lYcu5BA3RDo](https://www.youtube.com/watch?v=lYcu5BA3RDo)

Step 1: Back up wallet
Always make a back up of your wallet first if you have any Reddcoins in your wallet. Do not skip this step.

You can read here how to make a back up.
Step 2: Check if most recent version of Reddcoin Core is installed
It is important to use/run the most recent version of Reddcoin Core, as the most recent version will have bugfixes and improvements.

Currently, the most recent version is: Reddcoin Core v3.10.4.

To check the version of your Reddcoin Core, follow these steps:
·         Open Reddcoin Core.

·         Open 'Debug window', via 'Help' (menu) -> 'Debug window'.
↳ Screenshot

·         The ‘Debug window’ appears on the screen, showing the 'Information' tab.
Client version will tell you your Reddcoin Core version.

It should be v3.10.4.
↳ Screenshot

·         If your version is v3.10.4, you are running the most recent version. You can continue with step 3 below.

If your version is not v3.10.4 (and thus older), you should update Reddcoin Core first.
More info about updating can be found here: Updating Reddcoin Core to a newer version.
After you have updated, you can continue with step 3 below.
Step 3: Find your Reddcoin data directory
Your Reddcoin data directory contains important files used by Reddcoin Core, like the Reddcoin blockchain files and the wallet file. You need to know where your Reddcoin data directory is located, as you need to copy some files into this directory in the next steps.
·         Open Reddcoin Core.

·         Open 'Debug window', via 'Help' → 'Debug window'.
↳ Screenshot

·         The ‘Debug window’ appears on the screen, showing the ‘Information’ tab. Click on the ‘Open’ button at the bottom to open the ‘Debug log file’.
↳ Screenshot

·         The debug log file will be opened.
Search for the following in the file (CTRL + F) to see your data directory:
Using data directory
↳ Screenshot

In this example, the Reddcoin data directory is “C:\Blockchain\Reddcoin“.

·         Close/exit Reddcoin Core, via File -> Exit.
↳ Screenshot

·         Open your Reddcoin data directory using Windows File Explorer.
In my case, it’s “C:\Blockchain\Reddcoin“.
↳ Screenshot

·         Delete these two folders:

o	blocks
o	chainstate

·         Delete this file:

o	peers.dat

·         Leave this window open.
↳ Screenshot

Step 4: Download and extract the bootstrap file
You need to download the bootstrap file, and place the contents in your Reddcoin data.
·         Download the bootstrap file (.zip file – 4.5 GB):
https://download.reddcoin.com/bin/bootstrap/blockchain-latest.zip

·         After the file is downloaded, the next step is to copy the contents of the bootstrap file to your Reddcoin data directory.

Browse to the folder where the bootstrap file is saved.
Right click on the file → 'Open with' → Windows Explorer.
↳ Screenshot

·         The contents of the bootstrap file will be shown (two folders: blocks and chainstate).
Copy/move these folders to your Reddcoin data directory (the window from the previous step that is still open, where you deleted the files/folders earlier).
You can 'drag and drop', 'right click copy, right click paste' or 'CTRL + C, CTRL +V'.
↳ Screenshot
↳ Screenshot

Step 5: Finish the sync
Start Reddcoin Core. If you did everything correctly, you should sync only a few days of blockchain data, instead of more than 6 years. Wait until the blockchain is fully synced before doing any transactions.

To speed up the weeks syncing, you can do the following:
·         In Reddcoin Core, go to: Help (menu) → Debug window → Peers.
↳ Screenshot

·         Make the Peers window wider.

·         You are interested in the column 'User Agent' (2nd column).
Make the column wider to see its contents.
↳ Screenshot

·         Peers with User Agent “Reddcoin:3” use Reddcoin Core v3.
These peers are OK.

Peers with User Agent "Reddcoin:1" use Reddcoin Core v1.
Peers with User Agent "Reddcoin:2" use Reddcoin Core v2.
These peers are using outdated versions of Reddcoin Core, stop connecting to these peers by banning them. Right click on these peers and ban them for 1 year.
↳ Screenshot

·         Until the blockchain is fully synced, check the peers window every few minutes.
If you see new peers with "Reddcoin:1" or "Reddcoin:2", ban them as well.

·         I can recommend checking Peers and banning peers using older versions of Reddcoin Core (v1/v2) even after Reddcoin Core is fully synced. Not using v1/v2 peers help to keep your network traffic low and your blockchain data healthy.
When Reddcoin Core is fully synced, you can start using it!

