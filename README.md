# jpeg

#### Author of Package: Simon Urbanek

#### Author of Example Analysis and Deployed Website: Christine Hou

<!-- badges: start -->

<!-- badges: end -->

This package provides an easy and simple way to read, write and display bitmap images stored in the JPEG format. It can read and write both files and in-memory raw vectors.

### Project 3 Part 1

-   URL to the GitHub link to where the original R package came from: <https://github.com/s-u/jpeg>

-   URL to the deployed website: <https://jhu-statprogramming-fall-2023.github.io/biostat777-project3-part1-christinehou11/>

-   6 things I customized in my `pkgdown` website:

    -   Change the visual style of website using Bootswatch theme called **litera**

    -   Edit the color used for syntax highlighting in code blocks called **github-light**

    -   Override the default fonts used for main text to **Hedvig Letters Serif**

    -   Override the default fonts used for headings to **Open Sans**

    -   Change the background `bg`, foreground `fg`, and navbar/sidebar `primary` colors using `bslib` variable

    -   Change the background color used for inline code to **#2b2b2b**

## Installation

You can install the development version of jpeg like so:

``` r
install.packages("jpeg")
```

## Exported Functions

- **readJPEG(source, native = FALSE)**: Reads an image from a JPEG file/content into a raster array.


- **writeJPEG(image, target = raw(), quality = 0.7, bg = "white", color.space)**: Write a bitmap image in JPEG format and then create a JPEG image from an array or matrix.


## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(jpeg)

img<-readJPEG("myfile.jpeg")

plot(1:2, type='n')
rasterImage(img, 1, 1.25, 1.1, 1)
```
