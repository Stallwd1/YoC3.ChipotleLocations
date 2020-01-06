# YoC3.ChipotleLocations
Year of Coe: Day 3 | Where to Open a Chipotle Location?

Today's coding challenege followed another Datacamp project resource. The company's ability to guide users through the project allows you to really understand how to approach a data science problem.

In this project, the tidyverse [a very common and useful R package] is again used, in addition to the leaflet, leaflet.extras, and sf packages. As we know from yesterday's project, tidyverse is mainly used to 'tidy' the dataset and prep it for data model. The new packages [leaflet & sf] are being used to find potential loications for new Chipotle locations. The maps generated in this project are using the leaflet package, which paired with the sf, which allows the user to easily encode spatial vector data, can produce simple yet powerful visualizations.

The main preparation stages in this project revolved around filtering the data according to Chipotle locations that were closed [TRUE] and those that were open [FALSE]. By subsetting the data in this manner, the spatial maps generated can drive the questions:

- Where have Chipotle locations been closed?
- Where have there never been any Chipotle locations?
- How near/far is another Chipotle location?
- Where should open our next location?

After using these questions to guide the project, the main approach is to narrow down the states that have very few or zero Chipotle locations. These are deemed a better business strategy as they offer a new, untapped revenue source.

The subsetting leads us to see that South Dakota has not had any Chipotles opened in the state. We then use South Dakota' population dataset to reveal the population density across the state [We dont want to open a location up if there isnt enough people to but!]

We then use two counties that have been identified as 'suitable' candidates [Sioux Falls and Rapid City]. We use a 100 mile radius to plot a radius around the two proposed locations to view if any overlapping areas exist betwen inter- or intra-state locations.

The Sious Falls locaiton does seem to have a location within the specified 100 mi radius, deeming that Rapid City proves to be a better fit for our needs.

...

If you have any questions regarding my write-up or have any corrections regarding my communicated analysis, please feel free to contact me!
