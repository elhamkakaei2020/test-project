# test-project
just for test
install.packages("tidyverse")
library(tidyverse)
data()
view(mpg)
?mpg
glimpse(mpg)
str(mpg)
?filter
filter(mpg, cty>=20)
mpg-efficient <- filter(mpg, cty>=20)

mpg_efficient <- filter(mpg, cty >= 20)
view(mpg_efficient)
mpg-ford <- filter(mpg, manufacturer =="ford")
view(mpg)
mpg_ford <- filter(mpg, manufacturer == "ford")
view(mpg_ford)
mpg-metric<-mutate(mpg, cty_metric==0.425144*cty)
mpg_metric <- mutate(mpg, cty_metric = 0.425144 * cty)
glimpse(mpg_metric)
?mutate
mpg %>% 
  group_by(class) %>% 
  summarise(mean(cty)) 
view(mpg)
__calc
?calc
??calc
?pull
