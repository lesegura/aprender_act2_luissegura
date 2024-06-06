RMarkdown_actividad_2
================
Luis Segura
2024-06-06

## Introduccion

Primero voy a cargar la base de datos llamada NHANES que se encuentra
dentro del paquete NHANES.

``` r
library(tidyverse)
```

    ## ── Attaching core tidyverse packages ──────────────────────── tidyverse 2.0.0 ──
    ## ✔ dplyr     1.1.4     ✔ readr     2.1.5
    ## ✔ forcats   1.0.0     ✔ stringr   1.5.1
    ## ✔ ggplot2   3.5.1     ✔ tibble    3.2.1
    ## ✔ lubridate 1.9.3     ✔ tidyr     1.3.1
    ## ✔ purrr     1.0.2     
    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## ✖ dplyr::filter() masks stats::filter()
    ## ✖ dplyr::lag()    masks stats::lag()
    ## ℹ Use the conflicted package (<http://conflicted.r-lib.org/>) to force all conflicts to become errors

``` r
data("NHANES", package = "NHANES")
```

## Objetivo 1 - Descripcion de la base de datos

La NHANES es una encuesta recolectada por el NCHS que recolecta datos en
salud y nutricion desde los 60. Es una base de datos de individuos que
viven en hogares.

``` r
class(NHANES)
```

    ## [1] "tbl_df"     "tbl"        "data.frame"

El NHANES es un dataframe o base de datos compuesto por 10000 y por 76
variables.
