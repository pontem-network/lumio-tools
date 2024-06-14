# Lumio-сli

The Lumio CLI tool provides a convenient way to interact with Lumio blockchain

## Getting Started

* Download the latest version of the utility from the following link [LumioCli](https://github.com/pontem-network/lumio-tools/releases)
* Unpack the archive
* Add the path to the lumio-cli binary to the PATH environment variable

## Deposit

The deposit command allows you to transfer sol coins from L1 to L2.

How to use:

```bash
./lumio-cli deposit-sol 100
```

By default, the deposit command use solana config ("~/.config/solana/cli/config.yml") as a configuration file.
You can specify a different configuration file using the `--config` flag for the override the default solana config.

By default, the deposit command transfer coins to the address of the current account in the solana config to the same address on the lumio l2.
You can specify a different address using the `--to` flag.

```bash
./lumio-cli deposit-sol 100 --to F7J6FsZivaRRyGpLWhTo3yc75R7Lid8xWH6we4LSqh4r
```

