# Tpot-Data-analysis
T-Pot, an open source honeypot, was deployed in a cloud environment to collect data points, which were then logged. These logs were useful for determining the attackers intentions by analyzing the top attacking countries, IPs, and attack motives based on attack signatures and categories.

The prerequisite required to install T-Pot on AWS EC2 instance are:
1. Tpot installation requires Debian (GNU/Linux 9 (Stretch))
2. Ubuntu server 16.04 does not support debian packages
3. Needs 4 - 6 CPUs (AWS) i.e. 16 GB RAM
4. Web portal access on https://AWSpublicIP:64297 - The port 64297 is accessible to the source “myipaddress” to access the kibana dashboard for data visualization

T-Pot Installation type selected was "standard"

The steps required to install T-Pot honeypot are as follows:
1. sudo apt-get update
2. sudo apt-get upgrade
3. sudo apt install git –y (to get the required repository)
4. git clone https://github.com/dtag-dev-sec/tpotce
5. cd tpotce
6. sudo ./install.sh --type=user (This will start the installation and might take 10 to 15 minutes)
7. Install type used is “T-Pot’s standard installation”

To see the Logs from terminal (‘sudo su’ for root user) - The Tpot logs are stored in ‘data’ folder of respective honeypots
