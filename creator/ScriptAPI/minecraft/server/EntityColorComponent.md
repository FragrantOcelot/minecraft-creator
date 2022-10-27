---
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server.EntityColorComponent Class
description: Contents of the @minecraft/server.EntityColorComponent class.
---
# EntityColorComponent Class
>[!IMPORTANT]
>These APIs are experimental as part of the Beta APIs experiment. As with all experiments, you may see changes in functionality in updated Minecraft versions. Check the Minecraft Changelog for details on any changes to Beta APIs. Where possible, this documentation reflects the latest updates to APIs in Minecraft beta versions.

> [!CAUTION]
> This class is still in pre-release.  Its signature may change or it may be removed in future releases.

## Extends
- [*IEntityComponent*](IEntityComponent.md)

Defines the entity's color. Only works on certain entities that have predefined color values (sheep, llama, shulker).

## Properties

### **typeId**
`read-only typeId: string;`

Identifier of this component. Should always be minecraft:color.

Type: *string*

### **value**
`value: number;`

The palette color value of the entity.

Type: *number*

## Constants

### **componentId**
`static read-only componentId = "minecraft:color";`

Identifier of this component. Should always be minecraft:color.

Type: *string*
