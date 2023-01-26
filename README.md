# Car insurance client

Our client, a multinational insurance company, has requested us a new project: they need a service that helps to predict 
the car claims on a monthly based using the data they have from their insurance policies (a mix of car information, client
and the policy itself).

There are two final goals: 
1. provide a price rise on the policy to those models that are likely to be claimed
2. filter out new clients/policies for cars that are likely to have a claim in the next month. 

There are no data science team in the client but there are a couple of engineers from the client interested in the field. 
They have suggested us to use logistic regression to classify the policies as: **normal** and **likely to be claimed**. 
They do not have a clear idea on the way to do it so they need our support. 

The engineers have provided us with one dataset (`last_month_data.csv` in this repo) from last month where the policies with claims are labelled within column called `is_claim`. With 1 if they were claimed 0 if they were not claimed.

Using this data we propose you (as person in charge of the project) to provide a solution to the next tasks:

## **Task 1**: generate a classification model using logistic regression
The first task is to use the data provided to generate a classification model using logistic regression.
Provide most relevant information that in your opinion is needed to understand the performance of such model.

The expectation in this task is to have a jupyter notebook as an outcome with the required steps explained. 

## **Task 2**: generate a classification model of your choice

In this task you can choose your own classification model. Independent of the previous task
we want to present to the client an alternative to logistic regression.

You will have to choose a different classification algorithm and generate a model that *could* perform better than the 
previous logistic regression. Provide also the most relevant information to understand the performance of such model as well
as the information needed to compare it with the previous model. 

The expectation in this task is to have a jupyter notebook as an outcome with the required steps explained. 

## **Task 3**: describe, compare and present the previous models

Provide a presentation with plots about:
- the most relevant information about the data
- the performance about the two previous models
- which are the features that provide more information to the model for its performance for classification

## **Task 4**: generate a simple web service for predictions

Once the model is ready, the idea within the client is to have a service that could be consumed by other services to
obtain whether a given policy would be at risk of generating a claim. For that reason you should provide a small dockerize
application that using one of the previous models can return the class (`normal` or `likely to be claimed`) of a given policy. The data provided to the application to generate a prediction should be the same columns that were provided in the csv.

The expectation in this task is to have a dockerized application that provides an API that can be consumed by a REST client.

## **Task 5**: future ideas

Finally to show to the client that we have a plan for the project, we ask you to present your ideas about: 

- Taking in account that in the next months more data will arrive, How would you evolve the model once in production? Do 
you have any plan for versioning?

- How could the service/model be made resilient to changes in the production environment, such as data format alterations? 

- On which cloud provider will you leverage to serve the previous service/model and why.


## Things we love

- Your ideas and the way you express them (guide us through your thoughts)
- Documentation
- Well formatted code
- Readability of the code
- <ins>Testing!</ins>
- That you feel comfortable
- That you can use your preferred packages during the test


## Final words

Good luck! We hope you enjoy working on this task. And if you need anything at all, please feel free to reach out to us!
