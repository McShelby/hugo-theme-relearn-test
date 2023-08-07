---
archetype: "home"
title: "Home"
---

We have defined a few pages and some image resources in this example to see how linking of images works with plain markdown links.

| File                 | Type                     | Remark
|----------------------|--------------------------|--------|
| `/_index.md`         | Home (branch)            |        |
| `/index.md`          | Home (leaf)              | not tested |
| `/h.png`             | Home resource            |        |
| `/img/hi.png`        | Home resource (nested)   | not allowed in Hugo, at least it's not showing in the resources |
| `/singleh.md`        | Single (on home level)   |        |
| `/leaf/index.md`     | Leaf                     |        |
| `/leaf/l.png`        | Leaf resource            |        |
| `/leaf/img/li.png`   | Leaf resource (nested)   |        |
| `/leaf/singlel.md`   | Single (on leaf level)   | not allowed in Hugo, at least it's not showing in the resources nor is it printed in the menu |
| `/branch/_index.md`  | Branch                   |        |
| `/branch/b.png`      | Branch resource          |        |
| `/branch/img/bi.png` | Branch resource (nested) | not allowed in Hugo, at least it's not showing in the resources; probably supposed for an non existing bundle page of `branch/img` |
| `/branch/singleb.md` | Single (on branch level) |        |


## Flavor

- `md hugo` is the default implementation of Hugo without any own render hooks (to test, remove the themes `render-link.html` render hook)
- `md theme old` is the current render hook of the theme (the default in this test)
- `md theme jmo` is the implementation of [Joe Morington](https://www.veriphor.com/articles/link-and-image-render-hooks/) (to test, replace the `render-link.html` render hook)

## OutputFormat

- `html` is the display the HTML page in the browser
- `print` is the display of the chapter by pressing CTRL+ALT+P on each pge in the browser

## uglyURLs

Hugos setting to change branch and leaf bundles URLs from eg. `branch.html` to `branch/index.html`

## defaultContentLanguageInSubdir

Only the default @defaultContentLanguageInSubdir=false@ was tested.

## Results

- Results for `hi.png` and `bi.png` can be ignored, because of invalid Hugo structure.
- Project relative and aboslute works always.
- Page relative on the home page as branch bundle works always.
- Hugo can not address resources in their containing branch bundle if uglyURLs=true.
- JMos version is slightly better than the themes implementation in finding resources directly in branch bundles (h.png / b.png)

{{< resources >}}

#### Page Relative

![Figure H](h.png "H")
![Figure H with dot](./h.png "H")


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

![Figure HI](img/hi.png "HI")

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

![Figure B](branch/b.png "B")

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

![Figure BI](branch/img/bi.png "BI")

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

![Figure L](leaf/l.png "L")

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

![FigureL LI](leaf/img/li.png "LI")

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

#### Project Relative

Pathes with a starting `/` are always interpreted as relative to your projects content not your server root.

Project content and server root are different if you give a `baseurl` in your `config.toml` including a sub directory for your Hugo project.

An interpretation relative to your servers web root is not supported. This still may work as a fallback if a relative link meant as server relative is not contained in your Hugo project. But if this link is ambigous and valid interpreted as server relative _and_ project relative, project relative will win and be generated.

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

#### Absolute

It's enough to test it on one page, we do not repeat this on the sub pages.

![Figure H](http://localhost:1313/public/h.png "H")

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

![Figure HI](http://localhost:1313/public/img/hi.png "HI")

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

![Figure B](http://localhost:1313/public/branch/b.png "B")

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

![Figure BI](http://localhost:1313/public/branch/img/bi.png "BI")

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

![Figure L](http://localhost:1313/public/leaf/l.png "L")

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

![FigureL LI](http://localhost:1313/public/leaf/img/li.png "LI")

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
