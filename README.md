# Rover
Shell script to install a [Rover Coin Masternode](http://rovercoin.io/) on a Linux server running Ubuntu 16.04. Use it on your own risk.
***

## Installation
```
wget -q https://raw.githubusercontent.com/zoldur/RoverCoin/master/rover_install.sh  
bash rover_install.sh
```
***

## Desktop wallet setup

After the MN is up and running, you need to configure the desktop wallet accordingly. Here are the steps:  
1. Open the Rover Desktop Wallet.  
2. Go to RECEIVE and create a New Address: **MN1**  
3. Send **10000** ROE to **MN1**.  
4. Wait for 15 confirmations.  
5. Go to **Help -> "Debug Window - Console"**  
6. Type the following command: **masternode outputs**  
7. Go to **Masternodes** tab  
8. Click **Create** and fill the details:  
* Alias: **MN1**  
* Address: **VPS_IP:PORT**  
* Privkey: **Masternode Private Key**  
* TxHash: **First value from Step 6**  
* Output index:  **Second value from Step 6**  
* Reward address: leave blank  
* Reward %: leave blank  
9. Click **OK** to add the masternode  
10. Click **Start All**  
***

## Usage:
```
Roverd masternode status  
Roverd getinfo
```
Also, if you want to check/start/stop **Rover**, run one of the following commands as **root**:

```
systemctl status Rover #To check if Rover service is running  
systemctl start Rover #To start Rover service  
systemctl stop Rover #To stop Rover service  
systemctl is-enabled Rover #To check if Rover service is enabled on boot  
```  
***

## Donations

Any donation is highly appreciated  

  
**BTC**: 3MQLEcHXVvxpmwbB811qiC1c6g21ZKa7Jh  
**ETH**: 0x26B9dDa0616FE0759273D651e77Fe7dd7751E01E  
**LTC**: LNZpK4rCd1JVSB3rGKTAnTkudV9So9zexB

