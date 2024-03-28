
# BEP20 Token Contract for a Stable COin. EMail me mjoechia@gmail.com for any queries

This contract defines an interface for a BEP20 token on the Binance Smart Chain (BSC).

## Interface `IBEP20`

The `IBEP20` interface includes the following methods:

- `totalSupply()`: Returns the total amount of tokens in existence.
- `decimals()`: Returns the token decimals.
- `symbol()`: Returns the token symbol.
- `name()`: Returns the token name.
- `getOwner()`: Returns the BEP token owner.
- `balanceOf(address account)`: Returns the amount of tokens owned by `account`.
- `transfer(address recipient, uint256 amount)`: Moves `amount` tokens from the caller's account to `recipient`.
- `allowance(address _owner, address spender)`: Returns the remaining number of tokens that `spender` will be allowed to spend on behalf of `_owner` through `transferFrom`.
- `approve(address spender, uint256 amount)`: Sets `amount` as the allowance of `spender` over the caller's tokens.
- `transferFrom(address sender, address recipient, uint256 amount)`: Moves `amount` tokens from `sender` to `recipient` using the allowance mechanism.

The interface also includes two events:

- `Transfer(address indexed from, address indexed to, uint256 value)`: Emitted when `value` tokens are moved from one account (`from`) to another (`to`).
- `Approval(address indexed owner, address indexed spender, uint256 value)`: Emitted when the allowance of a `spender` for an `owner` is set by a call to `approve`.

## Contract `Context`

The `Context` contract provides information about the current execution context, including the sender of the transaction and its data. This contract is meant to be used as a library or inherited by other contracts.

## Notes

This contract is written in Solidity version 0.5.16.
```
