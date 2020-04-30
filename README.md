# btc-x86-bin - Portable Bitcoin Core x86 Binaries

A collection of portable x86 binaries for Bitcoin Core

## Build Script
`build_btc_x86.sh` script can be used as follows:

`./build_btc_x86.sh [-R] [-btcdir=BITCOIN_SRC_DIR] [-v=BTC_VERSION] -[bindir=OUTPUT_BINARY_DIR] [BUILD_OPTIONS]`

### Options
You can use the following options to change these values:  
`-btcdir |--bitcoin-dir`  : set the Bitcoin source folder  
`-bindir |--binaries-dir` : set where the Bitcoin x86 binaries will be stored  
`-v= | --version` : to set the release version to build  
`-R= | --requirements`  : install requirements (only works for Ubuntu)  
`*` : all other options will be used for the 'configure' script  

For example:  
`./build_btc_x86.sh -R -btcdir=../bitcoin/ -v=0.17.0 -bindir=bin/0.17.0 --without-gui`

### Defaults
Default values are:  
`btcdir='.'`  
`bindir=$btcdir/bin`  
`v=''` (using the current branch)  

### Note
If version is specified, a subfolder with the same name will be created inside the `bindir`  
E.g.: `./build_btc_x86.sh -v=0.17.0 -bindir=mybin` will save binaries in the path `./mybin/0.17.0`
