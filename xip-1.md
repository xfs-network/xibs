# XIP-1: Simple Bytescode format

## Abstract

## Specification

## Code format

|Offset|Bits|Description|
|:-----|:---|:---|
|0x0000|40|Header|
|0x0028|...|Payload|

## Header format

|Offset|Bits|Description|
|:-----|:---|:---|
|0x0000|32|Magic|
|0x0020|8|Type|
