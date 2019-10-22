# liracoin-italia
Source code of Liracoin cryptocurrency

Coin properties<br>
<ul>
  <li>Compiling OS 	Ubuntu 18.04 LTS</li>
  <li>Source branch 3.3</li>
  <li>Algorithm Quark</li>
  <li>Block type 	Proof-of-Work/Proof-of-Stake</li>
    <li>Coin name 	Liracoin</li>
    <li>Coin abbreviation 	LIT</li>
    <li>Address letter 	L</li>
    <li>Address letter testnet 	M</li>
    <li>RPC port 	11949</li>
    <li>P2P port 	11950</li>
    <li>Block reward 	50 coins</li>
    <li>Block reward (PoS) 	5 coins</li>
    <li>Last PoW block 	block 100000</li>
    <li>Superblock reward 	10%</li>
    <li>Masternode reward 	50%</li>
    <li>Masternode amount 	1000 coins</li>
    <li>Masternode confirmations 	15 blocks</li>
    <li>Coinbase maturity 	20 ( + 1 default confirmation) blocks</li>
    <li>Target spacing 	1 minutes</li>
    <li>Target timespan 	5 minutes</li>
    <li>Transaction confirmations 	3 blocks</li>
</ul>


<h3>How do I compile a daemon for Ubuntu Server 18.04 (Quark)?</h3><br>

applies to Quark<br>
branch 3.1+         <br>

<p>Updated August 1, 2019, </p>

<p>Use the following instructions to compile a daemon and GUI wallet for Ubuntu Server 18.04.</p>

<p>
<b>Update your Ubuntu machine.</b><br>
sudo apt-get update<br>
sudo apt-get upgrade<br>
</p>

<p>
<b>Install the required dependencies.</b><br>
sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl1.0-dev libevent-dev bsdmainutils python3 libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-test-dev libboost-thread-dev libboost-all-dev libboost-program-options-dev<br><br>
sudo apt-get install libminiupnpc-dev libzmq3-dev libqt5gui5 libqt5core5a libqt5dbus5 qttools5-dev qttools5-dev-tools libprotobuf-dev protobuf-compiler libqrencode-dev unzip libgmp3-dev<br>
</p>
<p><b>
Install Berkeley DB.</b><br>
sudo add-apt-repository ppa:bitcoin/bitcoin<br>
sudo apt-get update<br>
sudo apt-get install libdb4.8-dev libdb4.8++-dev<br>
</p>

<p><b>
Create a directory for the source code.</b><br>
cd ~/<br>
mkdir source_code<br>
cd source_code<br>
</p>

<p><b>
Download the source code</b> <br>
wget https://github.com/gammatecnology/liracoin-italia.git<br>
</p>

<p>
Execute the following commands to start compiling.
./autogen.sh
./configure --with-incompatible-bdb
make
</p>

<p>The compiling will take about 60 minutes depending on your system hardware.</p>

<p>
Your compiled GUI wallet named liracoin-qt can be found in the folder “src/qt” when compiling is finished.
Client tools liracoin-cl, liracoin-tx and the daemon liracoind can be found in the folder “src” when compiling is finished.
</p>

<br><br>
Support and other information to liracoin website: https://www.liracoin.it

