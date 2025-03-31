---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: "Assignment 2: a Data story"
---
The data that has been curated for this assignment is the San Francisco Police Department Incident Report dataset. This dataset starts in 2003, and we cut the data off at 2024. There are a lot of fields in the dataset, however the most important field we'll be looking at in our analysis is the Category field, which tells you which crime they committed. There are also temporal data that records the date and time the incident was reported it was taken and geospacial data like lat/long coordinates. Each entry will also include the police department district, or neighborhood. <br>
<br>
![Graph 1](https://raw.githubusercontent.com/mvalim165/mvalim165.github.io/refs/heads/main/overview.png)
In the graph above, we observe the proportion of all crimes committed that were drug/narcotic offenses. California Prop 47 passed in 2014, as annotated in the graph, leading to less police enforcement on drug and narcotics offenses[1]. While there is a larger trend before 2014 of less drug/narcotic incidents reported, one can reasonably assume this very important change in the law at least contributed to the continuation of this trend. In 2017, Fentanyl arrived in San Francisco and started to proliferate through the community, resulting in the spike from 2017 to 2018. The other large spike occurred when the new district attorney entered office in 2022. At this point, fentanyl was ravaging communities in San Fransisco and became a larger voter issue. As such the new District Attorney wanted to crack down on fentanyl, which raised police's likelihood of recording incidents which involved people who did or had consumed fentanyl, or were in possession of fentanyl. This crisis has gotten so bad that the Mayor has declared a state of emergency due to the drug's impact just last month [3]. This will have ramifications for the amount of money that different departments within the police department get, as well as the general culture of San Francisco police in terms of which offenses they prioritize, which is why analyses such as these are important.

[1] *Lopez, G., Katz, J., & Parlapiano, A. (2024, January 31). Can San Francisco Solve Its Drug Crisis? Five Things to Consider. The New York Times. https://www.nytimes.com/2024/01/31/upshot/san-francisco-drug-crisis.html?unlocked_article_code=1.7E4.a6XJ.QIxTydwlDGAL&smid=nytcore-ios-share&referringSource=articleShare* <br>
[2] *Carlos, C. (2025) San Francisco mayor Lurie Signs Fentanyl state of emergency ordinance; unveils ‘Stabilization center’ in tenderloin, CBS News. Available at: https://www.cbsnews.com/sanfrancisco/news/fentanyl-state-of-emergency-san-francisco-mayor-daniel-lurie/ (Accessed: 31 March 2025).*<br> 

Our crime data included only recorded crimes and especially since the decriminalization actions in 2014, that number does not perfectly capture the overdose crisis in the city. By looking at the spatial distribution, fentanyl's presence becomes more evident.

<iframe src="/sf_districts_bokeh.html" width="100%" height="600" frameborder="0"></iframe>

The drug-related crime has become increasingly unevenly distributed, which is showcased in the interactive figure above. By looking at the yearly district distributions, the focus on just a few districts is clear. Since 2020, over 50 % of drug-related crime has been recorded in Tenderloin.

To understand this location even better, the map below offers more insights: