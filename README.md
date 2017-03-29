# OmniTheme

Forked from Bart6114/artyfarty, adding a new theme

## Installation

    devtools::install_github("erichare/omnitheme")

## How-To

    library(ggplot2)
    library(omnitheme)

    mydf <- data.frame(x = rnorm(100))
    mydf$y <- mydf$x + rnorm(100, sd = 2)

    ggplot(data = mydf, aes(x = x)) +
        watermark_img(system.file("images", "OAG_CLR_web_big.png", package = "omnitheme"), location = "center", alpha = .1, width = 250) +
        geom_histogram(alpha = 0.9) +
        theme_omni() + 
        ggtitle("Omni Analytics Theme")

    ggplot(data = mydf, aes(x = x)) +
        watermark_img(system.file("images", "OAG_CLR_web_big.png", package = "omnitheme"), location = "tl", alpha = .5, width = 55) +
        geom_histogram(alpha = 0.9) +
        theme_omni() + 
        ggtitle("Omni Analytics Theme")

    ggplot(data = mydf, aes(x = x)) +
        watermark_img(system.file("images", "OAG_CLR_web_big.png", package = "omnitheme"), location = "tl", alpha = .5, width = 55) +
        geom_histogram(alpha = 0.9) +
        theme_omni() + 
        ggtitle("Omni Analytics Theme")

    ggplot(data = mydf, aes(x = x, y = y)) +
        watermark_img(system.file("images", "OAG_CLR_web_big.png", package = "omnitheme"), location = "center", alpha = .1, width = 250) +
        geom_point(alpha = 0.6) +
        theme_omni() + 
        ggtitle("Omni Analytics Theme")

    ggplot(data = mydf, aes(x = x, y = y)) +
        watermark_img(system.file("images", "OAG_CLR_web_big.png", package = "omnitheme"), location = "tl", alpha = .5, width = 55) +
        geom_point(alpha = 0.6) +
        theme_omni() + 
        ggtitle("Omni Analytics Theme")
