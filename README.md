# ETC5513-Team11-A4

Data: tidytuesday - Coffee Ratings

## About the Data
The data is from the Coffee Quality Institute's trained reviewers. It contains professional ratings for Arabica and Robusta Coffee Beans. Ratings are based on Sweetness, Acidity, Fragrance, Balance, etc. The rating is indocated by the total_cup_points variable where the scale is from 0 - 100. It also contains information about the processing method, expiration date, number of bags, bag weight, country of origin, company name and farm name. 

The data set contains **1339** rows and **43** variables. 

## Source
The data can be obtained from: https://github.com/rfordatascience/tidytuesday/blob/master/data/2020/2020-07-07/readme.md

```{r}
# Get the Data

# Read in with tidytuesdayR package 
# Install from CRAN via: install.packages("tidytuesdayR")
# This loads the readme and all the datasets for the week of interest

# Either ISO-8601 date or year/week works!

tuesdata <- tidytuesdayR::tt_load('2020-07-07')
tuesdata <- tidytuesdayR::tt_load(2020, week = 28)

coffee_ratings <- tuesdata$coffee_ratings

# Or read in the data manually

coffee_ratings <- readr::read_csv('https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2020/2020-07-07/coffee_ratings.csv')

```

## About the Project

All through our lives, there definitely has been a coffee lover we know or we will be coffee lovers ourselves. Coffee has helped a lot of us to stay awake to complete our assignments or any other important tasks. It has also worked adversely for many of us, where we drink coffee at very late hours and find it difficult to fall asleep. Coffee was first exported from Ethiopia to Yemen in the late 15th Century. This analysis will help in understanding the nature of the different coffee beans (Arabica and Robusta), the regions where it is grown, the ratings for the different types of coffee beans and also the processing methods. 


## Research Questions

1. How many bags of coffee from each country were sampled? 
2. Which country produces the highest rated coffee?
3. Which top3 countries cultivated most kinds of Arabica coffee beans and Robusta coffee beans respectively?
4. What is the difference of altitude of Arabica coffee beans and Robusta coffee beans production areas?
5. Which processing method leads to better rating
6. Which harvest year produced the best coffee?

## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are greatly appreciated!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b NewFeature`)
3. Commit your Changes (`git commit -m 'Add some New Feature'`)
4. Push to the Branch (`git push origin NewFeature`)
5. Open a Pull Request

## License
See `LICENSE` for more information.

## Contact

1. Sahinya Akila (saki0001@student.monash.edu)
2. Yiwen Liu ()
3. Panagiotis Stylianos ()
