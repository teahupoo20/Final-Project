# FINAL PROJECT by Edwin Pitono and Vinamrata Yadav
# HELLO DOE
Data Analysis Full-Time FEB2021, Paris

Presented on Friday April 2nd 2021

Project Description 
Hello Doe is a startup whose mission is to help companies recruit for student jobs. It uses the social media to market the job offerings in order to get faster response time. The purpose of this final project is to analyze the job market in Paris, France, in order to optimize the conversion rate of the business developper in Hello Doe. If the business developper can find the struggling sector in recruitment on one specific time, by priorizing his efforts to these companies he/ she will have better conversion rate from these clients. In order to organize the efforts and planning, the team also needs an overall view about the job market so they can make projections and plannings. Based on past data, a prediction for the job market in 2021 can also be done.

**Objectives :**

- Visualize the past data of job offer and job requests in Paris. 
- Spot the sectors which struggles to recruit
- Make a prediction for the job market in 2021

**Workflow**

**1. Dataset import**

   API and web scraping from the French Employment Agency website. The website contains data about job offers and job requests from actual and recent years. 
   
**2. Data cleaning, data manipulation and data visualization**

   The challenge with the datasets from Pole Emploi is the size, the redundancies and the datas present multiple dimensions (places, time and professions) which        present some challenge for the visualization
   
                                                RAW JOB OFFERS DATASET 
   <img width="959" alt="Capture d’écran 2021-04-21 à 14 56 18" src="https://user-images.githubusercontent.com/76606558/115557334-e59b3f80-a2b1-11eb-94b7-66865be079e0.png">

   We clean and filter our data. This is the subcleaned, raw data.

                                                JOB OFFERS DATASET AFTER DATA CLEANING

<img width="652" alt="Capture d’écran 2021-04-21 à 14 56 51" src="https://user-images.githubusercontent.com/76606558/115557480-06639500-a2b2-11eb-8ec8-03c7038869c4.png">

   And this one is the cleaned and filtered data ready for visualizations and other manipulations.

   After some manipulation, here's what the data visualization about job offer and demand look like 

                              Visualization of the top 20 job offers in Paris in 2019

![joboffertop20](https://user-images.githubusercontent.com/76606558/116888660-05c0ec00-ac2c-11eb-8da8-07fbeb8d5245.png)

                              Data viz according to the job type :

![jobofferparis19Assistanat commercial](https://user-images.githubusercontent.com/76606558/116888917-49b3f100-ac2c-11eb-98d6-80e00dc705e3.png)

                              We also made a ratio between job offer and job demand to highlight the sector with 
                              the most difficulty to recruit.

![ratio1](https://user-images.githubusercontent.com/76606558/116913288-92c66e00-ac49-11eb-9159-fa1b1526123c.png)

                              Here we can see that "Action sociale" job category has a job offer / demand ratio 
                              of more than 40:1.

![ratio2](https://user-images.githubusercontent.com/76606558/116912979-37947b80-ac49-11eb-8934-269ea3e9a76a.png)

                              We can visualize the plot differently with bubble plot. This plot is made using Tableau.

<img width="346" alt="Capture d’écran 2021-05-03 à 16 46 28" src="https://user-images.githubusercontent.com/76606558/116913108-5c88ee80-ac49-11eb-9ea2-64ea6b6c00ee.png">

**3. Prediction model**

   Our client needed a prediction of the job offer and job request for the coming months to facilitate the business developper's job. We have datasets 2010 - 2020      in job offers. We made a model out of 2010 - 2018 and test it on 2019. We had an overall MAPE of 52.48404702177265 but if we take a closer look our model            predicts with less errors for certain jobs. *The lower the MAPE score the better*
   
   <img width="839" alt="Capture d’écran 2021-05-03 à 16 37 44" src="https://user-images.githubusercontent.com/76606558/116890538-08bcdc00-ac2e-11eb-9aba-2ff01be3af05.png">
   
   Here the MAPE for "Actions sociales" is around 10 where for "Agent de distribution" it is around 323. This could be explained probably by an evolution in the job    industry for those with high MAPE scores and a stable sector for those with low MAPE scores.

   So we took this model to predict 2021 job offer 

                              Job offer prediction for 2021. One data point represents a trimester.

<img width="925" alt="Capture d’écran 2021-05-03 à 16 34 25" src="https://user-images.githubusercontent.com/76606558/116890976-7e28ac80-ac2e-11eb-811a-4467db99e635.png">

   Here we can see a nudge of job offers in the second trimester because model sees this nudge in the past years.


**In conclusion**

With this project, we demonstrated our skills to
-collaborate

-scrape data via api

-clean, manipulate and vizualize complex data

-make a hypothesis and test it

-make a prediction model and evaluate it

-use the domain expertise of our client to make sense of our work


Keywords :

Python, Pandas, FBProphet, Tableau
