﻿# ARMUTARLRecommender
About the Dataset

This dataset originates from Armut, Turkey’s leading online services platform that connects service providers with customers seeking various services, including cleaning, renovations, and moving, all accessible through a few taps on a computer or smartphone. The dataset includes records of customers who have used Armut’s services, capturing details about the services and their associated categories.

Each entry represents a specific service transaction, with the following information:

#UserId:# A unique identifier for each customer.
#ServiceId:# An anonymized ID representing specific services within categories (e.g., couch cleaning under the cleaning category).
#CategoryId:# An anonymized ID representing broad service categories (e.g., cleaning, renovations).
#CreateDate:# The date and time the service was ordered.
Given that some ServiceIDs represent different services depending on their CategoryID, a new "Hizmet" (service) variable is created by combining ServiceId and CategoryId, making each service unique within its category.

The dataset lacks a traditional "basket" or "invoice" definition. To apply Association Rule Learning (ARL), we define a basket as the set of services a customer purchases within a single month. Each unique combination of UserId and YearMonth forms an ID to represent monthly transactions.

Using ARL on this dataset, we aim to develop a service recommendation system for customers based on frequently purchased service combinations. This system can help Armut provide targeted service suggestions, enhancing the customer experience and promoting service diversity on the platform.
