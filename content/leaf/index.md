---
archetype: "chapter"
title: "Leaf Bundle"
weight: 1
---

This is a "leaf bundle": Any other markdown content other than this file (`index.md`) will not be available. Thus we shouldn't see `singlel` and referencing it via `ref` or `children` short code will lead to an compile time error.

{{< resources >}}

#### Page Relative

![Figure H](../h.png "H")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | nok    |
| md hugo      | print        | `true`   | ok     |
| md hugo      | html         | `false`  | ok     |
| md hugo      | print        | `false`  | ok     |
| md theme old | html         | `true`   | nok    |
| md theme old | print        | `true`   | ok     |
| md theme old | html         | `false`  | ok     |
| md theme old | print        | `false`  | ok     |
| md theme jmo | html         | `true`   | nok    |
| md theme jmo | print        | `true`   | ok     |
| md theme jmo | html         | `false`  | ok     |
| md theme jmo | print        | `false`  | ok     |

![Figure HI](../img/hi.png "HI")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | nok    |
| md hugo      | print        | `true`   | ok     |
| md hugo      | html         | `false`  | ok     |
| md hugo      | print        | `false`  | ok     |
| md theme old | html         | `true`   | nok    |
| md theme old | print        | `true`   | ok     |
| md theme old | html         | `false`  | ok     |
| md theme old | print        | `false`  | ok     |
| md theme jmo | html         | `true`   | nok    |
| md theme jmo | print        | `true`   | ok     |
| md theme jmo | html         | `false`  | ok     |
| md theme jmo | print        | `false`  | ok     |

![Figure B](../branch/b.png "B")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | nok    |
| md hugo      | print        | `true`   | ok     |
| md hugo      | html         | `false`  | ok     |
| md hugo      | print        | `false`  | ok     |
| md theme old | html         | `true`   | nok    |
| md theme old | print        | `true`   | ok     |
| md theme old | html         | `false`  | ok     |
| md theme old | print        | `false`  | ok     |
| md theme jmo | html         | `true`   | nok    |
| md theme jmo | print        | `true`   | ok     |
| md theme jmo | html         | `false`  | ok     |
| md theme jmo | print        | `false`  | ok     |

![Figure BI](../branch/img/bi.png "BI")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | nok    |
| md hugo      | print        | `true`   | ok     |
| md hugo      | html         | `false`  | ok     |
| md hugo      | print        | `false`  | ok     |
| md theme old | html         | `true`   | nok    |
| md theme old | print        | `true`   | ok     |
| md theme old | html         | `false`  | ok     |
| md theme old | print        | `false`  | ok     |
| md theme jmo | html         | `true`   | nok    |
| md theme jmo | print        | `true`   | ok     |
| md theme jmo | html         | `false`  | ok     |
| md theme jmo | print        | `false`  | ok     |

![Figure L](l.png "L")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | nok    |
| md hugo      | print        | `true`   | nok    |
| md hugo      | html         | `false`  | ok     |
| md hugo      | print        | `false`  | ok     |
| md theme old | html         | `true`   | ok     |
| md theme old | print        | `true`   | ok     |
| md theme old | html         | `false`  | ok     |
| md theme old | print        | `false`  | ok     |
| md theme jmo | html         | `true`   | ok     |
| md theme jmo | print        | `true`   | ok     |
| md theme jmo | html         | `false`  | ok     |
| md theme jmo | print        | `false`  | ok     |

![FigureL LI](img/li.png "LI")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | nok    |
| md hugo      | print        | `true`   | nok    |
| md hugo      | html         | `false`  | ok     |
| md hugo      | print        | `false`  | ok     |
| md theme old | html         | `true`   | ok     |
| md theme old | print        | `true`   | ok     |
| md theme old | html         | `false`  | ok     |
| md theme old | print        | `false`  | ok     |
| md theme jmo | html         | `true`   | ok     |
| md theme jmo | print        | `true`   | ok     |
| md theme jmo | html         | `false`  | ok     |
| md theme jmo | print        | `false`  | ok     |

