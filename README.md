# Arrakis Token List

Full list of Tokens used in Arrakis Vaults [App](https://github.com/ArrakisFinance/polygon-staking-ui)


## Adding new Token to List
1. Add an entry in the `tokens` field of the list. Please use the [checksum address](https://docs.ethers.io/v5/api/utils/address/#address). Here is an example of GEL Token:
    ```json
    {
      "chainId": 1,
      "address": "0x15b7c0c907e4C6b9AdaAaabC300C08991D6CEA05",
      "decimals": 18,
      "name": "Gelato Network Token",
      "symbol": "GEL",
      "logoURI": "https://raw.githubusercontent.com/ArrakisFinance/arrakis-tokenlist/main/images/0x15b7c0c907e4C6b9AdaAaabC300C08991D6CEA05-1.svg"
    }
    ```
2. Update the `timestamp` field to the current timestamp.
3. Update the `version` field to adhere to semantic versioning:
    * Increment major version when tokens are removed
    * Increment minor version when tokens are added
    * Increment patch version when tokens already on the list have minor details changed (name, symbol, logo URL, decimals)
  
	**Note:** Changing a token address or chain ID is considered both a remove and an add, and should be a major version update.
4. Add the token logo image to the `images/` folder.
