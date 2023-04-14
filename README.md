# Markr Assets - Tokens

To add your assets please follow steps described below:

# Tokens (ERC20)
1. Always add your token to the bottom of the list.
2. Token address must be converted into lowercase.
3. Find unique `identifier`. Search the project before select an identifier. If you deployed same token more than 1 chain. Please use same identifier for the other chains.
4. `created_at` refers deployed block of the asset.
5. If it's a bridged asset please set `bridged` to true. And provide bridge name with `bridge` field.
6. If it's not a bridget asset please set `native`to true.
7. Do not fill `median`, `stable`, `wrapped_native_currency` and `main_stable` fields. Otherwise your PR will be rejected.

# Example Asset

```
{
    "identifier": "usd-coin",
    "address": "0xa7d7079b0fead91f3e65f86e8915cb59c1a4c664",
    "name": "USD Coin",
    "symbol": "USDC.e",
    "decimals": 6,
    "bridge": "AB",
    "created_at": 3311254
}
```