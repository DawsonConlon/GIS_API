
<img width="3340" height="1834" alt="image" src="https://github.com/user-attachments/assets/ff52726a-beb0-4249-b8ca-409db4748a0e" />



Introduction

Air quality monitoring plays a critical role in understanding environmental health and identifying periods of elevated pollution that may pose risks to human health and ecosystems. Fine particulate matter (PM2.5) is one of the most widely used indicators of air quality because particles of this size are small enough to penetrate deep into the respiratory system and enter the bloodstream. As a result, monitoring PM2.5 concentrations provides valuable insight into both short-term pollution events and longer-term environmental trends.

This project analyzes PM2.5 air quality measurements for Saskatoon, Saskatchewan using data obtained from the Open-Meteo open-source API. The objective is to create ban automated data pipeline that explore patterns in particulate pollution and develop a clear visualization framework that could be used by environmental consultants or researchers to communicate air quality conditions.

The analysis focuses on three key objectives. First, the data is examined to identify significant pollution spikes where PM2.5 concentrations exceed 25 µg/m³, which is commonly used as a threshold for elevated particulate pollution events. Second, temporal patterns in the data are analyzed to determine whether seasonal trends influence air quality conditions throughout the year. Finally, the results are interpreted in the context of potential emission sources, such as wildfire smoke, transportation emissions, agricultural activity, and other regional environmental factors that may influence particulate concentrations in Saskatoon.

To support this analysis, a Python-based workflow was developed to process the API data, detect pollution events, and generate both statistical summaries and interactive visualizations through a dashboard. The goal of the project is not only to investigate local air quality trends, but also to demonstrate a reproducible data analysis pipeline that could be used for environmental monitoring and reporting.

Results:
I have pulled data from March 2016 - May 2017 from the API. The analysis of PM2.5 measurements collected for Saskatoon reveals several notable patterns in local air quality conditions over the study period. Overall, the data indicates that air quality in Saskatoon is generally within a moderate and expected range for a mid-sized urban center located within an agricultural region.

The average PM2.5 concentration observed in the dataset was 6.25 µg/m³, which falls within a typical background range for prairie cities. While this level is above the most stringent international guidelines, it is consistent with values commonly observed in Canadian urban environments influenced by transportation, residential emissions, and surrounding agricultural activity.

Despite generally moderate conditions, the dataset identified 18 individual sensor readings where PM2.5 concentrations exceeded 25 µg/m³, which was used in this analysis as a threshold for identifying significant pollution events. These exceedances represent short-term spikes in particulate pollution that may pose increased health risks during the period in which they occur.


<img width="756" height="331" alt="Screenshot 2026-04-14 at 6 38 44 PM" src="https://github.com/user-attachments/assets/50114070-4525-4884-8cc8-e198d0b7f73e" />


Most pollution spikes detected in the dataset were short-lived events, typically lasting less than one hour, indicating that the elevated particulate concentrations were likely caused by transient environmental factors rather than persistent emission sources. However, one event was detected that persisted for more than five hours, demonstrating that longer duration air quality degradation events can occur under certain atmospheric conditions.

The highest recorded PM2.5 concentration occurred on April 27, 2017, when measurements reached 51 µg/m³. On that same day, three additional readings also exceeded the 25 µg/m³ threshold, suggesting the presence of a sustained pollution episode rather than a single isolated spike.


<img width="828" height="548" alt="image" src="https://github.com/user-attachments/assets/7bf754e6-4985-4df4-bb2c-3d7b9160ae9c" />


Seasonal analysis of pollution events revealed a clear clustering of elevated PM2.5 measurements during April and May. These spring months appear to represent the period of highest risk for short-term particulate pollution events in Saskatoon.


<img width="738" height="602" alt="image" src="https://github.com/user-attachments/assets/6d76bf4a-0446-4201-85c7-6045538bab2c" />

Several environmental and regional factors may help explain this seasonal pattern. First, wildfire season in Saskatchewan officially begins on April 1st, and early-season fires can generate smoke plumes that travel long distances across western Canada and the northern United States. Even relatively distant wildfires can contribute measurable particulate pollution when atmospheric transport conditions carry smoke into urban areas.

In addition to wildfire smoke, spring agricultural activity across the Prairie provinces may contribute to elevated particulate concentrations. During this period, large areas of farmland surrounding Saskatoon undergo tillage and soil preparation, which can increase airborne dust levels and contribute to particulate matter in the atmosphere.

Other contributing factors may include road dust accumulation from winter, where sand and debris used for traction during colder months become resuspended once snow melts and roads dry, as well as unstable atmospheric mixing conditions common during seasonal transitions that can trap pollutants near the ground.

Interestingly, while wildfire smoke is often associated with mid-to-late summer in western Canada, this dataset shows fewer extreme PM2.5 events during peak summer months. This may reflect the specific wildfire activity patterns during the study period or limitations of the available dataset.

Two notable spikes occurred on May 12, 2016 and April 27, 2017, both of which produced some of the highest particulate concentrations observed. Unfortunately, publicly available historical air quality records for Saskatchewan prior to 2020 are limited, making it difficult to directly validate these events against archived environmental monitoring reports or media coverage. However, given the magnitude and temporal clustering of the readings, it is likely that these spikes were associated with regional wildfire smoke transport, potentially originating from fires within Saskatchewan or neighboring jurisdictions.

Finally, it is important to note that the analysis pipeline developed in this project is flexible and can easily be adapted to evaluate different pollution thresholds. For example, the same workflow could be used to identify days where PM2.5 concentrations exceed 10 µg/m³, which would allow for the detection of more moderate air quality degradation events and provide additional insight into long-term exposure trends.

Overall, the results demonstrate that while average air quality conditions in Saskatoon remain relatively stable, short-duration particulate pollution events do occur periodically and appear to be influenced by seasonal environmental factors common to prairie regions.
