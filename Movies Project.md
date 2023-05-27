# Movies Project

## Group members:
- Fai Alamri 
- Omar Alnasser
- Hisham Altayieb 


## Movies Report

  The movie industry has been a great influence on our everyday life from the 19th century. Movies have been used as means to educate people on history or to entertain people with fictional stories.
We want to dive deeper into the influence of movies. What makes a movie popular? what elements help elevate a movie? how much the movie industry has grown over the years? In the next section we will
answer all of these questions and more to compeletely analyze the movie industry.


We used "tmdb-movies" which is a database we downloaded from Kaggle that has ten thousand movies to analyze.
### This analysis process will contain the following questions:
   - Which genres are most popular from year to year?
   - What kinds of properties are associated with movies that have high revenues?
   - How much revenue do movies get over the years based on their budget?
   - Does the amount of budget spent on a movie affect its rating?
   - Is there a correlation between the amount of movies a production make and their success?
   - Is there a correlation between the amount of movies a director makes and their success?
   - Is there a correlation between the revenue a movie gets and its rating?
   - Have the movie industry been declining over the years with the appearance of other entertainment means?
   
   Our dataset information:
   
   ![Screenshot 2023-05-27 162147](https://github.com/Nier1419/Bootcamp-Project-2-Data-Analysis/assets/85634276/0652eebe-9200-47ca-9b00-74830bf0071e)

  According to our questions, we do not need missing values such as keywords, tagline, director, homepage, and production_companies, due to it don't have any effect on our data analysis process. 
We found that there were 10866 rows in the dataset with a variety of data types and some missing values. During our analysis, we are only interested in genres and release years columns, 
as well as some zero values in the revenue column and the budget column. A few changes have been made to some types of data to make calculations easier, 
including replacing zero values with column means, removing duplicates, and replacing zero values with column means.

###  Which genres are most popular from year to year?
We want to display which genres are most popular from 1960 to 2015, by displaying it in two chart one from 1960 till 1999,and the second from 2000 till 2015.

![MostMadeGenres2000](https://github.com/Nier1419/Bootcamp-Project-2-Data-Analysis/assets/85634276/874af351-c35c-4403-b2fd-74e92dc4a722)

After checking most popular genres thoughout the years, we wanted to check what are the most popular genres in general by using a pie chart:

![Popularity of Genres](https://github.com/Nier1419/Bootcamp-Project-2-Data-Analysis/assets/85634276/f26abcf3-171b-4cf8-9a71-6a4f29c2b4c4)

We have 21 genres. As a result, a total of 4251 movies were watched in 48 years in drama and comedy genres.

### What kinds of properties are associated with movies that have high revenues?

According to IMDB top rated 250 movies are above 8.0 unfortunately there is no standard rating even though in other websites such as rotten tomato.
So we will look into movies that have larger revenues which is above the mean and then check if it has 8.0 < rating or not. We will also make sure the revenues is higher than the average.

We compared between the revenue and the runtime for shows:

![Revenue and RunTime comparison](https://github.com/Nier1419/Bootcamp-Project-2-Data-Analysis/assets/85634276/228ca1d3-a523-4939-8f13-f9f19575ab86)

We also compared between popularity and revenue as shown below:

![popularity and Revenue Comparison](https://github.com/Nier1419/Bootcamp-Project-2-Data-Analysis/assets/85634276/779a717b-296e-4c1e-ac2d-51ade08c6595)

Then we showed every movies revenue compared to their vote average:

![vote average and revenue comparison](https://github.com/Nier1419/Bootcamp-Project-2-Data-Analysis/assets/85634276/f167c26e-0d93-495b-bd68-e9e7f3263aff)

After the visualization of our data, we discovered that 13 movies have higher revenue than the average and above 8.0 rate.

### How much revenue do movies get over the years based on their budget?

Showing the revenues increase by billions over the years:

![revenue throughout the years](https://github.com/Nier1419/Bootcamp-Project-2-Data-Analysis/assets/85634276/298f3790-dbcc-4865-a9c5-e92ae5d4ad0c)

Showing the budgets increase by 100 millions over the years:

![budget throughout the years](https://github.com/Nier1419/Bootcamp-Project-2-Data-Analysis/assets/85634276/ac6c2187-e0de-4d3d-a653-04b5eb8d196d)

Showing the difference of increase for both budget and revenue:

![budget and revenue comparison](https://github.com/Nier1419/Bootcamp-Project-2-Data-Analysis/assets/85634276/f2694c44-ff46-48df-9a67-a88825f077ed)

After visualizing movies revenue and budget, we discovered that revenue is in a steep increase in billions where budgets do not increase as much.

### Does the amount of budget spent on a movie affect its rating?

We will viualize the budget spent on a movie with the movies rating using a stem chart:

![budget to rating](https://github.com/Nier1419/Bootcamp-Project-2-Data-Analysis/assets/85634276/7541cd9a-7a33-4598-982c-b8845de298e8)

After visualizing our data, a movie with the highest budget in our chart which was 141 million got a rating of 6.4 which shows that budget does not affect rating.

### Is there a correlation between the amount of movies a production make and their success?

![company vs movies](https://github.com/Nier1419/Bootcamp-Project-2-Data-Analysis/assets/85634276/e4146067-45a8-48f0-8c10-8cda13fb5148)

As we can see the companys experience with making movies does not correlate to their movies success.

### Is there a correlation between the amount of movies a director makes and their success?

We wanted to know if the same applies for directors, so we visualized our data as seen below:

![directors and movies](https://github.com/Nier1419/Bootcamp-Project-2-Data-Analysis/assets/85634276/574e6ebc-64c6-4d88-aab5-3e5e74680380)

The graph concludes that the same applies with directors. Their experience with making movies does not correlate with a movies success.

### Is there a correlation between the revenue a movie gets and its rating?

First we wanted to show movies with the highest revenue only.

![revenue and rating to movies](https://github.com/Nier1419/Bootcamp-Project-2-Data-Analysis/assets/85634276/f5910e22-3373-4eb7-9081-a68815240bcc)

Then we visualized the highest rated movies with no regard to their revenue:

![highest rated movies](https://github.com/Nier1419/Bootcamp-Project-2-Data-Analysis/assets/85634276/a5757319-2db2-4701-bf97-f671c1777bfe)

We conclude that a movie can be a huge success in revenue but not get a high rating.

### Have the movie industry been declining over the years with the appearance of other entertainment means?
 
 To know wether the movie industry is declining or not, we visualized the amount of movies made by the years.
 
 ![number of movies made throughout the years](https://github.com/Nier1419/Bootcamp-Project-2-Data-Analysis/assets/85634276/0979a017-cda4-4c5e-96cd-69a0751d11f5)

As we can see the amount of movies made kept on increasing which means the movie industry is still an essential entertainment tool.



## Sources and references:
- [Kaggle]()
- [IMDB top rated movies](https://www.imdb.com/chart/top?pf_rd_m=A2FGELUUNOQJNL&pf_rd_p=4da9d9a5-d299-43f2-9c53-f0efa18182cd&pf_rd_r=9S9ZTYQ2Z3V30C03YNDV&pf_rd_s=right-4&pf_rd_t=15506&pf_rd_i=bottom&ref_=chtbtm_ql_3)
- Stack Overflow
- GeeksforGeeks
- matplotlib.org
- Coolors
- [python-charts.com](https://python-charts.com/matplotlib/styles/#:~:text=Matplotlib%20provides%20built-in%20style%20sheets%20to%20customize%20the,printing%20the%20following%3A%20import%20matplotlib.pyplot%20as%20plt%20print%28plt.style.available%29)