#### Project Relative

![Figure H](/h.png "H")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | ok     |
| md hugo      | print        | `true`   | ok     |
| md hugo      | html         | `false`  | ok     |
| md hugo      | print        | `false`  | ok     |
| md theme old | html         | `true`   | ok     |
| md theme old | print        | `true`   | ok     |
| md theme old | html         | `false`  | ok     |
| md theme old | print        | `false`  | ok     |
| md theme jmo | html         | `true`   | ok     |
| md theme jmo | print        | `true`   | ok     |
| md theme jmo | html         | `false`  | ok     |
| md theme jmo | print        | `false`  | ok     |

![Figure HI](/img/hi.png "HI")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | ok     |
| md hugo      | print        | `true`   | ok     |
| md hugo      | html         | `false`  | ok     |
| md hugo      | print        | `false`  | ok     |
| md theme old | html         | `true`   | ok     |
| md theme old | print        | `true`   | ok     |
| md theme old | html         | `false`  | ok     |
| md theme old | print        | `false`  | ok     |
| md theme jmo | html         | `true`   | ok     |
| md theme jmo | print        | `true`   | ok     |
| md theme jmo | html         | `false`  | ok     |
| md theme jmo | print        | `false`  | ok     |

![Figure B](/branch/b.png "B")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | ok     |
| md hugo      | print        | `true`   | ok     |
| md hugo      | html         | `false`  | ok     |
| md hugo      | print        | `false`  | ok     |
| md theme old | html         | `true`   | ok     |
| md theme old | print        | `true`   | ok     |
| md theme old | html         | `false`  | ok     |
| md theme old | print        | `false`  | ok     |
| md theme jmo | html         | `true`   | ok     |
| md theme jmo | print        | `true`   | ok     |
| md theme jmo | html         | `false`  | ok     |
| md theme jmo | print        | `false`  | ok     |

![Figure BI](/branch/img/bi.png "BI")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | ok     |
| md hugo      | print        | `true`   | ok     |
| md hugo      | html         | `false`  | ok     |
| md hugo      | print        | `false`  | ok     |
| md theme old | html         | `true`   | ok     |
| md theme old | print        | `true`   | ok     |
| md theme old | html         | `false`  | ok     |
| md theme old | print        | `false`  | ok     |
| md theme old | print        | `false`  | ok     |
| md theme jmo | html         | `true`   | ok     |
| md theme jmo | print        | `true`   | ok     |
| md theme jmo | html         | `false`  | ok     |
| md theme jmo | print        | `false`  | ok     |

![Figure L](/leaf/l.png "L")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | ok     |
| md hugo      | print        | `true`   | ok     |
| md hugo      | html         | `false`  | ok     |
| md hugo      | print        | `false`  | ok     |
| md theme old | html         | `true`   | ok     |
| md theme old | print        | `true`   | ok     |
| md theme old | html         | `false`  | ok     |
| md theme old | print        | `false`  | ok     |
| md theme jmo | html         | `true`   | ok     |
| md theme jmo | print        | `true`   | ok     |
| md theme jmo | html         | `false`  | ok     |
| md theme jmo | print        | `false`  | ok     |

![FigureL LI](/leaf/img/li.png "LI")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | ok     |
| md hugo      | print        | `true`   | ok     |
| md hugo      | html         | `false`  | ok     |
| md hugo      | print        | `false`  | ok     |
| md theme old | html         | `true`   | ok     |
| md theme old | print        | `true`   | ok     |
| md theme old | html         | `false`  | ok     |
| md theme old | print        | `false`  | ok     |
| md theme jmo | html         | `true`   | ok     |
| md theme jmo | print        | `true`   | ok     |
| md theme jmo | html         | `false`  | ok     |
| md theme jmo | print        | `false`  | ok     |
