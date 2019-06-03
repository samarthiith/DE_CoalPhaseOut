# Analysing possible generation adequacy issues with Germany's Coal Phaseout

With the announcement of coal phase out in Germany the issue of generation adequacy has become critically important. Here the data and code used for the analysis is provided.

The analysis is based on following indicators: 

![Indicators](https://github.com/samarthiith/DE_CoalPhaseOut/blob/master/indicators.png)

## Capacity Factor Comparision

Capacity factors from different sources were used - [EMHIRES](https://ec.europa.eu/jrc/en/publication/eur-scientific-and-technical-research-reports/emhires-dataset-part-i-wind-power-generation-european-meteorological-derived-high-resolution) and [NINJA](https://www.renewables.ninja/). Significant differences can be found between the sources. The Figure shows the distribution of the full load hours between the sources. 30 years weather data from each source is used.

![VRE Capacity Factors](https://github.com/samarthiith/DE_CoalPhaseOut/blob/master/resCFDist.png)

## Availability Factors used for calculation of reliable capacity

| Power Plant | Availability|
| -- 	| -- |
| Pump Storage | 1,000|
| Biomass		| 0,830|
| Run of River|	0,740|
| Other	| 0,900|
| Oil |0,845|
| Gas	|0,902|
| Coal |	0,857|
| Lignite |	0,857|

## Best and worst case assumptions w.r.t RES Installed capacities (2023)

|Installed Capacity [GW]| Worst Case | Best Case|
|---|---|---|
|Wind Onshore|54.7|67.7|
|Wind Offshore|7.1|9.4|
|PV|50.3|50.3|
|Total|112.2|124.5|

Comparing the two cases, the figure below shows the distribution of the peak residual. The distribution is based on 540 MC Instances (60 weather years and 9 load years). 

![VRE Capacity Factors](https://github.com/samarthiith/DE_CoalPhaseOut/blob/master/peakDist.png)
