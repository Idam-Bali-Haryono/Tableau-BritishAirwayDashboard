# Tableau-BritishAirwayDashboard

## Summary

**In pursuit of discerning the countries and plane models with the most favorable overall ratings**, a thorough analysis encompassing diverse factors such as ground service, cabin staff service, entertainment offerings, seat comfort, and the value proposition provided by airlines, particularly those under the auspices of **British Airways**, is imperative. This project endeavor is motivated by the need to make informed decisions regarding potential expenditures on luxury travel experiences, recognizing the infrequency of such indulgences and the importance of optimizing their value. **The conclusion of this analysis will be presented through a Tableau dashboard, enabling not only my decision-making process but also serving as a resource for others to evaluate and select the most suitable country and plane model according to their specific criteria and preferences.** acces the dashboard


## Bacground
Back in October 2023, I treated myself to some first-class bus action, and let me tell you, it's a whole another level compared to riding in economy. The food's better, the service is top-notch, and those seats? Man, they're like sitting on clouds – so spacious and comfy!

As someone who's not rolling in dough, it was a real treat, but I probably won't be doing it again anytime soon. It's just not the most bang for your buck, you know? But cruising in style on that bus got me thinking – what's it like to fly first class? Are we talking major upgrades?

So, I'm diving into British Airways' dataset to suss out which planes are the most chill and where they're jetting off from. Plus, I wanna know which ones have the cushiest seats in the sky.

In order to determine which country and plane model offer the best overall rating, a comprehensive analysis of factors such as ground service, cabin staff service, entertaiment, seat comfort, value provided by airlines originating from those countries particularly those operated by British Airways, is necessary.

This research is key because I don't wanna drop serious cash without knowing I'll be kicking back in luxury. And let's face it, chances are I won't be living that first-class life too often, so I gotta make it count, right?

### Problem Formulation
**Which ones have the cushiest seats in the sky?**

## Workflow
### Dataset 
The dataset under examination comprises reviews spanning from January to October 2023, authored by diverse contributors, and focuses on assessing various aspects of travel experiences. These reviews encompass evaluations of ground service, cabin staff service, entertainment offerings, seat comfort, and perceived value, utilizing a scoring system ranging from 1 to 5. access the dataset
### Import .csv to Tableau
### Preprocessing
### Making Filters
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
### Grouping Aircraft Model  
### Layout
## Access Dashboard 


   
