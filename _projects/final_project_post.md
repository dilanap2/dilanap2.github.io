---
name: Final Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/images.png
description: In depth analysis of the 2022-23 NBA Season
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# 2022-2023 NBA AST/TOV Analysis

By: Dilan Patel


In the NBA, a great metric to see how good of a playmaker or passer a player is is to look at how many assists they record versus how many turnovers they record. In order to record more assists, you need to pass more, but when a player makes a bad pass, it could turn into a turnover. An assist is when a player passes a ball to a teammate and then the teammate ends up scoring a basket. A turnover is when a player loses posession of the ball to the other team. This might happen when a pass gets intercepted by the other team or when a player throws the ball out of bounds. [this page](https://captaincalculator.com/sports/basketball/assist-turnover-ratio-calculator/#:~:text=Assist%20to%20turnover%20ratio%20puts,an%20indicator%20of%20ball%20control.) can teach you more about what an assist to turnover ratio is. 

The following chart is a scatterplot of every NBA player's asissts and turnovers per game in the 2022-2023 Regular Season:

<vegachart schema-url="{{ site.baseurl }}/assets/json/scatter1.json" style="width: 100%"></vegachart>

This scatter plot in Altair with NBA player's assists per game on the x-axis and turnovers per game on the y-axis can be a useful tool for coaches, scouts, and analysts in evaluating player performance. By plotting these two metrics on a scatter plot, it becomes easy to identify players who excel in assists and minimize turnovers. This can help coaches identify potential areas of improvement for their players or adjust their game plans accordingly. Additionally, scouts can use this graph to identify players with high assist-to-turnover ratios, which is an indicator of good decision-making and ball-handling skills. Analysts can also use this graph to compare players across teams or even across seasons to identify trends in player performance. Overall, this graph provides a simple yet powerful way to visualize and compare player performance data, which can be useful in a variety of ways for NBA teams and analysts. A player wants to be in the bottom right. If a player is in the top left, that means that they are not getting enough assists and comitting too many turnovers. If they are in the bottom left, they are careful with the ball but they arent getting enough assists. If a player is in the top right, they are getting assists but are being too careless with the ball and comitting turnovers.

Here are some contextual vizualizations I found on the web:

![Contextual 1](/assets/pngs/contextual1.png)

[source](https://www.reddit.com/r/nba/comments/5evzrx/of_active_players_with_more_than_5_assists_chris/)

This visualization shows how point guard Chris Paul has excelled at the assist/turnover stat for his entire carrer. This reddit post from the 2016-2017 shows that he was the only player in the NBA at the time that had a top 5 assist to turnover ratio that season while also having a carrer assist to turnover ratio that was above 4. As you can see in the scatterplot provided earlier, chris paul still excells at this stat as you can find Chris Paul having an average of 8.9 assists per game and 1.9 turnovers per game this season, 6 years after this graphic, he is still dominating this stat as he averages 4.68 assists for every turnover he commits.

![Contextual 2](/assets/pngs/contextual2.png)

[source](https://www.reddit.com/r/CollegeBasketball/comments/10spdw1/assist_to_turnover_ratio_vs_offensive_rating_from/)

This visualization is from this year's college basketball season, and it goes to show how much an offense relies on it's assist to turnover ratio in order to be sucessful. It is clear in this visualization that there is a direct positive correlation between a teams assist to turnover ratio and offensive rating of a team. 

## Search The Data & Methods

Below is where we can put some links to both the data and the analysis code as buttons:

```
<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html" text="The Analysis" %}
</div>
```

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

