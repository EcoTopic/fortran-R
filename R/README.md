# Notes on R and dplyr etc

[moving ave](https://datavizpyr.com/how-to-make-time-series-plot-with-rolling-mean-in-r/):
`library(tidyverse)
library(zoo)
data %>%
mutate(seven_avg= rollmean(positiveIncrease, 7,
                             align="left",
                             fill=0)) %>%
ggplot(aes(x = ...) +
geom_line(aes(y = seven_avg), color = "red", size = .75)`
                             

view date formats (e.g. %d, %m etc): ?strptime()
