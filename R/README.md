# Notes on R and dplyr etc

view date formats (e.g. %d, %m etc): ?strptime()
***
[moving ave](https://datavizpyr.com/how-to-make-time-series-plot-with-rolling-mean-in-r/):
<br>
```
library(tidyverse)
library(zoo)

data %>%
  mutate(seven_avg= rollmean(<target_column>, 7, align="left", fill=0)) %>%
  ggplot(aes(x = ...) +
  geom_line(aes(y = seven_avg), color = "red", size = .75)
```
***
[dual y axis](https://ggplot2.tidyverse.org/reference/geom_linerange.html)
or
[dual y axis](https://www.r-graph-gallery.com/line-chart-dual-Y-axis-ggplot2.html)
***

