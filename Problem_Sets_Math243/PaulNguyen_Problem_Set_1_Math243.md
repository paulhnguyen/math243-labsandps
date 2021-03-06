Problem Set 1
================
Paul Nguyen

------------------------------------------------------------------------

### Chapter 2 exercises

1a. Here, a flexible statistical learning method would be better than an inflexible method. My reasoning behind this is that with a large n and a small p, the large n will help prevent overfitting from the flexible model. 1b. With an extremely large p and a small n, here, it would be better to have an inflexible method than a flexible method. It would be very easy to overfit our model with a super flexible method. 1c. Here, a more flexible method would fit the data better than an inflexible method because the relationship between the predictors and respons is highly non-linear; an inflexible method will not capture the non-linear relationship, not sensitive enough. 1d. If the variance of the error terms is extremely high, we may need to make our method less flexible, as the flexibility is causing our variance to shoot up. The method is fitting too closely,

2a. This scenario is a regression problem and we are most interested in inference. n = 500, p = 4 2b. This scenario is a classification problem and we are most intersted in prediction. n = 20, p = 14 2c. This scenario is a regression problem and we are most interested in prediction. n = 52, p = 4

4a. My first application in which classification might be useful is if we are trying to determine what state a reedie is from. We can use whether or not they have a car as a predictor, and then if they do have a car, then use what license plate they have. We can also look at language specific predictors such as accents/slang. The goal of this application is prediction because we are trying to find out something new in the response based on these variables and not try to understand the relationship between the predictors and response. Another classification application could be to try and see what variables are most important when it comes to being an A/B student or a C/below student. The response here is the student's grades, and some predictors could be: time spent on homework and studying, whether or not they live on campus, their high school grades, hours of sleep student is getting a night. This would be an inference application because we aren't predicting anything, but we are trying to understand the relationship between our variables. Another classification application could be the government deciding if a road is safe for driving, or if they need to fix it or put warning signs. The predictors for this scenario can be number of accidents on the road, weather conditions, and when was the road last repaired or painted. This would be a prediction application because the government here is determining something based on the variables and not looking at the relationship between them.

4b. One real life application where regression would be useful is predicting a child's fully grown adult height. Some predictors for this can be how much sleep the child is getting, the child's weight, the child's parents height, or any of the child's siblings heights. Here,the goal of this application would be prediction, as we are trying to predict something in the future and not study the relationships between two variables. Another real life application could be predicting amount of precipitation a certain area will receive the next day. Some predictors for this can be humidity, max temperature the next day, min temperature the next day, and previous trends in the weather. Here the goal of the application would be prediction; we are trying to predict something based on some variables. One last application for regression can be seeing what variables are most important to see how many people visit your restaurant. Some predictors of this can be temperature, whether or not it is raining, location of your restaurant, or rating on the internet. This would be an inference, because we are trying to determine the most important variables to see which one impacts the response (how many visitors) the most. 4c. One situation where cluster analysis might be useful is looking at a DNA strand and seeing the location of certain genes to try and find out the cause of a certain disease. Another application can be identifying where people live in order to see where the most populous areas of the world are. We can also use cluster analysis to see what trends are becoming very popular; we can look at what the most popular phrases are on twitter and see what people are talking about... for example, everyone is talking about a certain tv show.

1.  The advantages of a very flexible approach is that this method will be very good at fitting the data that we have to the estimate. However, using a flexible method may lead to overfitting of the model and will increase the variance by a lot. With an inflexible method, you won't have to worry about a super high variance or about overfitting, but the method may be too simple to capture the trends of the data and introduce bias into the model. I think a flexible approach may be better with a large amount of n to reduce variance, or if the trends in the data are complicated. A more inflexible approach may be better when n is small, so we avoid overfitting, and when the data present relatively simple trends, for example a very linear one.

2.  The benefit of using a non-parametric approach is that by avoiding assuming a particular functional form for f, they have the potential to have a wider variety of possible shapes for f. They do not make any assumption about the form of f. However, they do not help estimate f by reducing to a small number of parameters, so we will still need a very large n to estimate f accurately. It is easy using the parametric form to estimate using certain parameters, than it is using a random f, but it may not fit the unknown form f perfectly.

### Additional exercises

Using the notation standards described at the end of chapter one, please provide notation for the following objects:

    Input: The 10 photos that we looked at on the first day, as if they were scanned at 64 x 64 pixel resolution.
     (bold)A ∈ R^(64×64)
     (bold)B ∈ R^(64×64)
     (bold)C ∈ R^(64×64)
     (bold)D ∈ R^(64×64)
     (bold)E ∈ R^(64×64)
     (bold)F ∈ R^(64×64)
     (bold)G ∈ R^(64×64)
     (bold)H ∈ R^(64×64)
     (bold)I ∈ R^(64×64)
     (bold)J ∈ R^(64×64)

Transformed Input: The 10 photos, after a small number of features have been identified. (this x is in lower case bold) x*A = (x*A1 x*A2 x*A3) (repeat 9 more times, replace A with B,C,D,E,F,G,H,I,J)

Output: The associated actual ages of those 10 photos. yA, yB, yC, yD, yE, yF, yG, yH, yI, yJ Model: Provide a guess at what (f) might look like (there is no single right answer here). I think that the model will look something like f(x) = B0 + B1xA1 + B2xA1^2 + B3xA2 + b4xA2^2 + B5xA3 + B6xA3^2 + e I don't think I got the notation correct, but I was thinking a parametric method with polynomial regression with different features xA1, xA2, . . . for however many features we deem proper, along with an error term
