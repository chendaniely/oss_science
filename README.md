# oss_science
NSF NCSES project on cost/value of OSS projects

# Setup

Code base is mainly in R

## Setup Github keys as an environment variable

Make sure you have the `usethis` library installed

```r
# install.packages('usethis')
```

Modify your `.Renviron`

```r
usethis::edit_r_environ()
```

Add the following lines to the `.Renviron` (make sure the file ends with a new line!)
Where the `XXXXX` and `YYYYY` are your Github Application Client ID and Client Secret values.

```
GH_CLIENT_ID=XXXXX
GH_CLIENT_SECRET=YYYYY
```

Now restart your R session, and your github keys should be availiable to you as an environment variable.

```r
Sys.getenv("GH_CLIENT_ID")
Sys.getenv("GH_CLIENT_SECRET")
```
