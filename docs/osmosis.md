## Osmosis

create validator

```bash
osmosisd tx staking create-validator \
    --amount=1000000uosmo \
    --commission-rate="0.05" \
    --commission-max-rate="0.1" \
    --commission-max-change-rate="0.01" \
    --min-self-delegation="1" \
    --pubkey=$(osmosisd tendermint show-validator) \
    --moniker="Polkachu" \
    --website "https://polkachu.com" \
    --identity "0A6AF02D1557E5B4" \
    --details "Polkachu is the trusted staking service provider for blockchain projects. 100% refund for downtime slash. Contact us at hello@polkachu.com" \
    --chain-id=osmosis-1 \
    --gas="auto" \
    --gas-adjustment="1.2" \
    --gas-prices="0.025uosmo" \
    --from=polkachu
```

Edit validator

```bash
osmosisd tx staking edit-validator \
    --moniker "polkachu.com" \
    --website "https://polkachu.com" \
    --chain-id=osmosis-1 \
    --gas="auto" \
    --gas-adjustment="1.2" \
    --gas-prices="0.025uosmo" \
    --from=polkachu
```
