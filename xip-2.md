# XIP-2: Token Standard

## Abstract

## Specification

### Methods

|Method Name|Bytecode|
|:---|:---|
|Name|0x01|
|Symbol|0x02|
|Decimals|0x03|
|TotalSupply|0x04|
|BalanceOf|0x05|
|Transfer|0x06|
|TransferFrom|0x07|
|Approve|0x08|
|Allowance|0x09|

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
