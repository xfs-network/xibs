# XIP-1: Simple Bytecode format

## Abstract

## Specification

### Code format

|Offset|Bits|Description|
|:-----|:---|:---|
|0x0000|24|Code|
|0x0018|...|Payload|
### Header format

|Offset|Bits|Description|
|:-----|:---|:---|
|0x0000|16|Magic|
|0x0010|8|BuiltinId|

* Magic: Fixed constant: 9168 (Little-Endian: 0xd023)
* BuiltinId: If `BuiltinId > 0` is a built-in contract, from [Builtin IDs](#builtin-ids)

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
