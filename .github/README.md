# Datacenter Node Home Directory Skeleton
This repository contains a base directory structure and associated shell scripts for the `solana` user on Solana's devnet/testnet-bound infrastructure.  What lives here should be kept to a minimum.  Instead prefer client-side logic in the scripts in the [`net` directory](https://github.com/solana-labs/solana/tree/master/net) of the solana repository.

## Usage
If the `solana` user's home directory is empty
```
$ git clone https://github.com/solana-labs/dc-homedir-skeleton.git .
```
Otherwise it's a little more involved
```
$ git init
$ git remote add origin https://github.com/solana-labs/dc-homedir-skeleton.git
$ git fetch
$ git reset --hard origin/master   # XXX: Any changes to tracked files will be lost!
$ git clean -xdff                  # XXX: Any untracked files will be removed!
```
