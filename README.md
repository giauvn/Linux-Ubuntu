# Linux-Ubuntu update
- sudo apt update
- sudo apt upgrade
# Install library
- sudo apt install -y wget git proot automake autoconf pkg-config libcurl4-openssl-dev libjansson-dev libssl-dev libgmp-dev zlib1g-dev make g++ build-essential yasm libboost-all-dev libdb++-dev dos2unix unzip
# Install and user NVTOP with GPU NVIDIA
- sudo apt install nvtop
- (Run)
- Nvtop
- (or)
- nvidia-smi
- (or)
- nvidia-smi -h

# 4 Useful Tools to Monitor CPU and GPU Temperature in Ubuntu
### lm-sensors
### Psensor
### Gnome System Monitor
### Conky
### Hardinfo
- sudo apt-get install hardinfo
- launch it from applications menu
- view your CPU and GPU temperature, click on "Sensors" tab in Hardinfo window.
- Htop
- sudo apt-get install htop
- run
- htop
- press "F2" key to open setup menu
- then navigate to "Columns" section and select "CPU temp" and/or "GPU temp".
    

# Install cpuminer 2.4
- sudo wget http://sourceforge.net/projects/cpuminer/files/pooler-cpuminer-2.4.tar.gz
- tar xzf pooler-cpuminer-2.4.tar.gz
- cd cpuminer-2.4
- ./configure CFLAGS="-O3 "
- make
#### Run cpuminer2.4
- sudo ./minerd -o stratum+tcp://litecoinpool.org:3333 -u giauvn.5 -p 1 -a scrypt
##### Noted :
- -u = wallet.username
- -p = pass
- App can run in background, if you want to quit press CTRL + c

# Install cpuminer-multi
- sudo git clone https://github.com/tpruvot/cpuminer-multi
- cd cpuminer-multi
- sudo ./build.sh
#### Run cpuminer-multi
- sudo ./cpuminer -o stratum+tcp://litecoinpool.org:3333 -u giauvn.5 -p 1 -a scrypt
#### Noted :
- -u = wallet.username
- -p = pass
- App can run in background, if you want to quit press CTRL + c
