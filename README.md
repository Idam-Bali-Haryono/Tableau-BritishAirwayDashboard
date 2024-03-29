
# FlightScope: The Ultimate British Airways Travel Companion

![plane](https://github.com/Idam-Bali-Haryono/Tableau-BritishAirwayDashboard/assets/115137963/38fcc98c-106c-4b9b-91d4-d226e89a8d56)

## Summary

To figure out which countries and plane models have the best ratings overall, we're doing a detailed analysis. We're looking at things like ground service, cabin staff service, entertainment options, seat comfort, and the overall value provided by airlines. We're focusing on British Airways and similar airlines. Why are we doing this? Well, we want to make smart choices when it comes to spending on luxury travel. These opportunities don't come around often, so it's crucial to get the most value out of them. Once we're done, we'll share our findings through a Tableau dashboard. This dashboard will help me make decisions and also be useful for others looking to pick the best country and plane model based on their needs and preferences. [Want to access the dashboard?](https://public.tableau.com/app/profile/idam7271/viz/BritishAirwaysTravelCompanion/Dashboard1?publish=yes)

## Bacground
Back in October 2023, I treated myself to some first-class bus action, and let me tell you, it's a whole another level compared to riding in economy. The food's better, the service is top-notch, and those seats? Man, they're like sitting on clouds – so spacious and comfy!

As someone who's not rolling in dough, it was a real treat, but I probably won't be doing it again anytime soon. It's just not the most bang for your buck, you know? But cruising in style on that bus got me thinking – what's it like to fly first class? Are we talking major upgrades?

So, I'm diving into British Airways' dataset to suss out which planes are the most chill and where they're jetting off from. Plus, I wanna know which ones have the cushiest seats in the sky.

In order to determine which country and plane model offer the best overall rating, a comprehensive analysis of factors such as ground service, cabin staff service, entertaiment, seat comfort, value provided by airlines originating from those countries particularly those operated by British Airways, is necessary.

This research is key because I don't wanna drop serious cash without knowing I'll be kicking back in luxury. And let's face it, chances are I won't be living that first-class life too often, so I gotta make it count, right?

### Problem Formulation
**Which ones have the cushiest seats in the sky for solo travel in premium class?**

## Workflow
This project utilizes Tableau Public to analyze data, create filters, group information, and design an interactive dashboard. Through careful design and attention to detail, the dashboard provides users with a user-friendly platform to access and interpret information about British Airways, facilitating informed decision-making and enhancing the overall user experience.
### Dataset 

![dataset](https://github.com/Idam-Bali-Haryono/Tableau-BritishAirwayDashboard/assets/115137963/2feb6726-d794-4125-ade3-b6ff75f0fbff)


The dataset under examination comprises reviews spanning from January to October 2023, authored by diverse contributors, and focuses on assessing various aspects of travel experiences. These reviews encompass evaluations of ground service, cabin staff service, entertainment offerings, seat comfort, and perceived value, utilizing a scoring system ranging from 1 to 5 and there is a overall rating column with scoring system ranging 1-10. access the dataset

### Making Filters
In our pursuit of identifying the most exceptional countries and plane models, we recognize the importance of various factors such as ground service, cabin staff service, entertainment offerings, seat comfort, and overall value. Additionally, we acknowledge the significance of seat class preferences, ranging from business class to economy, premium economy, and first class. Therefore we've developed a versatile metric selection filter within our Tableau dashboard. This filter allows you to tailor your analysis based on your specific preferences and priorities. Here's how it made: 


#### pick a metric!
![filter2](https://github.com/Idam-Bali-Haryono/Tableau-BritishAirwayDashboard/assets/115137963/4ddd2200-12a9-413d-97e9-b541fa119f38)


This filter empowers you to choose the variable that matters most to you when making your decision. To create this filter, we've incorporated a blank parameter below


![filter 3](https://github.com/Idam-Bali-Haryono/Tableau-BritishAirwayDashboard/assets/115137963/6673c11e-dc29-4b77-9922-b555a2cc53e3)


an then we connected to the relevant columns in our dataset using the following code:
```
CASE [Pick a Metric]
WHEN 'Overall Rating' THEN [Rating]
WHEN 'Cabin Staff Service' THEN [Cabin Staff Service]
WHEN 'Entertaiment' THEN [Entertainment]
WHEN 'Food' THEN [Food Beverages]
WHEN 'Ground Service' THEN [Ground Service]
WHEN 'Seat Comfort' THEN [Seat Comfort]
WHEN 'Value' THEN [Value For Money]
END
```
#### Enter Seat Type
 ![seat](https://github.com/Idam-Bali-Haryono/Tableau-BritishAirwayDashboard/assets/115137963/b04ba4e5-3bf8-405d-a214-9ee4a8f38324)

 
This filter enables you to specify your preferred seat type, ensuring that your analysis considers your seating preferences. Creating this filter is straightforward - simply drag the 'Seat' column into the filter box.
![seat2](https://github.com/Idam-Bali-Haryono/Tableau-BritishAirwayDashboard/assets/115137963/44f0271f-0d70-4544-900b-b2e4d859ef7c)



### Grouping Aircraft Model  
in this dataset, there are 149 diffrent types of aircraft model reviewed

![grouping2](https://github.com/Idam-Bali-Haryono/Tableau-BritishAirwayDashboard/assets/115137963/1423ac8d-fdb2-42d9-981c-40d4fcc8ebf5)


to make it representable, the aircraft model that have below 50review grouped into 1 group named 'Other'
![grouping3](https://github.com/Idam-Bali-Haryono/Tableau-BritishAirwayDashboard/assets/115137963/9bb9808c-1513-4d60-b98e-234cacc48e46)


### Layout
to make it interactive and cool, the average score by country using geographycal style

![layout2](https://github.com/Idam-Bali-Haryono/Tableau-BritishAirwayDashboard/assets/115137963/4001d13b-429e-4a9a-973e-7102fdc35755)

while the average score by plane model using heatmap style to make it compact and blend with the other graph.

![layout](https://github.com/Idam-Bali-Haryono/Tableau-BritishAirwayDashboard/assets/115137963/ff84b49c-043c-4571-a1a8-34e0d2f1a052)

## Conclusion
In conclusion, following the application of **my specified preferences in created dashboard, Bulgaria, Chile,   Romania, and Senegal emerge as preeminent destinations for luxury travel, showcasing a flawless flying score of 5/5. Meanwhile, the Boeing A380 aircraft, distinguished by its commendable rating of 4.1/5**, establishes itself as the premier selection for discerning passengers desiring unparalleled opulence and comfort during their aerial journeys. **In addition, for all travelers with different individual preference could use this dashboard to get comprehensive information.**

   
