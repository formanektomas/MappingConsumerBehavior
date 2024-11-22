# MappingConsumerBehavior

Supporting matterials for the article "Mapping consumer behavior: store location effects on retail sales across different basket types"


### List of variables considered for the explanatory part of the analysis

| Regressor name         | variable description | data source                                 |
|----------------------- | -------------------- | ------------------------------------------- |
| IDENT_PROD		 | store ID             |                                             | 		
| Region                 | NUTS 3 ID            | https://ec.europa.eu/eurostat/web/products-catalogues/-/ks-04-14-908 |
| PRG 	                 | binary for Prague    | https://ec.europa.eu/eurostat/web/products-catalogues/-/ks-04-14-908 |
| Pharm5mWalk            | No of pharmacies within reach of 5 min pedestrian walk (OSM)     |  https://www.openstreetmap.org/ |
| Pharm10mWalk           | No of pharmacies within reach of 10 min pedestrian walk (OSM)    |  https://www.openstreetmap.org/ |
| Post5mWalk             | No of post-offices within reach of 5 min pedestrian walk (OSM)   |  https://www.openstreetmap.org/ |
| Post5mWalkB            | Post5mWalk transformed into 0,1,2,3 where 3 is for 3+            |  https://www.openstreetmap.org/ |
| Post10mWalk            | No of post-offices within reach of 10 min pedestrian walk (OSM)  |  https://www.openstreetmap.org/ |
| Post10mWalkB           | Post10mWalk transformed into 0,1,2,3,4,5 where 5 is for 5+       |  https://www.openstreetmap.org/ |
| Rstn5mWalk             | No of restaurants/pubs within reach of 5 min pedestrian walk (OSM)|   https://www.openstreetmap.org/ |
| Rstn5mWalkB            | Rstn5mWalk transformed into 0,1,2,...,20 where 20 is for 20+     |    https://www.openstreetmap.org/ |
| Rstn10mWalk            | No of restaurants/pubs within reach of 10 min pedestrian walk (OSM)|   https://www.openstreetmap.org/ |
| Rstn10mWalkB           | Rstn10mWalk transformed into 0,1,2,...,40 where 40 is for 40+    |   https://www.openstreetmap.org/ |
| PTStop5mWalk           | No of public transport stops within reach of 5 min pedestrian walk (OSM)|   https://www.openstreetmap.org/ |
| PTStop5mWalkB          | PTStop5mWalk transformed into 0,1,2,...,20 where 20 is for 20+   |  https://www.openstreetmap.org/ |
| PTStop10mWalk          | No of public transport stops within reach of 10 min pedestrian walk (OSM)|   https://www.openstreetmap.org/ |
| PTStop10mWalkB         | PTStop10mWalk transformed into 0,1,2,...,40 where 40 is for 40+  |   https://www.openstreetmap.org/ |
| roadDist               | Distance of the store from highway/major road in meters (RCzechia) | OSM & RCzechia package in R | 
| parkDist               | Distance to nearest parking place in meters (no parking capacity info available)|    https://www.openstreetmap.org/ |                                                    
| mallDist               | Distance to nearest mall in meters                               |    https://www.openstreetmap.org/ |
| inMall                 | Binary in mall presence                                          |   https://www.openstreetmap.org/ & retailer records |
| Compet5mWalk           | No of competitors within reach of 5 min pedestrian walk (OSM)    |   https://www.openstreetmap.org/ |
| competHigh             | 5+ stores within 5 min pedestrian walk                           |   https://www.openstreetmap.org/ |
| Compet10mWalk          | No of competitors within reach of 10 min pedestrian walk (OSM)   |   https://www.openstreetmap.org/ |
| PopDens                | Inhabitants per sq km, for the relevant city district or for the whole city (village) if there are no districts |   https://csu.gov.cz/ |
| PopDens440m            | Population per 440m H3 hexagon                                  | https://www.kontur.io/geospatial-datasets-catalog/#population |
| PopDens3km             | Population per 3km  H3 hexagon                                  | https://www.kontur.io/geospatial-datasets-catalog/#population |
| Location               | Factor, 6 levels of location types (e.g. pedestrian area)       |  retailer   | 
| StoreSize              | Sales floor area                                                |  retailer   | 
| StoreSizeTotal         | Total store size                                                |  retailer   | 
| WageMean               | Mean wages at the NUTS3 level                                   |  https://csu.gov.cz/ |
| WageMedian             | Median wages at the NUTS3 level                                 |  https://csu.gov.cz/ |
| CityCent               | Binary from "Location", city center                             |  retailer   | 
| cityPer                | Binary from "Location", city periphery                          |  retailer   | 
| bc                     | Betweenness centrality                                          |  https://www.openstreetmap.org/ , igraph R package |
| bc_s                   | bc scaled                                                       |  https://www.openstreetmap.org/ , igraph R package | 
| hc                     | Hub centrality                                                  |  https://www.openstreetmap.org/ , igraph R package |
| hc_s                   | hc scaled                                                       |  https://www.openstreetmap.org/ , igraph R package |
| cc                     | Closeness centrality                                            |  https://www.openstreetmap.org/ , igraph R package |
| cc_s                   | cc scaled                                                       |  https://www.openstreetmap.org/ , igraph R package |
| ec                     | Eigenvector centrality                                          |  https://www.openstreetmap.org/ , igraph R package |
| ec_s                   | ec scaled                                                       |  https://www.openstreetmap.org/ , igraph R package |
| rc                     | Reach centrality                                                |  https://www.openstreetmap.org/ , igraph R package |
| cc_s                   | rc scaled                                                       |  https://www.openstreetmap.org/ , igraph R package |
| idc                    | In-degree centrality                                            |  https://www.openstreetmap.org/ , igraph R package |
| idc_s                  | idc scaled                                                      |  https://www.openstreetmap.org/ , igraph R package |
| odc                    | Out-degree centrality                                           |  https://www.openstreetmap.org/ , igraph R package |
| odc_s                  | odc scaled                                                      |  https://www.openstreetmap.org/ , igraph R package |
| buidl_sat              | Built-up area as of 2019, satellite imagery, Copernicus,        | https://lcviewer.vito.be/download | 
| build_OSM              | Built-up area as of 2019, OSM polygons                          | http://download.geofabrik.de/europe/czech-republic.html# |



