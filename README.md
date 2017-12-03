# Comparing Performance of top EPL teams

# Research Question
Which among the 4 top English Premier League teams (Chelsea, Arsenal,
        Manchester City and Manchester United) have been the most consistent
        performer over the period 2002 to 2016?

# Data Sources
- https://en.wikipedia.org/wiki/List_of_Chelsea_F.C._seasons [https://en.wikipedia.org/wiki/List_of_Chelsea_F.C._seasons]
- https://en.wikipedia.org/wiki/List_of_Manchester_United_F.C._seasons [https://en.wikipedia.org/wiki/List_of_Manchester_United_F.C._seasons]
- https://en.wikipedia.org/wiki/List_of_Manchester_City_F.C._seasons [https://en.wikipedia.org/wiki/List_of_Manchester_City_F.C._seasons]
- https://en.wikipedia.org/wiki/List_of_Arsenal_F.C._seasons [https://en.wikipedia.org/wiki/List_of_Arsenal_F.C._seasons]

# Analysis

The visualizations are concerned with answering the question of which team
        among the 4 top English Premier League teams, namely Chelsea, Arsenal,
        Manchester City and Manchester United have been the most consistent
        during the period 2002 to 2016. For this, I scraped Wikipedia pages
        and cleaned the data to create data frames for each team which contained
        their win-losses and their position in the league for each season.
        I first calculated win percentage for each team for each season and
        then used rolling_mean function of pandas to calculate five year moving
        average win percentages. Both the position in the league and win
        percentages were plotted to enable the viewer to compare the
        consistency in ranking and performance based on wins.

The plots clearly indicate that Arsenal FC is the most consistent team as
        it has remained in the top 5 throughout the analysis period and has
        an almost horizontal line in terms of win percentage.
        On the opposite end, seems to be the Manchester City team as its
        performance has grown over the period and has become consistent
        over the last 5-6 years.

# Using Cairo's Principles

 - In terms of truthfulness, the focus was to ensure that the scales of axis were suitably labelled and re-scaled. For instance, in case of performance in terms of ranking chart, the y-axis was scaled to reflect all 1-20 ranks and the y-axis was reversed to reflect 1 being more important. In the win percentage chart, y-axis was re-scaled from 0 to 100 to reflect all possible values.

 - In terms of beauty, the colors of the lines were chosen based on the uniform colors of the teams to allow audience to easily relate to them. Data-ink ratio has been kept high by removing chart boxes and unnecessary ticks.

 - In terms of functionality, lines have been labelled directly in the bottom chart and legend is used in the top chart. The most prominent result i.e. the lines representing Arsenal have been made bolder than other lines to focus attention on it.

 - In terms of insightfulness, two relevant charts one reflecting relative performance in terms of ranking and other reflecting absolute performance in terms of win % are used to draw conclusion on consistency of a team.
