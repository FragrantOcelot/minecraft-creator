---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: fill Command
description: Description and usage of the fill command
---
# `/fill` Command
Fills all or parts of a region with a specific block.

<table>
  <tr>
    <th>Permission Level</th>
    <td>Game Directors</td>
  </tr>
  <tr>
    <th>Requires Cheats?</th>
    <td>Yes</td>
  </tr>
</table>

## Usage
### Fill with optional fill mode
`/fill <from: x y z> <to: x y z> <tileName: Block> [tileData: int] [oldBlockHandling: FillMode]`

Fill a region `from` one position `to` another of a particular `block name`, `block id`, with an optional `fill mode`.

### Fill with replacement block name or block ID
`/fill <from: x y z> <to: x y z> <tileName: Block> <tileData: int> replace [replaceTileName: Block] [replaceDataValue: int]`

Fill a region `from` one position `to` another of a particular `block name` or `block id` with a replacement `block name` or `block id`.

### Fill with block state, optional fill mode
`/fill <from: x y z> <to: x y z> <tileName: Block> [blockStates: block properties] [oldBlockHandling: FillMode]`

Fill a region `from` one position `to` another of a particular `block state` with an optional fill mode.

### Fill, filter on block states, optional replace with tile name or block state
`/fill <from: x y z> <to: x y z> <tileName: Block> <blockStates: block properties> replace [replaceTileName: Block] [replaceBlockStates: block properties]`

Fill a region `from` one position `to` another of a particular `block name`, filtering on particular `block states`, and replacing with blocks using an optional `replacement tile name` and optional `replacement block states`.

## Arguments
- `blockStates`: block properties
An array of block states.
- `from: x y z`: position
A vector that specifies the location in `x`, `y`, and `z` coordinates of `float` type.
- `oldBlockHandling`: FillMode
Old block handling fill mode
- `replaceBlockStates`: block properties
An `array` of block states to replace.
- `replaceDataValue`: int
An `integer` that specifies the block `id` to filter for when filling.
- `replaceTileName`: [Block](../enums/Block.md)
An `enum` of the type of the block `id` to replace in the fill region.
- `tileData`: int
An `integer` that represents the block `id` to use for the fill command.
- `tileName`: [Block](../enums/Block.md)
An `enum` of the block `id` of the block to fill the region with.
- `to: x y z`: position
A `vector` that specifies the location in `x`, `y`, and `z` coordinates of `float` type.

## Enums
### `FillMode`
An `enum` of type `destroy`, `hollow`, `keep`, `outline`, or `replace`.
`destroy` replaces all blocks in the fill region and removes existing blocks.
`hollow` replaces only the block on the outer edge with the specified block.
`keep` replaces only the air blocks in the fill version.
`outline` replaces only inner blocks on the outer edge with the specified block.
`replace` replaces all blocks in teh fill region with the specified block without dropping blocks.

#### Values
- `destroy`
`destroy` replaces all blocks in the fill region and removes existing blocks
- `hollow`
`hollow` replaces only the block on the outer edge with the specified block
- `keep`
`keep` replaces only the air blocks in the fill version
- `outline`
`outline` replaces only inner blocks on the outer edge with the specified block