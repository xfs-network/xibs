# XIP-2: Token Standard

## Abstract

## Specification

### Create

|Parameter Name|Data Type|
|:---|:---|
|Name|string|
|Symbol|string|
|Decimals|uint8|
|TotalSupply|uint256|

### Methods

|Method Name|
|:---|
|[Name](#method-name)|
|[Symbol](#method-symbol)|
|[Decimals](#method-decimals)|
|[TotalSupply](#method-totalSupply)|
|[BalanceOf](#method-balanceof)|
|[Transfer](#method-transfer)|
|[TransferFrom](#method-transferfrom)|
|[Approve](#method-approve)|
|[Allowance](#method-allowance)|

### Method: Name

Returns the name of the token - e.g. "MyToken".

* No Parameters

* Return type: string

### Method: Symbol

Returns the symbol of the token. E.g. “HIX”.

* No Parameters

* Return type: string

### Method: Decimals

Returns the number of decimals the token uses - e.g. 8, means to divide the token amount by 100000000 to get its user representation.

* No Parameters

* Return type: uint8

### Method: TotalSupply

Returns the total token supply.

* No Parameters

* Return type: uint256

### Method: BalanceOf

Returns the account balance of another account with address `owner`.

* Parameters

|Name|Data Type|
|:---|:---|
|owner|address|

* Return type: uint256

### Method: Transfer

Transfers `value` amount of tokens to address `to`

* Parameters

|Name|Data Type|
|:---|:---|
|to|address|
|value|uint256|

* Return type: bool

### Method: TransferFrom

Transfers `value` amount of tokens from address `from` to address `to`

* Parameters

|Name|Data Type|
|:---|:---|
|from|address|
|to|address|
|value|uint256|

* Return type: bool


### Method: Approve

Allows `spender` to withdraw from your account multiple times, up to the `value` amount.
If this function is called again it overwrites the current allowance with `value`.

* Parameters

|Name|Data Type|
|:---|:---|
|spender|address|
|value|uint256|

* Return type: bool

### Method: Allowance

Returns the amount which `spender` is still allowed to withdraw from `owner`.

* Parameters

|Name|Data Type|
|:---|:---|
|owner|address|
|spender|address|

* Return type: uint256


