# KYC-gated Token

-   [`KYCToken.sol`](src/KYCToken.sol): ERC20 with KYC checks for mint, burn and transfer. Deployed at `0x298dd16AC0C45827C004032c56864B98C9764572` on **Ethereum Goerli Testnet**
-   [`KYCToken.t.sol`](test/KYCToken.t.sol): Fuzzing unit tests for the KYCToken contract

## Tests

Install Foundry from [here.](https://book.getfoundry.sh/getting-started/installation)
Run tests in the root directory with `forge test`

## Monitor token events

-   You need an API key to access a Node RPC endpoint. Get one for Ethereum Goerli at https://www.alchemy.com/.
-   Create a text file `.env` in the root dir and add your complete URL like so

```bash
# .env file
ETH_GOERLI=<Your RPC URL>
```

-   Then, install dependencies and run the monitor script.

```bash
# Using Python 3.10
pip install -r requirements.txt
python monitor.py
```
