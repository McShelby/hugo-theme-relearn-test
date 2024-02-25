---
archetype: default
title: "Single page on home level"
weight: 1
---

This is a "single page" in a "branch bundle" and should **not** be available. Results may change if the home page is renamed from `_index.md` to `index.md` but that wasn't tested.

{{< resources >}}

#### Page Relative

![Figure H](../h.png "H")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | ok     |
| md hugo      | print        | `true`   | nok    |
| md hugo      | html         | `false`  | nok    |
| md hugo      | print        | `false`  | nok    |
| md theme old | html         | `true`   | ok     |
| md theme old | print        | `true`   | nok    |
| md theme old | html         | `false`  | nok    |
| md theme old | print        | `false`  | nok    |
| md theme jmo | html         | `true`   | ok     |
| md theme jmo | print        | `true`   | ok     |
| md theme jmo | html         | `false`  | ok     |
| md theme jmo | print        | `false`  | ok     |

![Figure HI](../img/hi.png "HI")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | ok     |
| md hugo      | print        | `true`   | nok    |
| md hugo      | html         | `false`  | nok    |
| md hugo      | print        | `false`  | nok    |
| md theme old | html         | `true`   | ok     |
| md theme old | print        | `true`   | nok    |
| md theme old | html         | `false`  | nok    |
| md theme old | print        | `false`  | nok    |
| md theme jmo | html         | `true`   | ok     |
| md theme jmo | print        | `true`   | nok    |
| md theme jmo | html         | `false`  | nok    |
| md theme jmo | print        | `false`  | nok    |

![Figure B](../branch/b.png "B")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | ok     |
| md hugo      | print        | `true`   | nok    |
| md hugo      | html         | `false`  | nok    |
| md hugo      | print        | `false`  | nok    |
| md theme old | html         | `true`   | ok     |
| md theme old | print        | `true`   | nok    |
| md theme old | html         | `false`  | nok    |
| md theme old | print        | `false`  | nok    |
| md theme jmo | html         | `true`   | ok     |
| md theme jmo | print        | `true`   | nok    |
| md theme jmo | html         | `false`  | nok    |
| md theme jmo | print        | `false`  | nok    |

![Figure BI](../branch/img/bi.png "BI")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | ok     |
| md hugo      | print        | `true`   | nok    |
| md hugo      | html         | `false`  | nok    |
| md hugo      | print        | `false`  | nok    |
| md theme old | html         | `true`   | ok     |
| md theme old | print        | `true`   | nok    |
| md theme old | html         | `false`  | nok    |
| md theme old | print        | `false`  | nok    |
| md theme jmo | html         | `true`   | ok     |
| md theme jmo | print        | `true`   | nok    |
| md theme jmo | html         | `false`  | nok    |
| md theme jmo | print        | `false`  | nok    |

![Figure L](../leaf/l.png "L")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | ok     |
| md hugo      | print        | `true`   | nok    |
| md hugo      | html         | `false`  | nok    |
| md hugo      | print        | `false`  | nok    |
| md theme old | html         | `true`   | ok     |
| md theme old | print        | `true`   | nok    |
| md theme old | html         | `false`  | nok    |
| md theme old | print        | `false`  | nok    |
| md theme jmo | html         | `true`   | ok     |
| md theme jmo | print        | `true`   | nok    |
| md theme jmo | html         | `false`  | nok    |
| md theme jmo | print        | `false`  | nok    |

![FigureL LI](../leaf/img/li.png "LI")

| flavor       | outputFormat | uglyURLs | result |
|--------------|--------------|----------|--------|
| md hugo      | html         | `true`   | ok     |
| md hugo      | print        | `true`   | nok    |
| md hugo      | html         | `false`  | nok    |
| md hugo      | print        | `false`  | nok    |
| md theme old | html         | `true`   | ok     |
| md theme old | print        | `true`   | nok    |
| md theme old | html         | `false`  | nok    |
| md theme old | print        | `false`  | nok    |
| md theme jmo | html         | `true`   | ok     |
| md theme jmo | print        | `true`   | nok    |
| md theme jmo | html         | `false`  | nok    |
| md theme jmo | print        | `false`  | nok    |

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
