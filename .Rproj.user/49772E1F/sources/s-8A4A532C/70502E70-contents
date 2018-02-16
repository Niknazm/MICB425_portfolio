#Comments
install.packages("tidyverse")
library(tidyverse)
#In terminal, copy data





#Load data
read.table(file="Saanich.metadata.txt")
#Save data as object in environment 
metadata = read.table(file="Saanich.metadata.txt", header=TRUE, row.names=1, sep="\t", na.strings =c("NAN", "NA", "."))

OTU = read.table(file="Saanich.OTU.txt", header=TRUE, row.names=1, sep="\t", na.strings =c("NAN", "NA", "."))




#DAY 2
library(tidyverse)
#%>% (take anything before "%>%" it puts it in the function), how it looks:
data %>% function
#last line does the same as function(data)

metadata %>% 
  select(02|oxygen) %>%


metadata %>% 
  select(matches (02|oxygen) %>% 
           
# ^this is used to look for anything that has the word O2 or oxygen in it
  
#to now look to see what rows have oxygen=0 and at what depth 
metadata %>%
  filer(02_um==0) %>%
  select(Depth_m)

#exercise:find at what deoth methane is above 100 nM while temperature is below 10  
#select: selects for columns
#filter: selects for rows

metadata %>%
  select(matches("CH4|methane"))


metadata %>%
  select(matches("temp"))

#the three lines below are the same thing

metadata %>%
  filter(CH4_nM>100) %>%
  filter(Temperature_C <10) %>%
  select(Depth_m,CH4_nM, Temperature_C)

metadata %>%
  filter(CH4_nM>100 & Temperature_C <10)

metadata %>%
  filter(CH4_nM>100, Temperature_C <10)

metadata %>%
  mutate(new=N20_nM/1000)



