---
archetype: "chapter"
title: "Branch Bundle"
weight: 2
---

This is a "branch bundle": All other markdown content next to this file (`_index.md`) _should_ be available.

The image resources are only available on the same directory level as the branch bundle itself. Thus `img/bi.png` should not be available.

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

![Figure B](b.png "B")

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

![Figure BI](img/bi.png "BI")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | nok    |
| md hugo      | print        | `true`   | nok    |
| md hugo      | html         | `false`  | ok     |
| md hugo      | print        | `false`  | ok     |
| md theme old | html         | `true`   | nok    |
| md theme old | print        | `true`   | nok    |
| md theme old | html         | `false`  | ok     |
| md theme old | print        | `false`  | ok     |
| md theme jmo | html         | `true`   | nok    |
| md theme jmo | print        | `true`   | nok    |
| md theme jmo | html         | `false`  | ok     |
| md theme jmo | print        | `false`  | ok     |

![Figure L](../leaf/l.png "L")

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

![FigureL LI](../leaf/img/li.png "LI")

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
