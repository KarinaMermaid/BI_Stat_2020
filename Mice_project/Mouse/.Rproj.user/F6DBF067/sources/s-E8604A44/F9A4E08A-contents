# читаем данные
library("readxl")
mouse_data <- read_excel('Data_Cortex_Nuclear.xls')

#  смотрим их структуру
str(mouse_data)

# последние 4 колонки по идее на факторы можно поменять 
mouse_data$Genotype <- factor(mouse_data$Genotype)
levels(mouse_data$Genotype) <-  labels = с("Control", "Ts65Dn")

# смотрим, что с пропущенными значениями 
mouse_na <- colSums(is.na(mouse_data))
as.table(mouse_na)
mouse_data$class <- as.factor(mouse_data$class)
mouse_data$class
mouses_without_na <- na.omit(mouse_data)

ir <- iris
str(ir)
samp_ir <- sample_n(iris, 10, replace = TRUE) 

data("selfesteem2", package = "datarium")
selfesteem2 %>% sample_n_by(treatment, size = 1)
# Gather the columns t1, t2 and t3 into long format.
# Convert id and time into factor variables
selfesteem2 <- selfesteem2 %>%
   gather(key = "time", value = "score", t1, t2, t3) %>%
   convert_as_factor(id, time)

selfesteem2 %>% sample_n_by(treatment, time, size = 1)
?predict
?t
?n
?scatter3D
library(plotly)
??plotly
??rgl   
