Traffic count data from around Wellington, New Zealand. Collected for multiple dates between February and November 2024.
Counts taken on quarter-hourly intervals aggregated into hourly counts.
Weekend dates removed. 
Historical, hourly, weather data from open-meteo.com. 
Matched on date and hour, engingeered weather for previous hour against traffic count for present hour.
ie predict current traffic based on the weather in the previous hour.

No strongly performing models (best R2=.28, best MAE = 127).
Comparisons of top 10 coefficient effects from linear models and feature importances from ensemble models.
There was agreement for only six features, relating to: season (strong reduction of traffic counts in summer); traffic origin/destination/ (moderate reduction when traffic if from the south);
2nd and 3rd hours of peak traffic (strong increases), time of day (slight reduction in the morning),  and temperature (moderate increase in traffic counts).

Recommendations including using more of the traffic data set (not excluding weekend data), and/or trying to find a dataset covering an entire year. Also, there are certain engineered polynomial features
we didn't explore but expect could have have been more enlightening.

TLDR: Compared hourly traffic counts to weather from the previous hour. Predictive models performed poorly.
Key features highlight pattern of importance relating to positional commuting hour, season, wind direction, and time of day.
Models may have performed better with more traffic data, and/or with the inclusion of polynomial features.
