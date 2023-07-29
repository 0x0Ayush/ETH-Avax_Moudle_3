# Panda (PND) Smart Contract

Panda (PND) is an ERC20 token smart contract deployed on the Ethereum Testnet blockchain. It allows the contract owner to mint new tokens, users to transfer tokens, and users to burn tokens.

## Token Details

- Name: Panda
- Symbol: PND
- Decimals: 18
- Initial Supply: 1,000,000 PND

## Functions

### Minting Tokens

Only the contract owner can mint new tokens. To mint tokens, use the `mint` function.

#### mint Function 

```solidity
function mint(address to, uint256 amount) public onlyOwner
```
# Transferring Tokens

Any user can transfer tokens to another address using the standard ERC20 ```transfer``` function.

```solidity
function transfer(address to, uint256 amount) public override returns (bool)
```
# Burning Tokens

Any user can burn their own tokens using the ```burn``` function.

```solidity
function burn(uint256 amount) public
```


