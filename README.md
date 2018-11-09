# btc-x86-bin - Portable Bitcoin Core x86 Binaries

A collection of portable x86 binaries for Bitcoin Core

## Build Script
`build_btc_x86.sh` script can be used as follows:

### Options
You can use the following options to change these values:  
`-btcdir |--bitcoin-dir`  : set the Bitcoin source folder  
`-bindir |--binaries-dir` : set where the Bitcoin x86 binaries will be stored  
`-v= | --version`  :  used to set the release version to build  
`*` : all other options will be used for the 'configure' script

For example:  
`./build_btc_x86.sh -btcdir=../bitcoin/ -v=0.17.0 -bindir=bin/0.17.0 --without-gui`

### Defaults
Default values are:  
`btcdir='.'`  
`bindir=$btcdir/bin`  
`v=''` (using the current branch)  
