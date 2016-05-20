---
title: Array.length<'T> Function (F#)
description: Array.length<'T> Function (F#)
keywords: visual f#, f#, functional programming
author: dend
manager: danielfe
ms.date: 05/16/2016
ms.topic: language-reference
ms.prod: visual-studio-dev14
ms.assetid: 760ca92f-46d4-44f9-aa5b-caab442d3f51 
---

# Array.length<'T> Function (F#)

Returns the length of an array.

**Namespace/Module Path:** Microsoft.FSharp.Collections.Array

**Assembly:** FSharp.Core (in FSharp.Core.dll)

## Syntax

```
// Signature:
Array.length : 'T [] -> int

// Usage:
Array.length array
```

#### Parameters

*array*
Type: **'T**[[]](http://msdn.microsoft.com/en-us/library/def20292-9aae-4596-9275-b94e594f8493)

The input array.

**Returns the length of the array.**

## Remarks

You can also use the property **System.Array.Length**.

This function is named **Length** in compiled assemblies. If you are accessing the function from a language other than F#, or through reflection, use this name.

**The following code example demonstrates how to use Array.length.**
[!code-fsharp[Main](snippets/fsarrays/snippet50.fs)]

**Output**

```
Length: 100
Length: 0
Length: 50
```

## Platforms

Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2

## Version Information

**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable

## See Also

[Collections.Array Module &#40;F&#35;&#41;](Collections.Array-Module-%5BFSharp%5D.md)

[Microsoft.FSharp.Collections Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Collections-Namespace-%5BFSharp%5D.md)

