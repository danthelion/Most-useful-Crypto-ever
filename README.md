# how to mine the most useful crypto ever

Create your wallet

```shell
touch ~/wallet
```

Set it to become append only so the blockchain is immutable:

```shell
chattr +a ~/wallet
```

Run the miner to produce your coins:

```shell
base64 /dev/urandom | grep -i "dingdong" >> ~/wallet
```

You have proof of stake when you hit 53 coins. Hit ^C to terminate the miner at any time, and run it again to add more coins to your wallet.

To check your wallet's contents run:

```shell
wc -l ~/wallet
```

And to verify that a wallet was truly generated by an RNG run the verifier:

```shell
cat ~/wallet | rngtest
```

Which will use the FIPS 140-2 standard to verify the wallet.
