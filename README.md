# downloads

Decentralbank.com and dcentralcoin (DCC):<br>
Decentralization is the process of redistributing or dispersing functions, powers, people or things away from a central location or authority. By definition, it is to move power away from a central authority, like a bank or government. Decentralization means that no single organization or entity has absolute power over a certain aspect of society.<br>
Dcentralbank has all the elements that are necessary to make a functional, decentralized banking system. With the rise of the internet, this is especially relevant. Be your own bank. A decentralized system doesn’t only bring the benefit of not having to trust a central bank to do the job, but you also get to avoid unnecessary fees. Because you are dealing with other people within the decentralized system, instead of going through a middleman. Dcentralcoin offers total payment confidentiality, maintaining a decentralised network using a public blockchain.<br>

Getting started<br>
Use the following instructions to mine a block.<br>
Open your wallet, and make sure your wallet is connected with a node. <br>
Your wallet is connected when you see the icon in the lower right corner of your wallet.<br>
The message “Syncing Headers (0,0%)” will disappear once you mine your first block.<br>
Close your wallet and create the file dcentralcoin.conf in the folder “%APPDATA%\dcentralcoin\”.<br>
 Paste the following text into dcentralcoin.conf and save the file.<br>
 rpcuser=rpc_dcentralcoin<br>
 rpcpassword=password<br>
 rpcallowip=127.0.0.1<br>
 rpcport=4887<br>
 listen=1<br>
 server=1<br>
 addnode=136.144.171.201<br>
Open your wallet.<br>
Create a .bat file named mine.bat in the same folder where you extracted dcentralcoin-cli.exe and paste the following text into mine.bat.<br>
@echo off<br>
set SCRIPT_PATH=%cd%<br>
cd %SCRIPT_PATH%<br>
echo Press [CTRL+C] to stop mining.<br> 
:begin<br>
 dcentralcoin-cli.exe generate 1<br>
goto begin <br>
Save the file.<br>
Execute mine.bat to start mining your first block.<br>
It will take about +/- 30 minutes to mine your first block, depending on your computer hardware.<br>
