# R package `dfqr` documentation <img src="assets/images/dfqr_hex.png?raw=true" align="right" height="138" />


<!--
[![jsDelivr](https://data.jsdelivr.com/v1/package/gh/dfqr/dfqr/badge)](https://www.jsdelivr.com/package/gh/dfqr/dfqr)
![visitors](https://visitor-badge.laobi.icu/badge?page_id=dfqr.dfqr.github.io)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)



![CI](https://github.com/JV-conseil/jekyll-theme-read-the-docs/workflows/CI/badge.svg?branch=develop)
[![License BSD 3-Clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](LICENSE)
-->

| Find the R package                                 | Find the documentation                     |
|----------------------------------------------------|--------------------------------------------|
| [dfqr Github repo](https://github.com/dfqr/dfqr)   | [dfqr docs](https://dfqr.github.io/)   |

> Data frame management, including potentially big data, and query utility for R.

### Learn more by exploring the list below or the sidebar

- **[Index](/p/index.html)** - Detailed index

- **[Installation Guide](/p/Install.html)** - Install the package

- **[Quick Start Guide](/p/Quick-Start.html)** - Get up and running quickly

- **[Features & Use Cases](/p/features.html)** - The whole game

- **[FAQ](/p/faq.html)** - Frequently asked questions and common issues

- **[Tutorials](/p/Tutorials.html)** - Learn through tutorials

- **[Reference & Functions](/p/Reference-Functions.html)** - Function reference

- **[Benchmarks](/p/benchmarks.html)** - Performance

- **[News](/p/News.html)** - Stay up to date with latest developments

- **[Contribute](/p/contribute.html)** - Interested in contributing?

<!--

## What does it do?

Easily manage big data sets that can't fit into memory with minimum overhead.

## Quick start

1. **dfqr is an R package, so first install R and probably an IDE/editor.**

The best installation istructions for R and RStudio can be found at [Posit](https://posit.co/download/rstudio-desktop/).

2. **Install the package from Github using the remotes package**

```{r}
install.packages("remotes")
remotes::install_github("dfqr/dfqr")
```

## Usage

```{r}
library(dfqr)
```

1. **dfqr uses CSV files, so first convert your file type to CSV.**

The burden is on the user to write the source data to CSV. Many tools have this capability and conversion tools are available.

2. **dfqr checks your CSV formatting.**

Assuming your CSV file is called "mydata.csv".

```{r}
check_csv("mydata.csv")
```
dfqr tells you if the format doesn't match the package's CSV standard. If no issues were detected, skip step 4.

3. **dfqr will adapt your CSV to the dfqr CSV standard.**

Assume you would like to write the source data "mydata.csv" to a new file called "mydata_formatted.csv".

```{r}
rewrite_csv("mydata.csv", "mydata_formatted.csv")
```

4. **dfqr reads CSV data into an efficient format for reading.**

You can control the number of rows and columns to read efficiently. For example, say you want to read 1 million rows at a time of each column separately. Set rows to 1000000 and cols to 1.

```{r}
mydata = read_csv("mydata_formatted.csv", rows = 1000000, cols = 1)
```

5. **dfqr reads CSV data into an efficient format for reading.**

Now, read the first 1 million rows of the first variable. Set x to 1 (first million rows) and y to 1 (first variable).

```{r}
read_partial(mydata, x = 1, y = 1)
```

-->
