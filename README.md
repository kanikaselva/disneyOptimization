# **Let it Queue**

# An Optimization Framework for Theme Park Ride Scheduling

### Problem

Planning a day at a theme park can be challenging for visitors who want to experience as many rides as possible. Long lines, walking distances between attractions, and fluctuating crowds make it difficult to navigate the park efficiently. This project’s goal is to minimize wait times while maximizing the “fun values” achieved in a day by finding the ideal sequence of rides to visit.

### Why Dynamic Programming

In the theme park scenario, the environment is unstable since the waiting time for each ride in each hour is not fixed. Fortunately, we have enough data informing us about the change process of waiting time that allows us to adopt Dynamic Programming, which globally optimizes the whole day plan instead of just finding the next optimal ride.

### Data

We used the dataset from touringplans.com (2018). The dataset includes the information on waiting times, ride durations, holiday seasons, ticket seasons, and other factors for multiple rides across parks at Disney World (5 rides from Disney’s Animal Kingdom, 4 from Hollywood Studios, 3 from Magic Kingdom, and 2 from Epcot). Our data folder includes the following files:

1. touringplans_2018: Wait times for each ride based on what’s posted at the queue by the hour, actual wait time for each ride
2. Attraction_metadata: Average wait times for each ride, park location, and duration of ride
3. Parks_metadataraw: how long each theme park was open for a particular day, designated holiday season (if any), events, EMH (Extended Magic Hours) availability for each park, forecasted temperatures, school sessions for particular regions, ticket season (peak, regular)

### Installation Guide

To effectively run all the files, please ensure that the following libraries are downloaded in your local environment:

* pandas
* numpy
* sklearn

As for the files, run them in the order stated under the folder code, starting with '0. cleanData.ipynb' and ending with '5. greedyOptimization.ipynb'.
