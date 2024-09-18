---
sort: 1
---

# Installation Instructions <img src="assets/images/dfqr_hex.png?raw=true" align="right" height="138" />

## 0. **System Dependencies**

`dfqr` is only available for Unix-like operating systems such as MacOS and Linux.

## 1. **Install R and an IDE**

Before installing dfqr, ensure you have R and an IDE (e.g., RStudio). The best installation guide for R and RStudio can be found here.

## 2. **Install dfqr from GitHub**

Install `dfqr` via the `remotes` package:

```r
install.packages("remotes")
remotes::install_github("dfqr/dfqr")
```

## 3. **Usage**

Load the package after installation:

```r
library(dfqr)
```