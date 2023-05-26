# README

Welcome to this Git repository where you can produce the base plot that turned into this: 
![The U.S. Presidency](https://github.com/whiteellie/us_presidents/blob/main/2_out/us_presidents_final.png)


This repository contains an R Markdown file that you can use to analyze data or create reports. To use the R Markdown file, you need to have the following:

1. R installed on your computer
2. RStudio (an integrated development environment for R) installed on your computer
3. The necessary R packages installed on your computer

## Installation

### 1. Install R

If you haven't already done so, please download and install R from the following website:

https://cran.r-project.org/

### 2. Install RStudio

Once you have installed R, you should then download and install RStudio from the following website:

https://www.rstudio.com/products/rstudio/download/

### 3. Install the necessary R packages

To run the R Markdown file, you will need to install the following packages and more:

- `tidyverse`
- `ggplot2`
- `knitr`
- `rmarkdown`

To install these packages, open RStudio and run the following commands in the console:

```
# Install the necessary packages
install.packages("tidyverse")
install.packages("ggplot2")
install.packages("knitr")
install.packages("rmarkdown")
``` 

You can customize the package list as per your requirements. Simply include this code block in your markdown file, and the packages will be installed when the code is executed.

## Usage

### 1. Download the R Markdown file

You can download the R Markdown file from this Git repository by clicking on  "<>Code" then "Download ZIP" or by cloning the repository using the following command:

```
git clone https://github.com/whiteellie/us-presidents.git
```

### 2. Open the R Markdown file in RStudio

Once you have downloaded the R Markdown file, open it in RStudio by navigating to the file location and double-clicking on the file.

### 3. Run the R Markdown file

You can run the R Markdown file by clicking on the "Knit" button in RStudio, or by running the following command in the console:

```
rmarkdown::render()
```


## Overall Process to Create the Viz

1) `rmarkdown` to get data ready. Major packages used were 'polite`, `httr`, and `rvest` to scrape the data from Wikipedia and `tidyverse` to clean up and format the data. 
2) `ggplot2::geom_segment() + coord_polar()` to make base plot segments, and other `ggplot` customizations with `ggimage()` and `facet_wrap`. 
3) PowerPoint to add chart elements

## Design Considerations

* I included portraits so the audience could easily identify and connect the data to the person who was serving in the office at the time. 
* Major party colors were picked to match the Wikipedia article for consistency. Other colors were picked and the grey slightly modified considering the contrast needed for those with visual impairements and/or colorblindness (508 compliance).
* Fonts were chosen and text hierarchy was deliberately designed to guide the eye and progressively deliver information. 
*  Information on parties were added in a dedicated legend spot to provide context for those not familiar with US political parties or their origins. Thanks to Reddit Users of r/dataisbeautiful for helping me refine that messaging to include the parties current stance in the political landscape. 
* "how to read the plot" diagram on the top left provides a quick orientation to how the data is layed out and is meant to be consumed first.
* Captions and color legend provide extra information about the underlying data and are meant to be consumed last if users are interested. 


## Conclusion

Thank you for using this Git repository! We hope that you find the R Markdown file useful for your data analysis or report writing needs. If you have any questions or feedback, please feel free to contact me white.elaheh@gmail.com.
