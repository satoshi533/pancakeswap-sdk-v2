# Pancakeswap SDK

[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
[![Actions Status](https://github.com/pancakeswap/pancakeswap-sdk/workflows/CI/badge.svg)](https://github.com/pancakeswap/pancakeswap-sdk)
[![npm version](https://img.shields.io/npm/v/@pancakeswap-lib/sdk/latest.svg)](https://www.npmjs.com/package/@pancakeswap-lib/sdk/v/latest)

## V2 SDK for the BSC testnet

This is a fork of `@pancakeswap-libs/sdk-v2` modified to work on the BSC testnet against PancakeSwap V2 routers coupled with [`pancake-swap-interface-v1`](https://github.com/pancakeswap/pancake-swap-interface-v1).

Detailed instructions and the modified `pancake-swap-interface-v1` code can be found at [https://github.com/ibhagwan/pancake-swap-interface-v1](https://github.com/ibhagwan/pancake-swap-interface-v1).

### Building this SDK

Clone either this repository or the official one:
```
❯ git clone https://github.com/ibhagwan/pancakeswap-sdk-v2
```

- Modify `FACTORY_ADDRESS` & `INIT_CODE_HASH` in `src/constants.ts`
- Modify the testnet `WBNB` at the end of `entities/token.ts`:
    ```
    [ChainId.BSCTESTNET]: new Token(
        ChainId.BSCTESTNET,
        '0xae13d989dac2f0debff460ac112a837c89baa7cd',
        18,
        'WBNB',
        'Wrapped BNB'
    )
    ```

Build:
```
❯ yarn
❯ npm run build
```

### PancaeSwap V2, option #1 (default)
Router: [`0xD99D1c33F9fC3444f8101754aBC46c52416550D1`](https://testnet.bscscan.com/address/0xD99D1c33F9fC3444f8101754aBC46c52416550D1)

Factory: [`0x6725f303b657a9451d8ba641348b6761a6cc7a17`](https://testnet.bscscan.com/address/0x6725f303b657a9451d8ba641348b6761a6cc7a17)

WETH: [`0xae13d989dac2f0debff460ac112a837c89baa7cd`](https://testnet.bscscan.com/address/0xae13d989dac2f0debff460ac112a837c89baa7cd)

INIT_CODE_PAIR_HASH: `0xd0d4c4cd0848c93cb4fd1f498d7013ee6bfb25783ea21593d5834f5d250ece66`


### PancaeSwap V2, option #2
Router: [`0x9Ac64Cc6e4415144C455BD8E4837Fea55603e5c3`](https://testnet.bscscan.com/address/0x9Ac64Cc6e4415144C455BD8E4837Fea55603e5c3)

Factory: [`0xb7926c0430afb07aa7defde6da862ae0bde767bc`](https://testnet.bscscan.com/address/0xb7926c0430afb07aa7defde6da862ae0bde767bc)

WETH: [`0xae13d989dac2f0debff460ac112a837c89baa7cd`](https://testnet.bscscan.com/address/0xae13d989dac2f0debff460ac112a837c89baa7cd)

INIT_CODE_PAIR_HASH: `0xecba335299a6693cb2ebc4782e74669b84290b6378ea3a3873c7231a8d7d1074`



