# SFO-Flight-Delays

## Introduction
________
  This project arose out of years of frustration in picking the wrong flights out of the San Francisco International Airport (SFO). I grew up in California with SFO was our main hub for travel, and I have spent more time between those walls and on the tarmac than I care to reflect on. 

  In the future I would like to be able to select flights not only on price but also on whether or not the flight is likely to depart on time. There are a number of factors that influence departure times, only some of which can reasonably be considered with free public data. Perhaps the largest influencer of flight delays is aircraft maintanence, though even if I could access that data I'm not sure it would help much. Presumably airlines are up to their eyeballs in it and they always at least pretend to be surprised when one of the [600,000 odd parts](http://www.boeing.com/farnborough2014/pdf/BCA/fct%20-737%20Family%20Facts.pdf) on the plane is flagged as broken post boarding. Instead, I will examine three hypotheses. 1.  Does poor weather slow down departure times? 2. Do larger flights get runway priority? 3. Are some airlines more or less on time than others?

  The first seems reasonable, since anyone who has been to San Francisco for more than a day or so can attest, we have fog problems. The second comes from my anecdotal experience in trying to fly to Santa Barbara a number of times in small planes that always seem to leave extremely late. The third is purely out of curiosity. I have no specific anecdotal evidence one way or the other but some people that I have asked feel quite strongly about it.

  To test these hypotheses I scraped all of the flights departing SFO in 2017 and most of 2018, hourly weather readings for the airport during the same timeframe, and average cost of a ticket between SFO and the destination city, which is used as a proxy for the size of the flight. 

  Then I explore various classification algorithms to sort flights into on time vs delayed, and then make a prediction on how long the delay will be with a linear regression model trained on previously delayed flights. 
  
 ## Table of Contents
 _________________
 
 ### Data acqusition and processing notebooks
 
 * TransScrape - Notebook to scrape and process departures data from [transtats gov website](https://www.transtats.bts.gov/)
 * FaresScrape - Notebook to scrape and process average fares from SFO to all destination cities. 
 #### More coming: Stay tuned!
