---
title: Array.foldBack<'T,'State> Function (F#)
description: Array.foldBack<'T,'State> Function (F#)
keywords: visual f#, f#, functional programming
author: dend
manager: danielfe
ms.date: 05/16/2016
ms.topic: language-reference
ms.prod: visual-studio-dev14
ms.technology: devlang-fsharp
ms.assetid: 67f07981-c84a-4ca1-b2aa-04367472e5c9 
---

# Array.foldBack<'T,'State> Function (F#)

Applies a function to each element of the array, threading an accumulator argument through the computation. If the input function is **f** and the elements are **i0...iN** then computes **f i0 (...(f iN s))**.

**Namespace/Module Path:** Microsoft.FSharp.Collections.Array

**Assembly:** FSharp.Core (in FSharp.Core.dll)

## Syntax

```fsharp
// Signature:
Array.foldBack : ('T -> 'State -> 'State) -> 'T [] -> 'State -> 'State

// Usage:
Array.foldBack folder array state
```

#### Parameters
*folder*
Type: **'T -&gt; 'State -&gt; 'State**

The function to update the state given the input elements.

*array*
Type: **'T**[[]](https://msdn.microsoft.com/library/def20292-9aae-4596-9275-b94e594f8493)

The input array.

*state*
Type: **'State**

The initial state.

## Exceptions

|Exception|Condition|
|----|----|
|[ArgumentNullException](https://msdn.microsoft.com/library/system.argumentnullexception.aspx)|Thrown when the input array is null.|

## Return Value

The final state.

## Remarks
This function is named `FoldBack` in compiled assemblies. If you are accessing the function from a .NET language other than F#, or through reflection, use this name.

## Example

[!code-fsharp[Main](snippets/fsarrays/snippet76.fs)]

**Output**

```
6
5
5
-5
5
```

## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2

## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable

## See Also
[Collections.Array Module &#40;F&#35;&#41;](Collections.Array-Module-%5BFSharp%5D.md)

[Microsoft.FSharp.Collections Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Collections-Namespace-%5BFSharp%5D.md)

