## Wolrd Events Analysis April 2022

This page illustrates a set of analysis as well as visualizations of the current world events happening in April 2022, specifically focusing on analyzing events in Ukraine. 

![image](Russia-Ukraine.jpeg)

### Introduction

It is war time in Ukraine, the internet is down and there is not enough proper access to the news sources. Fortunately, a foreign intelligence agency was able to provide [screenshots](https://drive.google.com/file/d/1XhV7EUPRAKlzKHYpjR_LN1W3IjP8l-5U/view) from three news sources CNN, Fox, and Alijazeera. Each screenshot contains all the news from a single day from March 2022, sorted chronologically and stacked on top of each other. It is important to be able to extract the data from these images and to analyze the events as they unfold day by day. 

Any discovery would be attributed to understanding events happening in Ukraine. 

### Data processing

Technologies such as Optical Character Recognition (OCR), Named Entity Recognition (NER), GeoParsing and some visualization are ultilized to analyze the given data.

1. Firstly, the OCR tool Tesseract was used to extract text out of the given screenshots.
2. Secondly, the NER tool SpaCy was used to detect and extra the following entities out of OCR texts:
  - PERSON: People, including fictional.
  - NORP: Nationalities or religious or political groups.
  - FAC: Buildings, airports, highways, bridges, etc.
  - ORG: Companies, agencies, institutions, etc.
  - GPE: Countries, cities, states.
  - LOC: Non-GPE locations, mountain ranges, bodies of water.
  - PRODUCT: Objects, vehicles, foods, etc. (Not services.)
  - EVENT: Named hurricanes, battles, wars, sports events, etc.
  - DATE: Absolute or relative dates or periods.
  - TIME: Times smaller than a day.
4. Finally, Python GeoPy was used for geoparsing GPE and LOC entities to illustrate the frequency of these entities as they appear in the news day-by-day.


### Findings

[LOC Mapbox](LOC_pic.html)

### Contributors
Team DHKMWY - [Duyen Nguyen](https://github.com/duyen21), Harvey Fu, Kaiyin Chan, My Ta, Weixing Nie, and Yue Zeng.

Our source code can be found at the top right of the page or [here](https://github.com/duyen21/World-Events-Analysis).
