---
layout: post
title: Wildfire Watch
subtitle: Get updated alerts for wildfires within a custom radius of your home
---

[Wildfire Watch](https://wildfirewatchapp.com/) helps Americans be prepared for wildfires in their area.

Users can save multiple locations by address and set a custom radius for each location. Wildfire Watch will notify users of any wildfires near their saved locations.

I created a Flask API that routinely checks for updates on wildfire locations by accessing InciWeb's Wildfire RSS Feed. The API takes positions as requests and returns a list of fires near that location.

This project will be passed down to another team in Lambda School, so I created a data pipeline that records MODIS active fire and weather data. This data is then labeled using InciWeb's RSS feed.

Once the pipeline collects enough data with confirmed fires, we'll be able to use the data to train a predictive model.

My main responsibilities on the project:
  * Created Flask API to process and relay data the the backend of our app
  * Created an ElephantSQL instance to connect to our data pipeline
  * Labeled historical data for machine learning
  
Check out our codebase on the [Wildfire Watch Github Repo](https://github.com/Lambda-School-Labs/forest-fire-watch-ds/tree/staging_labs17)! My most recent work is in the `staging_labs_17` branch.
