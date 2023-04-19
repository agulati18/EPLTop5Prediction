# Predicting English Premier League Season Outcomes

## Introduction

I aimed to tackle the business problem of predicting season outcomes for teams in the English Premier League. My goal was to predict which teams would come in the 'Top 5', get relegated, or remain in the league based on their Wins, Draws, Losses, Goals Scored, and Goals Conceded.

## Data

I used a dataset of English Premier League Standings from 2010 to 2021, which included all team standings at the end of the season. I dropped columns with team names and qualification/relegation to remove noise. Further, I dropped the points and position columns because they were perfectly correlated with outcomes, which is what I was trying to predict.

## Methodology

I applied decision tree models to make our predictions, utilizing feature engineering and data preprocessing to fine-tune model results. My analysis highlighted the significance of Wins and Losses as key predictors of team success, as well as Goals Scored and Goals Conceded. I also learned about the importance of evaluating model performance accurately.

## Results

My findings suggest that incorporating additional independent variables such as 'Total Team Value', 'Freekicks and Penalties received and conceded', and 'Number of Managerial changes in the season' could further improve our predictions. The feature importances revealed that Wins and Losses make up the majority of the importance, followed by Goals Scored and Goals Conceded, while Draws only count for a very small percentage.

I also visualized the first decision tree with depth 1, which asked if a team got more than 17.5 wins in a season and based on that, put teams into the Middle or Top 5 status. While the gini for the “Middle” status remained fairly high, the gini for “Top5” was already quite low considering our tree had only a depth of 1. My feature importances indicated that wins (40%) and losses (30%) were the most important predictors of a team's success, followed by goals for (ca. 15%) and goals against (ca. 15%). Draws only contributed a very small percentage to the model. Therefore, my analysis showed that wins predict a team's status much better than draws, despite draws also giving teams a point.

 ![image](https://user-images.githubusercontent.com/67696969/232373379-9f8ce776-61fe-4842-9744-8fcbc4e5bb38.png)


## Conclusion

This project provided valuable experience in utilizing decision tree models for business problem-solving and highlighted the importance of feature selection and evaluation in machine learning. My features proved to be highly correlated with our dependent variable, making our model a good fit. Further analysis could be done to include additional independent variables to improve prediction accuracy, such as 'Total Team Value', 'Freekicks and Penalties received and conceded', and 'Number of Managerial changes in the season', among others. My visualizations of decision trees helped me understand how my models were making predictions and which features were the most important in determining team outcomes.

## Skills Learned

Through this project, I developed several valuable skills in data analysis and machine learning. I learned how to clean and preprocess data to make it usable for machine learning models, perform feature selection and engineering to improve model accuracy, and evaluate model performance using various metrics. I also honed my skills in using decision tree models and gained experience in interpreting and visualizing results.
