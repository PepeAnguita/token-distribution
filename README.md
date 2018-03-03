# HashBX Token

This document gives an overview of HBXToken

# Overview

## HashBX Token

The HBX `HBXToken.sol` is ERC20-compatible and has the following additional characteristics:

1. An initial amount of 1,000,000 HBX tokens supply.
2. An ability to burn tokens by users to reduce total number of token supply to proportionally increase each token holder’s percentage in the overall token amount.

At the completion of the final token sale, HashBX plans to do the following:

- Burn all unallocated tokens

### Implementation

We use OpenZeppelin code for `SafeMath`, `Ownable`, `Burnable` and `StandardToken` logic.

* `SafeMath` provides arithmetic functions that throw exceptions when integer overflow occurs
* `Ownable` keeps track of a contract owner and permits the transfer of ownership by the current owner
* `Burnable` provides a burn function that decrements the balance of the burner and the total supply
* `StandardToken` provides an implementation of the ERC20 standard

The token contract includes the following constants:

```javascript
    name             = "HashBX";
    symbol           = "HBX";
    decimals         = 18;
    INITIAL_SUPPLY   = 1 million HBX
```

The above constants indicate a maximum supply of 1 million tokens.


Copyright 2017 HashBX Global Company Limited. All Rights Reserved.