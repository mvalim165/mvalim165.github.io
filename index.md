---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: "Cycling in Helsinki: 2015 vs 2022"
---
Explainer notebook: https://github.com/mvalim165/mvalim165.github.io/blob/e5bfcf573d9e12f9f8dc7cb3a73b93acfef64053/Explainer_notebook_Group1.ipynb
## Introduction
There has been a decrease in cycling accidents in Helsinki, as shown by the following graph. The data only includes accidents reported to the police, so the data is far from comprehensive. The absolute values are to be taken with a grain of salt but the the overall trend is so stark that it is fair to assume that the city has become more safe – at least in some way – for cyclists. Though as shown in the smaller plots on the right, the number of lethal accidents varies from 0–2 throughout the years. These severe accidents are all included in the data.
<iframe src="/Reported_cycling_accidents_in_Helsinki.png" width="1400" height="850" frameborder="0"></iframe>

The accident numbers are obviously strongly influenced by the amount of people cycling. However those numbers are difficult to capture and again influenced by several factors besides safety, e.g. how cycling compares to other means of tranport (walking, public transport). To investigate the decrease in accident numbers, we looked into several datasets. Information on the reachability of public transport stations was available from years 2015 and 2022, thus these two years are studied. To assess the cyclist numbers, we present analysis based on automatic traffic counters as well as synthesis from bi-annual barometer questionnaires. The closest years available where 2016 and 2022. From the same questionnaires, we could also extract citizen insights on public transport and safety in relation to cycling.

## Public transport and light traffic

<iframe src="/data/bike_15min_map.html" width="1400" height="550" frameborder="0"></iframe>
Looking at the map shows us that the most densely populated parts of Helskinki appear to have gotten more access to public transport. This can be seen in the map through the intensity of the yellow, region in the city center. In 2022 this yellow is much more intense than in 2025. Additionally, the coverage areas do seem to have spread out a small bit in 2022 as compared to 2015. One important thing to note is that the vast majority  of the residential areas appear to be within 15 minute bike ride to a station. We believe this could be a factor that feeds into the prevelance of biking in Helsinki. In addition, the increase in the number of stations that can be accessed means faster travel times to different regions in Helsinki. We believe this is critical because one of the advantages of cars to public transport is that with a car you can typically take a very direct route to your destination, whereas with public transport you are at the whim of the route. This ties back to how likely people are to cycling because if you can get to just about anywhere relatively quickly and you only had to bike 15 minutes, then you would have more people buying bicycles and rididng them to and from bus stages.

<iframe src="/data/bike_15min_counts.html" width="1400" height="550" frameborder="0"></iframe>

Looking at the data in this format yields more clear insights that might be difficult to read on my map. It's important to note that because the borders are not perfect, the 0 column is going to appear inflated, but the real number is much lower. That being said, it's still true that over half the city can reach a bus stop or train station in a 15 minute bike ride. Additionally, aside from 0, it appears most places in Helsinki are 15 minutes from not 1 but 3 or 4 stations/bus stops, which I've explained earlier why this is a good thing. Additionally, the number of places in Helsinki which were already dense have become denser, while the areas which had 2 or 3 sattions likely increased their coverage/density to 4. Finally, it's clear to see that the density has increased in the city center. One thing to note is the lack of increase in coverage as in 2022 there has only been a decrease of 34 areas without the access to a train station or bus stop from 2015. Helsinki should invest in spreading coverage of the public transportation network, then also increasing the amount of areas in which 3/4 stations are reachable by a 15 minute bike ride.

<iframe src="/data/walk_10_min_map.html" width="1400" height="550" frameborder="0"></iframe>

