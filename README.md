# SimpleMonero
SimpleMonero is an all-in-one BASH script for installing Monero coin mining software on Ubuntu.

How do I install SimpleMonero?
------------------------------

To install SimpleMonero, simply run these three simple lines of code on your Ubuntu server:

    wget https://raw.githubusercontent.com/vcninc/SimpleMonero/master/script
    chmod +x script
    ./script
    
SimpleMonero will then load all of the required software and start mining automatically.

What does SimpleMonero do?
--------------------------

SimpleMonero runs a series of simple commands that can turn basically any Ubuntu box into a Monero-mining machine in a matter of minutes. After making sure that your system files are up to date (via apt-get update and apt-get upgrade), SimpleMonero will install the following software (via apt-get install):

- libcurl4-openssl-dev
- libncurses5-dev
- pkg-config
- automake
- yasm
- git
- make

It then clones CPUMiner-Multi (from lucasjones/cpuminer-multi) and compiles it via make. Finally, SimpleMonero will use ./minerd to start mining Monero coins with all of the available resources.
