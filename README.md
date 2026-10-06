# plimsoll-protocol.github.io

The organisation site for [Plimsoll](https://github.com/plimsoll-protocol).

- `/` redirects to the app at `/plimsoll-app/`.
- `/.well-known/stellar.toml` is the [SEP-1](https://github.com/stellar/stellar-protocol/blob/master/ecosystem/sep-0001.md)
  file for the **testnet demo issuer** of PUSD
  (`GBIE3ANCRVCBWETUZXWYKRMP27LQVJHX757XXAQUT3LYHVTNFPPPXEY4`), whose
  `home_domain` is set to `plimsoll-protocol.github.io`. Its
  `attestation_of_reserve` points at the demo reserve statement, so the full
  SEP-1 loop can be seen on testnet: issuer account → home domain →
  stellar.toml → attestation document → on-chain hash.

`.nojekyll` is required: Jekyll would otherwise skip the `.well-known` folder.
