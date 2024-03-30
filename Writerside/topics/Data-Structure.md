# Data Structure

| field name            | 	Description                                                                                                                                           |
|-----------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    | Id of the Fungi / Bacteria.                                                                                                                            |
| Class                 | 	The taxonomy of life is a system that classifies life into domains, kingdoms, phyla, **classes**, orders, families, genera, and species.              |
| Coordination          | 	The Coordinates where the plant was sampled, the coordinates will be in this format: {"lon": longitude (float), "lat": latitude (float)}              |
| Date                  | 	Date when the plant was sampled (MM/DD/YYYY)                                                                                                          |
| DiffR                 | 	Diffused radiation (w/m^2) [Data from Israel Meteorologic Service]                                                                                    |
| F                     | 	"F" refers to "Flower"                                                                                                                                |
| Family                | 	The taxonomy of life is a system that classifies life into domains, kingdoms, phyla, classes, orders, **families**, genera, and species.              |
| Fr                    | 	"Fr" refers to "Fruit"                                                                                                                                |
| Genus                 | 	The taxonomy of life is a system that classifies life into domains, kingdoms, phyla, classes, orders, families, **genera**, and species.              |
| Grad                  | 	Global radiation (w/m^2) [Data from Israel Meteorologic Service]                                                                                      |
| Hebrew Plant Name     | 	The name of the plant in Hebrew                                                                                                                       |
| Kingdom               | 	The taxonomy of life is a system that classifies life into domains, **kingdoms**, phyla, classes, orders, families, genera, and species.              |
| Kit ID                | 	The id of the kit                                                                                                                                     |
| L                     | 	"L" refers to "Leaf"                                                                                                                                  |
| Location              | 	The location where the plant was sampled                                                                                                              |
| Location Picture      | 	Screenshot of the location in Google Maps, Apple Maps...                                                                                              |
| NIP                   | 	Direct radiation (w/m^2) [Data from Israel Meteorologic Service]                                                                                      |
| Order                 | 	The taxonomy of life is a system that classifies life into domains, kingdoms, phyla, classes, **orders**, families, genera, and species.              |
| Phylum                | 	The taxonomy of life is a system that classifies life into domains, kingdoms, **phyla**, classes, orders, families, genera, and species.              |
| Plant Picture         | 	Image URL of the plant                                                                                                                                |
| R                     | 	"R" refers to "Root"                                                                                                                                  |
| RH                    | 	Relative humidity (%) [Data from Israel Meteorologic Service]                                                                                         |
| Rain                  | 	Rainfall (mm) [Data from Israel Meteorologic Service]                                                                                                 |
| S                     | 	"S" refers to "Soil"                                                                                                                                  |
| STDwd                 | 	Standard deviation wind direction (deg)                                                                                                               |
| School                | 	The name of the school where the students from                                                                                                        |
| Scientific Plant Name | 	The scientific name of the plant                                                                                                                      |
| Species               | 	The taxonomy of life is a system that classifies life into domains, kingdoms, phyla, classes, orders, families, genera, and **species**.              |
| TD                    | 	Temperature (Celsius) [Data from Israel Meteorologic Service]                                                                                         |
| TDmax                 | 	Maximum Temperature (Celsius) [Data from Israel Meteorologic Service]                                                                                 |
| TDmin                 | 	Minimum Temperature (Celsius) [Data from Israel Meteorologic Service]                                                                                 |
| TG                    | 	Grass minimum Temperature (Celsius) [Data from Israel Meteorologic Service]                                                                           |
| Temperature           | 	The temperature that the students wrote in the meta data according a weather app                                                                      |
| Treatment             | 	Detailing the sample's origin, specifying if it originates from an experimental setup or is derived from an environment that has undergone treatment. |
| WD                    | 	Wind direction (deg) [Data from Israel Meteorologic Service]                                                                                          |
| WDmax                 | 	Gust wind direction (deg) [Data from Israel Meteorologic Service]                                                                                     |
| WS                    | 	Wind speed (m/s) [Data from Israel Meteorologic Service]                                                                                              |
| WSmax                 | 	Gust wind speed (m/s) [Data from Israel Meteorologic Service]                                                                                         |
| count_F               | 	1 if there is Fungi / Bacteria in the Flower, 0 otherwise                                                                                             |
| count_Fr              | 	1 if there is Fungi / Bacteria in the Fruit, 0 otherwise                                                                                              |
| count_L               | 	1 if there is Fungi / Bacteria in the Leaf, 0 otherwise                                                                                               |
| count_R               | 	1 if there is Fungi / Bacteria in the Root, 0 otherwise                                                                                               |
| count_S               | 	1 if there is Fungi / Bacteria in the Soil, 0 otherwise                                                                                               |
| kit_id                | 	The id of the kit                                                                                                                                     |

Note: there is two columns with kit id, `kit_id` and `Kit ID`, their values the same.