
## Team Name and Members

Team Name: 21479_2

Team Members:

* [@CarsonHall](https://github.com/carsonehall15/21479_2)
* [@Jacob Hoover](http://GitHub.com/Jakehoov1/SQLGroupProject)
* [@Ryan Restino](https://github.com/rrestino/Ryan-Restino-MIST-4610-Group-Project-1)
* [@Mason Sprinkle](https://github.com/masonSprinkle/21479_2_Mason-/blob/main/README.md)
* [@Owen Swonger](https://github.com/ocs08576/21479_2)



## Business Description

The industry that our team is focusing on is the film industry.
The specific aspect of the film industry that we are looking
after is the distribution, budgeting, and awarding of a film
after it has been created by the studio. This process is usually very convoluted and spread thin across many parties, while our model consolidates and simplifies many of these processes. We provided two improvements that will allow the studio to better understand how the film is being distributed and the performance of the film. With these improvements, our project looks at both the qualitative and quantitative aspects of a film after production to see, overall, how well the film did.

    Improvements:
        1. The first improvement we made was to develop a way 
        for the studio’s to track contract details by storing
        the information in a database rather than contract
        details just being on paper or on various files held by
        different people. This allows for everyone to access
        the same details in the database. This makes seeing
        where the film rights are going much more convenient
        and easier to track the performance of the
        distribution. 
        2. The second improvement we made was to add a way for
        the companies to track the distribution of films to
        streaming services. With the rise of streaming
        services, films are no longer only distributed to
        cinemas to be shown in theaters. This was a key
        addition as it will help the studios to accurately
        track the distribution rights of the various films they
        have. This can be seen later as the StreamingServices
        entity in our data model.


 
    
## Data Model
![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/254805237a59ecfc223e16e3f7165fc65e38f0ad/Data%20Model.png)


## Data Model Description

As stated earlier in our business description, the specific aspect of the film industry that we are looking at is the distribution, budgeting, and awarding of a film after it has been created by the studio. The relationships between the entities are important to understand since they are the basis for how we are able to conduct queries and investigate various aspects of the company. 

    ONE TO MANY RELATIONSHIPS: 
    1. A Country has many Studios 
    2. A Studio has many Films 
    3. A Film have many Expenses
    4. A Film can have many Budgets 

    MANY TO MANY RELATIONSHIPS:
    1. Films have many Genres but a Genre has many Films 
    2. Films can have many Awards but an Award can also 
        be won by many films
    3. A Film can have many Cinemas and Cinemas can have many
        films resulting in the associative entity of
        ContractDeals
    4. A Film can have many StreamingServices and 
        StreamingServices can have many films resulting in the 
        associative entity of ContractDeals




## Data Dictionary
![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/Data%20Dictionary4.png)
![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/Data%20Dictionary3.png)
![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/Data%20Dictionary2.png)
![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/Data%20Dictionary.png)






## Query #1 : Write a query that displays each film's filmTitle and expense amount for the film's production department. 

This query is relevant to management because it allows them to see how much financial resources the production department is using. Tracking expenses is a key part of business to allow the company to see where they can cut costs.

![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q1.png)

![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q1%20Results.png)




## Query #2: Write a query to list the filmName and total expenses for that film if expenses are greater than or equal to $4000.

This query is relevant to management because it allows them to see the total amount of expenses incurred by each Film for films that have larger expenses.


![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q2.png)

![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q2%20Results.png)

## Query #3: Write a query to see how over budget a film was based on if total expenses are greater than the budget.

This query is relevant to management because it allows them to see whether or not the film is staying on the right track financially or if it was over budget. 


![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q3.png)

![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q3%20Results.png)
## Query #4: Write a query to list the budget of films that have won 2 or more awards.

This query is relevant to management, because it would be beneficial to see if there is a correlation between the amount of money spent on producing a film and the amount of awards those films win. 

![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q4.png)

![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q4%20Results.png)
## Query #5: Write a query to show the amount of different films that a studio is producing (group by studio name). 

This query is relevant because it allows the user to see the exact number of films that a studio may be producing at a given time.


![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q5.png)

![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q5%20Results.png)
## Query #6: Write a query to list the average revenue of each genre produced by our studio.

This query is relevant to management because it would be beneficial to know which genres of film are on average the most successful financially and which genre’s may struggle more financially on average. 

![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q6.png)

![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q6%20Results.png)
## Query #7:   Write a query that lists out filmName and totalRevenue for films that have total revenue less than the average total revenue of films from the same genre.


This query would be relevant to management because it allows them to see which films are underperforming for their genre.



![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q7.png)

![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q7%20Results.png)
## Query #8:Write a query to see which films do not have contract deals.


This query is relevant to management, because it will allow them to keep their contract negotiations organized and see which films need to be prioritized. 

  

![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q8.png)

![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q8%20Results.png)
## Query #9: Write a query to see the average distribution percentage of each Cinema company.


This query will allow management to see which Cinema companies they typically get the best deals with and use that information to negotiate going forward. 


![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q9.png)

![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q9%20Results.png)
## Query #10: Write a query to list which specific budget was allocated the most amount of money along with that budget’s corresponding filmTitle. 


This query is relevant to management because it will allow management to see which particular budget required the most amount of money spent. They then can use that information to determine if there was any correlation to that budget’s impact on the film. 


![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q10.png)

![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/TP_Q10%20Results.png)
## Features Covered In Queries

![App Screenshot](https://raw.githubusercontent.com/carsonehall15/21479_2/main/Query%20Matrix.png)



