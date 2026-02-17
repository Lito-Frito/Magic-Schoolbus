# Magic School Bus - Remote Learning Proof of Concept
![Magic School Bus](https://user-images.githubusercontent.com/56422761/165651711-3a9c08c4-0959-4607-9cea-805b10c4e8f3.png)

A proof-of-concept using system design to show how to bring wifi, via busses, to facilitate remote learning for kids during the pandemic. This is modeled after Kajeet's own success in doing something similar. 

## Use Cases
This would be for a max of a **few hundred students** in less than a **dozen spots** with maybe **1-2 buses per spot**. The buses have to be in the neighborhoods of kids to avoid having kids commute to the buses instead (e.g. if the buses were parked at a school lot and students need to drive up to it with parents to access).

**Wifi extenders** might be necessary to ensure complete coverage. The buses might need **GPS** capabilities to track buses for any reason. A local internet provider is essential  in order to have internet access. A partnership might be possible.

The wifi would **only be for school purposes** (e.g. no Netlfix or IG). This is to **minimize the load on the modem** (managing bandwidth) and to ensure kids are focused on school work. Would need to ensure that wifi is strong enough to stream video for Zoom. Can also have wifi only available during certain hours (e.g 8am-2pm) in order to minimize costs.

Wifi-buses enable schools to move expenses from transport budget to instructional budget. If a school bus serves a Title I school, funding can be used as it serves an instructional service. Additionally, buses can also double as a lunch delivery service for students on free or reduced lunch that don’t have access to food which could further scale costs.

## Entity Relationship Diagram
![alt text](https://user-images.githubusercontent.com/56422761/175348205-570d3296-624b-4ca6-95d9-2c058c6ac0a5.png)

## Constraints, Estimations, Bottlenecks, & Tradeoffs
The biggest constraints are the **range of the wifi**, the **power source** for the modem, and the **money** to upgrade the buses.

Based off figures from [Kajeet](https://www.cnn.com/2020/04/14/us/austin-wifi-busses-independent-school-district-trnd/index.html), the range of the wifi is about **300 ft**. This is probably using **2.4Ghz** wifi. While 5Ghz provides more bandwidth (which would be better suited for the purposes of conducting Zoom classes), it has significantly less range. It’s possible that more than one bus per location will be needed to ensure ample bandwidth for Zoom classes. **Wifi extenders** or a **mesh network** might also be needed in order to provide the necessary coverage needed. These would need to be integrated into the neighborhoods of the students somehow.

The effectiveness of this range is also affected by where the buses can park. Ideally they can park in areas with a high density of students. Otherwise students will need to drive up to lots the buses can park at so as to access it but still maintain social distancing. This can be another barrier for students and parents. A possible solution for this would be to provide multiple buses per area to provide a wide area of coverage to a neighborhood where the students are not close to one another.

To power the buses, Kajeet recommends running an AC adapter and an extension cord to a nearby physical outlet at a building. Or, depending on weather conditions, using a solar panel that charges that battery while the router is in use (which would incur additional charges).

For cost, we look at an example of a school in [Austin](https://www.cnn.com/2020/04/14/us/austin-wifi-busses-independent-school-district-trnd/index.html). They are quoted as having equipped ~500 buses with wifi through a $600K grant from [Kajeet](https://www.kajeet.net/how-does-school-bus-wi-fi-work/). We can estimate that it would cost ~**$1,200** per bus (this is probably higher if less buses are needed because cost scales less). The cost of a bus driver and potentially one staff member per bus might be needed and will incur additional costs. There is an [alternative](https://www.startlandnews.com/2020/03/transportant-wifi-covid-19/) to Kajeet but no cost information is available. The school could also choose to build the infrastructure themselves but that could be more costly and requires knowledge and skill that the school might not have.
