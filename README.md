
# despair

# Overview

`despair` is a package inspired by Shakespeare’s work and his well-known
pessimism. It allows the user to create short, clever codes called
bard–bits inspired by Shakespeare’s work and use daily demotivational
quotes for personal use or to share with others.

## Installation

You can install this package on CRAN

``` r
install.packages("despair")
```

You can also install the development version of this package through the
`devtools` package.

``` r
devtools::install_github("jpmonteagudo28/despair")
```

## Usage

There are three basic functions in the package: demotivate, motivate,
and bard.bits. Each function will take a category input and an optional
numeric or character seed for reproducible results.

``` r
library(despair)

#> Get info on package version 
 despair.message()
#> despair string generated by {despair} v.0.1.0.R version 4.4.1 (2024-06-14 ucrt).

demotivate()
#> "I’m not really good at advice. Can I interest you in a sarcastic comment?"
demotivate("science", seed = 123)
#> "No matter how hard you try, you’ll always be within one standard deviation of average."
demotivate("science", seed = "lanky poodle")
#> "Don't worry! There might be a socio-anthropoligical intepretation of your results"

motivate("lit")
#> "If you tell the truth, you don't have to remember anything. — Mark Twain"
motivate("religion", seed = 123)
#> "The Christian does not think God will love us because we are good, but that God will make us good because He loves us. - C.S. Lewis"
motivate("religion", seed = "bewildered pooh")
#> "Really great things, when discussed by little men, can usually make such men grow big. - Augustine of Hippo"

bard.bits()
#> "brownish purple kite"
bard.bits("character", seed = 123)
#> "filthy duncan"
bard.bits("character", seed = "stinky chihuahua")
#> "lofty tranio"
```
