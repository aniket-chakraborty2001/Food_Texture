# Food_Texture
Here I use the Food_Texture Data set and use data mining steps to complete the project
### Introduction:
In this project we will use the Food_Twxture_Data which is given in the project files as .csv file. This data we get from the website <https://openmv.net/info/food-texture>
This data set contains differnt products and their Density, Oil,Hardness, Fracture and Crispyness. Here we perform data mining steps in order to understand the data.

### Explanation of the project:
Like other projects here we perform the same data mining steps. They are discussed briefly:

#### 1. Installing and loading packages:
At first we install and load the required packages useing the **install.packages()** function. We use the tidyverse packages here. Under this package we use the following libraries:
* tidyverse
* dplyr
* gbgplot2

#### 2. Data Reading:
In this step we read the **Food_Texture_Data.csv** file using **read.csv()** function. The function comes under the readr library of tidyverse package.

#### 3. Data Understanding:
In this step we use commands to know the data set well. This step includes Previewing the data, knowing the structure of the data, getting summary statistics of each and every continuous column , getting row and column numbers and getting first few rows of the data set. In this process we use some functions like:
* View()
* Str()
* summary() or glimpse()
* head()
* nrow() and ncol()

#### 4. Data manipulation:
This is the third step of data mining. In this step we use the **dplyr libratry** along with the pipe operator, which is denoted as **"%>%"** This step deals with missing data, correcting errors, renaming variable names, selecting some variables, filtering data from data set, group them by categories, calculating different values such as max,min etc. The functions that are involved in this step are as follows:
* select()
* filter()
* group_by()
* rename()
* summarize()
* mutate() and so on.

for example in this project we change the names of the cariables Oil, Crispy,X. Mutate the Price_in_dollar and Price_in_Rs columns. Filter the Product which costs the least and so on.

#### 5. Data Visualization:
In this step we visualize the trend or relationship between the data's different variables. For this case we use the **ggplot2 library** that comes under the tidyverse package. To plot the graphs we use **ggplot()** function. It uses some parameters such as **mapping, aesthetics, plot object** etc. Using this functions we can plot dot plot, line graph, bar grapg, boxplot, histogram, density plot, pie chart and so on. It produces high level graphical output. For example in this project we create plots for:
* Price vs Density
* Price vs Oil
* Price vs Hardness
* Price vs Crispyness
* Price vs Hardness

#### Conclusions of this Project:
This includes the inferences we made by doing or completing the project. The inferences are:
* The produch names **B237** costs the least.

* There is no such  strong linear relation or trend between Density and Price. The price of a product is spread all over the density values. The Price and the density tend to make a cluster in the center region.

* There is no such  strong linear relation or trend between Oil_Percentage and Price. The price of a product is spread all over the oil percentage values. The Price and the oil percentage tend to make a cluster in the center region.

* However the Price and Crispyness of the product are in a amazing pattern. we can say that for one value of crispyness we can observe prices of different objects. In other words from this plot we can not say that Price depends on direct Crispyness. We have to consider other factors too.

* As the Fracture increases, the price of the product also increases. It looks like the plots of the fisrt two cases.

* Well Hardness is the most important factor that clearly depicts the relationship between price and itself. As Hardness increases the Price of the product decreases in a linear trend. 
