# CryptoClustering
A challenge to utilize knowledge of Python with sklearn library and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes. 

## Data Collection and Preprocessing
The datasets used for analysis were provided by edX Boot Camps LLC, and are intended for educational purposes only. I used pandas to load the csv data into a dataframe. I performed basic preprocessing steps such as data cleaning, feature selection "price_change_percentage_24h" and "price_change_percentage_7d", and checking for missing values. I utilized StandardScaler() from the sklearn library to normalize the dimensions of the data.

## Methods
I imported essential dependencies like pandas, hvplot, and sklearn. After preprocessing the data, I used the elbow method to find the best k-value to cluster the original data. The resulting line graph showed that four was the best k-value.

![Value for k Using Original Data](https://github.com/ASPigman/CryptoClustering/assets/145923874/c6e2b717-343b-44e2-8132-8f08d0d600bb)

From there, I used K-means to cluster the data with a k-value of four. Then I used hvplot to plot the clusters in a scatterplot. The results are shown below.

![Kmeans clusters Using the Original Data](https://github.com/ASPigman/CryptoClustering/assets/145923874/e7972300-5b97-4763-a748-b051a5c059a1)

To compare clustering techniques, I utilized the Principal Component Analysis (PCA) model with three components. This helped to reduce the number of features used to cluster the data. The goal os this is to capture as much of the variance while simultaneously considering less of the data. The total explained variance of the three principal components came to 89.50%, which indicates quite good accuracy. From there, I followed the same pattern as I did using the original data. I first found the best k-value using the elbow method. The result for this was also four.

![Best Value for k Using PCA Data](https://github.com/ASPigman/CryptoClustering/assets/145923874/b2e47cff-cf89-4be0-a149-859c2d842c9d)

Then, I again utilized K-means to cluster the data with a k-value of four. Then I used hvplot to plot the clusters in a scatterplot.

![kmeans clusters using pca data](https://github.com/ASPigman/CryptoClustering/assets/145923874/249e4f07-fd55-4434-94e5-fc600f0bd876)


## Conclusion


## Acknowledgements
Othmane Benyoucef - Instructor for Tulsa Community College Data Analytics Accelerated Training Program

Kaylie Butler - TA

Jacob Peroutek - TA

EdX Bootcamps

<a href="https://plnkr.co/edit/qAjh0duPRI4US6Q4DSCN?p=preview&preview" target="_blank">Adjusting font color for legend in CSS</a>
