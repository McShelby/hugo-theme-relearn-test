---
archetype: "chapter"
title: "Leaf Bundle"
weight: 1
---

This is a "leaf bundle": Any other markdown content other than this file (`index.md`) will not be available. Thus we shouldn't see `foo` and referencing it via `ref` or `children` short code will lead to an compile time error.

{{< children showhidden="true" >}}

![This is Figure B](img/b.png)
