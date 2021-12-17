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

|Method Name|Bytecode|
|:---|:---|
|[Name](#method-name)|0x01|
|[Symbol](#method-symbol)|0x02|
|[Decimals](#method-decimals)|0x03|
|[TotalSupply](#method-totalSupply)|0x04|
|[BalanceOf](#method-balanceof)|0x05|
|[Transfer](#method-transfer)|0x06|
|[TransferFrom](#method-transferfrom)|0x07|
|[Approve](#method-approve)|0x08|
|[Allowance](#method-allowance)|0x09|

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


