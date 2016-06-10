---
layout: post
title: How slow was the 2016 Vermont City Marathon?
---

The 2016 edition of the Vermont City Marathon was stopped for the first time ever at 3 hours and 58 minutes into the race due to [extreme heat](http://www.vermontcitymarathon.org/news/letter-from-runvermont-executive-director/). Anyone who had the pleasure of running and watching the event knows that it was a [tough](http://levelrenner.com/2016/06/04/duhon-overcomes-heat-deep-vcm-field/) [race](http://levelrenner.com/2016/05/31/pelletier-repeats-for-the-2nd-time/).

Many people had goal times they failed to achieve, as the primary focus given the conditions was finishing. So I wondered, how much did the weather conditions impact race times. Or to put it the other way, how much faster could you have run on a 'normal' VCM day (as if there was such a thing as a normal spring day in New England).

To do this, I looked at the number of runners under different time thresholds (3 hrs, 3:30, 4:00, 4:30) in 2016, and then compared this to the simulated distribution of finishers under each time threshold based on data for the previous 5 years. The results are telling; the number of finishers under each time threshold in 2016 (the red line) is well lower than the expected distribution (blue area).

![](..img/vcm_2016/gsim-1.png)

To determine how much slower 2016 was due to the temperature, I found the time in 2016 for the finishing place at each time threshold in the previous years. For example, in 2015, 92 runners finished under 3 hours, and in 2016, the time for the 92nd finisher was 3:11:53. Using this data, I then calculated the percent time difference between the Xth finisher in each year. For the example I just gave, the 92nd finisher in 2016 was 7% slower than the 92nd finisher in 2015.

I grabbed hourly weather data from wunderground for each race day, and using this data I fit a statistical model using the temperature at 10am (2 hours into the race) to predict how much slower the average runner's pace was in 2016, 81C at 10 am, then if the race had been at cooler temperatures.  


This table shows that a 3 hour marathoner was ~5% slower in 2016 than if the race temp had been 60C, and ~7% slower than if the temp had been 50C. This may not seem like much, but for a 3:30 marathoner (8 min/mi pace) they would slow to 8:33 min/mi pace, or a 3:44 marathon. Bummer.

I also noticed that the percent pace slowdown was less for faster runners, which makes sense as they spend less time out in the heat, and their generally higher marathon fitness may have allowed them to perform better given the conditions.


Time       Temp at 10am   Percent Slower
--------  -------------  ---------------
2:30:00              50              3.4
2:30:00              60              1.8
2:30:00              70              0.1
3:00:00              50              6.8
3:00:00              60              5.2
3:00:00              70              3.6
3:30:00              50             10.3
3:30:00              60              8.7
3:30:00              70              7.1
4:00:00              50             13.8
4:00:00              60             12.2
4:00:00              70             10.6


Hopefully this provides some consolation to runners out there that yes, they could have gone faster if it had been a cooler day! Better luck next time!
