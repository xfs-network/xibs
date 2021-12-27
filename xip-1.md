# XIP-1: Simple Bytecode format

## Abstract

## Specification

### Code format

|Offset|Bits|Description|
|:-----|:---|:---|
|0x0000|21|Header|

### Header format

|Offset|Bits|Description|
|:-----|:---|:---|
|0x0000|16|Magic|
|0x0010|1|Type|
|0x0011|8|BuiltinId|

* Magic: Fixed constant: 9168 (Little-Endian: 0xd023)
* Type: If `type == 1` is a built-in contract, else `type = 0`
* BuiltinId: If `type = 0:  builtinId = 0`, else find specification from [Builtin IDs](#builtin-ids)

### Builtin IDs

|Name|Bytecode|Description|
|:-----|:---|:---|
|XRC2|0x01|Specification from [XIP-2](./xip-2.md)|
|XRC3|0x02|Specification from [XIP-3](./xip-3.md)|

### Built in Contract Standards

* CREATE: INPUT = CODE + CREATE_FUNC_HASH (256 bits) + FUNC_PARAMETERS
* CALL: INPUT = CALL_FUNC_HASH (256 bits) + FUNC_PARAMETERS

### Data type specification

|Type|bits|
|:---|:---|
|uint8|8|
|uint16|16|
|uint32|32|
|uint256|256|
|address|200|
|bool|1|

* string type required length + text
