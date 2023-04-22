AY2023 semester 2 lab group B134 SC1015 mini project 
Collaborators: SAM YE ZHI and OATES BENJAMIN HARRY
Description:
This mini project was started in mind to try and predict the meta in the popular online multiplayer game League of Legends (LOL).
The mini project serves to try and predict the meta by trying to predict which characters inside LOL would be buffed or nerfed in subsequent gameplay update patches.

We first retrieved 2 datasets from Kaggle which is a popular website providing datasets. The dataset contained data on the names, win rates, pick rates, ban rates and 
some other variables on characters in patch 12.11 and 12.14 of LOL. We imported the csv files into jupyter notebook and cleaned the data. We removed unnecessary columns
of information from the dataset such as KDA and only left useful variables. We also manually scraped through all the LOL patch notes from 12.11 to 12.17 for data on which champions were buffed or nerfed. We added 2 more columns of variables inside the datasets called "Buffed" and "Nerfed". Those 2 variables are categorical variables that are either labeled 1 or 0. Champions that were buffed within 3 gameplay patches would be labelled 1 under the "Buffed" column and vice versa. Likewise, champions that were nerfed within 3 gameplay patches would be labelled 1 under the "Nerfed" column and vice versa.

We then calculated the correlation values between each of our three numerical variables Win, Pick, Ban and the categorical variables of Buffed and Nerfed. We
visualized the data by plotting out box and violin plots for the relationship between the three numerical variables and the categorical variables. After that, we used
a weighted average based on the correlation of the three numerical variables and the categorical variables to create 2 new variables "weighted buffed" and "weighted 
nerfed" which were used to predict how each character was positioned in terms of their strength in the meta. We plotted a scatterplot for 12.11 and listed the rankings
of the characters based on the new weighted variables. We did the same for data from patch 12.14 to test if our approach was accurate. Finally we used machine learning for anomaly detection to find out why certain characters which were ranked highly were not getting nerfed or why characters that were ranked very lowly were not getting buffed.

        
