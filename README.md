# ERC20 Smart contract updated to be compiled with the newest version of Solidity.
## Code ported solidity version 0.4.24
## Code updated by CryptoLuigi

### Code Ported from:
```
https://github.com/bitfwdcommunity/Issue-your-own-ERC20-token
```

In order to alter the code to suit you token issuing needs.
Altering the contructor with the parameters
```
    constructor() public {
        symbol = "LUIGI";
        name = "LUIGI Token";
        decimals = 6;
        _totalSupply = 21000000000000;
        balances[0x5ec911DAc0D978Ebf547717B778eaaADf61E4746] = _totalSupply;
        emit Transfer(address(0), 0x5ec911DAc0D978Ebf547717B778eaaADf61E4746, _totalSupply);
    }
    
```
The key parameters to change are symbol, name, decimal, total supply and ethereum address.

## Working implementation of this ERC20
```
https://etherscan.io/token/0xb22d06e956b5010efdb7774c7e7c3cd04b282341
```
