# The Freedom Coin Masternode Setup Guide (Ubuntu 16.04)

This guide will assist you in setting up a The Freedom Coin Masternode on a Linux Server running Ubuntu 16.04. (Use at your own risk)

If you require further assistance contact the support team @  [Discord](https://discord.gg/MX28atT)

Thanks to RealBitYoda (RIP) and Himesh for updating the script!

----------

## [](https://github.com/Realbityoda/FreedomCoin#requirements)Requirements

1.  **5,000 TFC coins.**
2.  **A Vultr VPS running Linux Ubuntu 16.04.**
3.  **A Windows local wallet.**
4.  **An SSH client such as  [Bitvise](https://dl.bitvise.com/BvSshClient-Inst.exe)**

----------

## [](https://github.com/Realbityoda/FreedomCoin#contents)Contents

-   **Section A**: Creating the VPS within  [Vultr](https://www.vultr.com/?ref=7296974).
-   **Section B**: Downloading and installing Bitvise.
-   **Section C**: Connecting to the VPS and installing the MN script via Bitvise.
-   **Section D**: Preparing the local wallet.
-   **Section E**: Connecting & Starting the masternode.

----------

## [](https://github.com/Realbityoda/FreedomCoin#section-a-creating-the-vps-within-vultr)Section A: Creating the VPS within  [Vultr](https://www.vultr.com/?ref=7296974)

_**Step 1**_

-   Register at  [Vultr](https://www.vultr.com/?ref=7296974)

----------

_**Step 2**_

-   After you have added funds to your account go  [here](https://my.vultr.com/deploy/)  to create your Server

----------

_**Step 3**_

-   Choose a server location (preferably somewhere close to you)  [![Location](https://camo.githubusercontent.com/726f38950e2f82c45b83f2fb9c3d8ca36bffdb27/68747470733a2f2f692e696d6775722e636f6d2f6f7a6937426b722e706e67)](https://camo.githubusercontent.com/726f38950e2f82c45b83f2fb9c3d8ca36bffdb27/68747470733a2f2f692e696d6775722e636f6d2f6f7a6937426b722e706e67)

----------

_**Step 4**_

-   Choose a server type: Ubuntu 16.04  [![OS](https://camo.githubusercontent.com/88246bd470b091bf8318ee450db4dde8f9185b94/68747470733a2f2f692e696d6775722e636f6d2f61534d7148554b2e706e67)](https://camo.githubusercontent.com/88246bd470b091bf8318ee450db4dde8f9185b94/68747470733a2f2f692e696d6775722e636f6d2f61534d7148554b2e706e67)

----------

_**Step 5**_

-   Choose a server size: $5/mo will be fine  [![OS](https://camo.githubusercontent.com/6efcd9f23f6ddf7ca046ee39e361597b691a192e/68747470733a2f2f692e696d6775722e636f6d2f556f476f48634d2e706e67)](https://camo.githubusercontent.com/6efcd9f23f6ddf7ca046ee39e361597b691a192e/68747470733a2f2f692e696d6775722e636f6d2f556f476f48634d2e706e67)

----------

_**Step 6**_

-   Set a Server Hostname & Label (name it whatever you want)  [![Hostname](https://camo.githubusercontent.com/a3a8e68d8e0f46b1b32bd09dfcb1adc21af42923/68747470733a2f2f692e696d6775722e636f6d2f75753072764f722e706e67)](https://camo.githubusercontent.com/a3a8e68d8e0f46b1b32bd09dfcb1adc21af42923/68747470733a2f2f692e696d6775722e636f6d2f75753072764f722e706e67)

----------

_**Step 7**_

-   Click "Deploy now"

[![Deploy](https://camo.githubusercontent.com/6e59f5b0bc55bf11db7063400ec2f520e01bbd9b/68747470733a2f2f692e696d6775722e636f6d2f347170597548302e706e67)](https://camo.githubusercontent.com/6e59f5b0bc55bf11db7063400ec2f520e01bbd9b/68747470733a2f2f692e696d6775722e636f6d2f347170597548302e706e67)

----------

## [](https://github.com/Realbityoda/FreedomCoin#section-b-downloading-and-installing-bitvise)Section B: Downloading and installing BitVise.

_**Step 1**_

-   Download Bitvise  [here](https://dl.bitvise.com/BvSshClient-Inst.exe)

----------

_**Step 2**_

-   Select the correct installer depending upon your operating system. Then follow the install instructions.

[![Bitvise-Installer](https://camo.githubusercontent.com/8dd1d1119ccfae158da86a0f6e6f7aaa19e8ae89/68747470733a2f2f692e696d6775722e636f6d2f794633363934472e706e67)](https://camo.githubusercontent.com/8dd1d1119ccfae158da86a0f6e6f7aaa19e8ae89/68747470733a2f2f692e696d6775722e636f6d2f794633363934472e706e67)

----------

## [](https://github.com/Realbityoda/FreedomCoin#section-c-connecting-to-the-vps--installing-the-mn-script-via-bitvise)Section C: Connecting to the VPS & Installing the MN script via Bitvise.

_**Step 1**_

-   Copy your VPS IP (you can find this by going to the server tab within Vultr and clicking on your server.  [![Vultr](https://camo.githubusercontent.com/3794aa2045be353ce1f27394f0adc4f8a6ee066f/68747470733a2f2f692e696d6775722e636f6d2f7a34314d6977592e706e67)](https://camo.githubusercontent.com/3794aa2045be353ce1f27394f0adc4f8a6ee066f/68747470733a2f2f692e696d6775722e636f6d2f7a34314d6977592e706e67)

----------

_**Step 2**_

-   Open the bitvise application and fill in the "Hostname" box with the IP of your VPS.  [![Bitvise-Installer](https://camo.githubusercontent.com/1e507520904d317f9f24358f2e44652c4efa986e/68747470733a2f2f692e696d6775722e636f6d2f766b4e31616c432e706e67)](https://camo.githubusercontent.com/1e507520904d317f9f24358f2e44652c4efa986e/68747470733a2f2f692e696d6775722e636f6d2f766b4e31616c432e706e67)

----------

_**Step 3**_

-   Copy the root password from the VULTR server page.  [![RootPass](https://camo.githubusercontent.com/5905c8f2c5dd12f5ebe06fce11a1018389290274/68747470733a2f2f692e696d6775722e636f6d2f4a6e58515861762e706e67)](https://camo.githubusercontent.com/5905c8f2c5dd12f5ebe06fce11a1018389290274/68747470733a2f2f692e696d6775722e636f6d2f4a6e58515861762e706e67)

----------

_**Step 4**_

-   Type "root" as the login/username.  [![Root](https://camo.githubusercontent.com/b00482104e5ee6e000ac7eb7b3ff81c0f5042916/68747470733a2f2f692e696d6775722e636f6d2f3131474d6b76412e706e67)](https://camo.githubusercontent.com/b00482104e5ee6e000ac7eb7b3ff81c0f5042916/68747470733a2f2f692e696d6775722e636f6d2f3131474d6b76412e706e67)

----------

_**Step 5**_

-   Paste the password into the Bitvise terminal by right clicking (it will not show the password so just press enter)  [![RootPassEnter](https://camo.githubusercontent.com/f08703c7e251c0718e9b55b9257272e2696aca00/68747470733a2f2f692e696d6775722e636f6d2f7a56684f414b752e706e67)](https://camo.githubusercontent.com/f08703c7e251c0718e9b55b9257272e2696aca00/68747470733a2f2f692e696d6775722e636f6d2f7a56684f414b752e706e67)

----------

_**Step 6**_

-   Once you have clicked open it will open a security alert (click yes).

----------

_**Step 7**_

-   Paste the code below into the Bitvise terminal then press enter (it will just go to a new line)  [![RootPassEnter](https://camo.githubusercontent.com/16a25c7c91ab6e92802c8c6e6752f296d761da80/68747470733a2f2f692e696d6775722e636f6d2f4b36786c6e61762e706e67)](https://camo.githubusercontent.com/16a25c7c91ab6e92802c8c6e6752f296d761da80/68747470733a2f2f692e696d6775722e636f6d2f4b36786c6e61762e706e67)

`wget -q https://github.com/louisnelza/FreedomCoin/blob/master/myfreedom_install.sh`

----------

_**Step 8**_

-   Paste the code below into the Bitvise terminal then press enter

`bash myfreedom_install.sh`

[![Bash](https://camo.githubusercontent.com/62a2a524ead43bd959bda3cec031a12a3022d659/68747470733a2f2f692e696d6775722e636f6d2f6d79766d4b54452e706e67)](https://camo.githubusercontent.com/62a2a524ead43bd959bda3cec031a12a3022d659/68747470733a2f2f692e696d6775722e636f6d2f6d79766d4b54452e706e67)

----------

_**Step 9**_

-   Sit back and wait for the install (this will take 10-20 mins)

----------

_**Step 10**_

-   When prompted to enter your Gen key - press enter

[![installing](https://camo.githubusercontent.com/6a767f47fc47888dc7a0ee309c0a8e563bdc069c/68747470733a2f2f692e696d6775722e636f6d2f734c76576431532e706e67)](https://camo.githubusercontent.com/6a767f47fc47888dc7a0ee309c0a8e563bdc069c/68747470733a2f2f692e696d6775722e636f6d2f734c76576431532e706e67)

----------

_**Step 11**_

-   You will now see all of the relavant information for your server.
-   Keep this terminal open as we will need the info for the wallet setup.  [![installing](https://camo.githubusercontent.com/8e2b8ea234fbfd0cb11bdcfb17f44c72ff8bfcbd/68747470733a2f2f692e696d6775722e636f6d2f3930734f4e48632e706e67)](https://camo.githubusercontent.com/8e2b8ea234fbfd0cb11bdcfb17f44c72ff8bfcbd/68747470733a2f2f692e696d6775722e636f6d2f3930734f4e48632e706e67)

----------

## [](https://github.com/Realbityoda/FreedomCoin#section-d-preparing-the-local-wallet)Section D: Preparing the Local wallet

_**Step 1**_

-   Download and install the The Freedom Coin wallet  [here](https://github.com/TheFreedomCoin/Freedom-Coin/releases)

----------

_**Step 2**_

-   Send EXACLY 5,000 TFC to a receive address within your wallet.

----------

_**Step 3**_

-   Create a text document to temporarily store information that you will need.

----------

_**step 4**_

-   Go to the console within the wallet

[![console](https://camo.githubusercontent.com/97d2380205574366df9657769fb27e41f7b337df/68747470733a2f2f692e696d6775722e636f6d2f32483842485a772e706e67)](https://camo.githubusercontent.com/97d2380205574366df9657769fb27e41f7b337df/68747470733a2f2f692e696d6775722e636f6d2f32483842485a772e706e67)

----------

_**Step 5**_

-   Type the commands below and press enter

`masternode genkey`

[![Masternode-genkey](https://camo.githubusercontent.com/45c98041e84032a717287b2d98a3a6b86cf24100/68747470733a2f2f692e696d6775722e636f6d2f57706c776f4a682e706e67)](https://camo.githubusercontent.com/45c98041e84032a717287b2d98a3a6b86cf24100/68747470733a2f2f692e696d6775722e636f6d2f57706c776f4a682e706e67)

`masternode outputs`

[![Masternode-outputs](https://camo.githubusercontent.com/711da3ac8f0c57f1cf46585ca6e26a9f77bf8f5b/68747470733a2f2f692e696d6775722e636f6d2f474437526f316d2e706e67)](https://camo.githubusercontent.com/711da3ac8f0c57f1cf46585ca6e26a9f77bf8f5b/68747470733a2f2f692e696d6775722e636f6d2f474437526f316d2e706e67)

----------

_**Step 6**_

-   Copy your Masternode Genkey.
-   Copy the long key (this is your transaction ID) and the 1 or 0 at the end (this is your output index)
-   Paste these into the text document you created earlier as you will need them in the next step.

----------

# [](https://github.com/Realbityoda/FreedomCoin#section-e-connecting--starting-the-masternode)Section E: Connecting & Starting the masternode

_**Step 1**_

-   Now Click on the Masternodes Tab, Click my masternodes and Click on create  [![Create](https://camo.githubusercontent.com/434d74b66b38c995febf46be10b9315e5110513e/68747470733a2f2f692e696d6775722e636f6d2f66784b4b6559702e706e67)](https://camo.githubusercontent.com/434d74b66b38c995febf46be10b9315e5110513e/68747470733a2f2f692e696d6775722e636f6d2f66784b4b6559702e706e67)

----------

_**Step 2**_

-   Fill in the form.
-   For  `Alias`  type something like "MN01"  **don't use spaces**
-   The  `Address`  is the IP and port of your server (this will be in the Bitvise terminal that you still have open).
-   The  `PrivKey`  is your masternode Gen key (This is also in the Bitvise terminal that you have open).
-   The  `TxHash`  is the transaction ID/long key that you copied to the text file.
-   The  `Output Index`  is the 0 or 1 that you copied to your text file.
-   The  `Reward Address`  You can leave Blank.
-   The  `Reward %`  You can leave this Blank.

Click "Ok"

----------

_**Step 3**_

-   Close out of the wallet and reopen Wallet *Click on the Masternodes tab "My masternodes"
-   Click update than start all in the masternodes tab

----------

_**step 4**_

-   Check the status of your masternode within the VPS by using the command below:

`Freedomcoind masternode status`

`Freedomcoind getinfo`

*You should see  _**status 9**_

If you do, congratulations! You have now setup a masternode. If you do not, please contact support and they will assist you.
