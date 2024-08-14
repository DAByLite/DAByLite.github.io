# DAByLite docs <a href="https://DAByLite.github.io"><img src="assets/images/DAByLite_hex.jpeg?raw=true" align="right" height="138" /></a>

[![jsDelivr](https://data.jsdelivr.com/v1/package/gh/dabylite/dabylite/badge)](https://www.jsdelivr.com/package/gh/dabylite/dabylite)
![visitors](https://visitor-badge.laobi.icu/badge?page_id=DAByLite.DAByLite.github.io)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)


<!--
![CI](https://github.com/JV-conseil/jekyll-theme-read-the-docs/workflows/CI/badge.svg?branch=develop)
[![License BSD 3-Clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](LICENSE)
-->

> Big data management in R

## What it does

Easily manage big data sets that can't fit into memory with minimum overhead.

## Quick start

1. **DAByLite is an R package, so first install R from the [R Project](https://www.r-project.org/).**

The best installation istructions for R and RStudio can be found at [Posit]([https://www.r-project.org/](https://posit.co/download/rstudio-desktop/)).

3. **Install the package from Github using the remotes package**

```{r}
install.packages("remotes")
remotes::install_github("DAByLite/DAByLite")
```

## Usage

```{r}
library(DAByLite)
```

1. DAByLite uses CSV files, so first convert your file type to CSV.

The burden is on the user to write the source data to CSV. Many tools have this capability and conversion tools are available.

2. DAByLite checks your CSV formatting.

Assuming your CSV file is called "mydata.csv".

```{r}
check_csv("mydata.csv")
```
DAByLite tells you if the format doesn't match the package's CSV standard. If no issues were detected, skip step 4.

4. DAByLite will adapt your CSV to the DAByLite CSV standard.

```{r}
write_csv("mydata.csv", "mydata_formatted.csv")
```

5. DAByLite reads CSV data into an efficient format for reading.

```{r}
read_csv("mydata.csv")
```

## Features

- Shortcodes (Toasts card, mermaid)
- Pages Plugins (emoji, gist, avatar, mentions)
- Auto generate sidebar
- [Attribute List Definitions](https://kramdown.gettalong.org/syntax.html#attribute-list-definitions) (Primer/css utilities, Font Awesome 4)
- Service worker (caches)
- SEO (404, robots.txt, sitemap.xml)
- Canonical Link (Open Graph, Twitter Card, Schema data)

## Options

| name          | default value        | description       |
| ------------- | -------------------- | ----------------- |
| `title`       | repo name            |                   |
| `description` | repo description     |                   |
| `url`         | user domain or cname |                   |
| `baseurl`     | repo name            |                   |
| `lang`        | `en`                 |                   |
| `direction`   | `auto`               | `ltr` or `rtl`    |
| `highlighter` | `rouge`              | Cannot be changed |

```yml
# folders sort
readme_index:
  with_frontmatter: true

meta:
  key1: value1
  key2: value2
  .
  .
  .

google:
  gtag:
  adsense:
  site_verification:

# GDPR compliant alternative to Google Analytics
mouseflow:
  project_api_key:

posthog:
  project_api_key:

telemetry:
  app_id:
  user_identifier:

umami:
  website_id:

mathjax: # this will prased to json, default: {}

# NOTE: mermaid custom link are no longer supported
# instead mermaid is updated to the lastest version
# available through cdn.jsdelivr.net
# mermaid:
#   custom:     # mermaid link
#   initialize: # this will prased to json, default: {}

scss:   # also _includes/extra/styles.scss
script: # also _includes/extra/script.js

translate:
  # shortcodes
  danger:
  note:
  tip:
  warning:
  # 404
  not_found:
  # copyright
  revision:
  # search
  searching:
  search:
  search_docs:
  search_results:
  search_results_found: # the "#" in this translate will replaced with results size!
  search_results_not_found:

plugins:
  - jemoji
  - jekyll-avatar
  - jekyll-mentions
```

## Sponsorship

If this project helps you, you can offer me a cup of coffee ☕️ :-)

[![Become a sponsor to JV-conseil](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/JV-conseil)

<!-- links -->

[rundocs/starter]: https://github.com/rundocs/starter