Looking at the walking numbers is a bit tricky because we think if you can walk you will walk over biking. That being said I do think this yields interesting results. Firstly looking at the number of stations reachable by 10 minute walk in 2015 vs 2022 chat map, what I immediately noticed is in the city center there's a large region where you are likely to be in an area of which you could chose between 1 of 3-5 train station/bus estacians. Someone who lives in a place like this we believe is actually de-incentivized to cycle as the entire city is reachable with a short walk. If the government wants to increase the amount of cyclist, they should invest in expanding the network so it revolves less strongly around major roads, as clearly demonstrated in the above graph, rather than increasing the density of the city center

<iframe src="/data/walk_10min_counts.html" width="1400" height="550" frameborder="0"></iframe>

Looking at the count reveals something we found interesting-- the coverage has increased, likely leading to a decrease in the amount of people who cycle. Additionally it does seem that the density has also increased, which would also lead to a decrease in the amount of peolpe who cycle. 

## Cyclist numbers and accidents

Estimating cycling numbers is not a simple task. The automatic counters, located currently in 20 locations around the city are one way to estimate where and in which volumes the people of Helsinki cycle. For our focus years 2015 and 2022, there was limited overlap on counters in use and at least nearly full year time series. That and efficient differences in locations were the reasoning behind showcasing only *the* *seven* *locations* below. 

As the counters are at static locations, changes in cyclist amounts can be due to several different reasons and might not capture general changes in cycling habbits. To put it bluntly, there might be the exact same amount of cyclists on the street but just on the other side of it. All cicty cyclists probably know how one switches routes if there is e.g. a consturction site somewhere. 

To account for these shortcomings, data from the barometer is presented in tandem. The 8th subplot shows percentiles of respondees who (1) own at least one bicycle and (2) cycle at least sometimes.  
<iframe src = "/cyclist_counters_subplotgrid.html" width="1800" height = "800" frameborder="0"></iframe>

Based on these graphs it appears that there has been no major change in amount of cyclists in recent years. However, the proportion of bike owners has decreased. Funnily enough, the quite popular and well-functioning city bike system was launched indeed in 2016. Our comparison captures how cycling in Helsinki no longer requires owning a bike. Besides the obvious influence of weather, the city bike season from April to October also explains the seasonal differences in counter numbers in 2022. One could speculate that this explains the 20–30k inrease in cyclists on Baana, a key route through the city center that is seperate from car traffic. To understand this better, the city bike data available should be analysed, but that is beyond the scope of this project. A funny Finnish fact: Most people have their summer holiday in July. You can see the temporal mitigation to summer houses in the cyclist numbers. 

Considering the locations, it becomes clear though that the bike traffic is very concentrated in the city center, with locations such as just mentioned 'Baana' and 'Hesperia park (the Opera)' hosting the highest numbers both in 2016 and 2022. In the following map, these locations are shown with the accident locations.

<iframe src = "/bike_accidents_map.html" width="1400" height = "800" frameborder="0"></iframe>

The heatmap captures the varying locations of the accidents. The level of randomness in locations is to be accounted for, but several hotsopts, for example in Punavuori and along Mannerheimintie have disappeared. These could indicate that the bikelanes have been improved. The survey data from 2016 and 2022 aligns with these observations on safety: the percentages of respondents that perceive cycling at least quite safe has increased from 74 % to 82 %.

## Conclusion

To cycle or not to cycle... Individual's decision on whether to hop on a bike or not depends on several factors, not only safety. The graph below showcases these factors:

<iframe src = "/Why_not_cycle.png" width="1400" height = "900" frameborder="0"></iframe>

This graph clearly offers answers to some of our questions. Respondents prefer something else: walking, driving or public transport. This change could be partially due to improvements in reaching public transport, as presented in the first part of this story. Similarly long distances are not as big of a problem anymore – maybe because combining public transport with cycling is easier? 

Related to accidents, the graph also hints towards people feeling more safe in the traffic: feelings of unsafe are more rare. However, poor route planning, meaning e.g. illogical or discontinous routes, have stayed consistently annoying.

Based on our analysis it seems that slowly and steadily, Helsinki is becoming more pleasant and safe city for cyclists.