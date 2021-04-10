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

The ELK stack included with tpot is useful for analysing logs. The images of the kibana dashbaord are shown below.

![dashboard 1](https://user-images.githubusercontent.com/73482919/114270212-c9cda900-9a28-11eb-86b6-bf6f217ea1ad.png)

![dashboard 2](https://user-images.githubusercontent.com/73482919/114270219-cf2af380-9a28-11eb-98e5-33dc222cf245.png)

![dashboard 3](https://user-images.githubusercontent.com/73482919/114270229-d4883e00-9a28-11eb-87de-2243b0676a7d.png)

![dashboard 4](https://user-images.githubusercontent.com/73482919/114270235-d81bc500-9a28-11eb-87df-126ed8221be6.png)

![dashboard 5](https://user-images.githubusercontent.com/73482919/114270237-dce07900-9a28-11eb-9d7d-fbaf48b5bafe.png)

![dashboard 6 Cowrie command input](https://user-images.githubusercontent.com/73482919/114270240-e0740000-9a28-11eb-9c59-238c3cec6e81.png)


