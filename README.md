# btc-x86-bin

Portable x86 binaries for Bitcoin Core

## Build Script
build_btc_x86.sh script can be used as follows:

Default values are:
Bitcoin Directory: '.'
Binaries Directory: $BitcoinDirectory/bin
Branch: master

You can use the following options to change these values:
-btcdir |--bitcoin-dir  : set the Bitcoin source folder
-bindir |--binaries-dir : set where the Bitcoin x86 binaries will be stored
-v= | --version  :  used to set the release version to build
* : all other options will be used for the 'configure' script

For example:
`./build_btc_x86.sh -btcdir=../bitcoin/ -v=0.17.0 -bindir=bin/0.17.0 --without-gui`
