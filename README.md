<!--
  TO DO:
  3. Remove the Gephi_report.docx file and attach a gdrive link for it here
  4. Mention the other contributors
  7. Complete with a thank you note
  8. Add description, not here in About option
-->

# 🚑Ambulance Path Analysis and Optimization using Network Analysis

## Introduction

<p>Ambulances transport people in need of emergency medical attention to nearby hospital in shortest time possible. The road network and the route chosen plays a crucial role in deciding
the duration of the journey. An efficient road network should ensure these conditions, the ambulance reaches the destination in shortest time irrespective of any change in the network, it
must be constructed in such a way that no accident prone zone is left unconnected to the network and hospitals are situated near to accident prone zones. Also, an efficient road network 
should have more roads connecting hospitals and accident prone zones, thereby ensuring the ambulance reaches in time even when the route changes suddenly. And an optimal route must include places or edges that are near to hospitals.</p>

<p>A road network can be evaluated based on these criteria to know its efficiency in ambulance services. This will help in deciding where to construct new hospitals and how to connect new
or existing accident prone zones to hospitals in shortest distance possible. In this project we have proposed a model which visualizes a road network as a graph and uses graph measurements like shortest path and shortest path distance to evaluate the road network efficiency in connecting hospitals and accident prone zones. The model evaluates the road network even at conditions when the crucial roads are blocked and when 2/5th of roads are blocked. This provides more insights on the strengths and drawbacks of the road network, which can be used to improve the efficiency of the road network. In addition to this, the model orders the existing paths or nodes connecting hospitals and accident prone zones based on the shortest distance. This can be used in optimizing the ambulance route by finding the next optimal path
or node in the times of sudden change in the road network.</p>

## Data Used
A simple network compirising of 12 nodes and 39 edges is used for analysis. The 12 nodes were divided into 3 categories, hospital, accident prone zones, normal places. The edges were reprsented using excel table, which was fed into the model for analysis.
#### Image of the Network
> ![Network used for analysis](https://github.com/G-stack-coder/Ambulance-Path-Analysis-and-Optimization-using-Network-Analysis/assets/72331711/73c47cec-5c23-4013-92b9-ad92b09b716e)

## Result of Analysis
> ![Result Table](https://github.com/G-stack-coder/Ambulance-Path-Analysis-and-Optimization-using-Network-Analysis/assets/72331711/d6430ab9-b7a5-4e4e-a68f-4626438927a2)

#### Columns
1. Graph : The Graph label<br>
2. Edges : Total number of edges in the network<br>
3. Perfect Accident Prone Zone : Accident Prone Zone that is connected to every hospital present in the network <br>
4. Poor Accident Prone Zone : Accident Prone Zone that is not connected to any hospital present in the network<br>
5. Sum of Shortest Paths : The sum of shortest paths between every accident prone zone to every hospital in the network

## Tools
1. Kaggle Notebook
2. Excel
3. Gephi

## Python Libraries 
1. Networkx
2. Pandas
3. Random
4. Matplotlib
5. Sklearn
   
## Future Scope
The real - world road networks consists of thousands of places and tens thousands of roads that are interconnected in a complex way. The proposed model was tested on a simple network, but by scaling up, the same model can be used to analyse real - world road networks. The results found out can be used as a deciding factor in choosing the right place to construct a new hospital, road or flyover. Also, a new model can be developed which can suggest a set of places in an decreasing order of priority. The parameters and constraints that influences the order of places can be the degree by which connectivity improves, the cost, environmental conditions, etc. The combination of both these models will help in increasing the efficiency of road network in ambulance services and also in increasing the connectivity between hospitals and accident prone zones.

## Project Files
1. **_APOREA_** : This file contains the source code of the model.
2. **_Edge_data_** : This contains the network in the form of a excel spreadsheet. There are two columns, _from_ and _to_ columns specifies the nodes of each edge in the network.
3. **_Flow Chart_** : This image depicts the overall flow of the model.
4. **_Node_label_** : This excel spreadsheet contains the labels associated with each node. There are three labels which are _Hospital_, _Accident Prone Zone_, _Normal Place_.
