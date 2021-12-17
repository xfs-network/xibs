# XIP-1: Simple Bytecode format

## Abstract

## Specification

### Code format

|Offset|Bits|Description|
|:-----|:---|:---|
|0x0000|40|Header|
|0x0028|...|Payload|

### Header format

|Offset|Bits|Description|
|:-----|:---|:---|
|0x0000|32|Magic|
|0x0020|7|Type|
|0x0027|1|Flag|

* Magic: Fixed constant: 9168 (Little-Endian: 0xd0230000)
* Type: From standard specification
* Flag: CREATE or CALL

### Types

|Type|Bytecode|Description|
|:-----|:---|:---|
|XRC2|0x01|Specification from [XIP-2](./xip-2.md)|
|XRC3|0x02|Specification from [XIP-3](./xip-3.md)|

### Built in Contract Standards

* CREATE: Payload as creation parameters
* CALL: Payload = METHOD_CODE (8 bits) + METHOD_PARAMETERS

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
