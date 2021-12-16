# XIP-2: Token Standard

## Abstract

## Specification

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

* Return type: string

### Method: TotalSupply

Returns the total token supply.

* No Parameters

* Return type: string

### Method: BalanceOf

Returns the account balance of another account with address `owner`.

* Parameters

|Offset|Name|Data Type|
|:-----|:---|:---|
|0x0000|owner|byte\[10\]|
