# ADR 2: Video Storage
User video data will have to be stored for BadmintonPro. However, solutions such as SQL or NoSQL would not store video files efficiently. We need a solution that can efficiently store video files.

## Decision 
We will utilize cloud based video storage services in order to store video files. 

## Rationale 
Cloud video storage promotes operational excellence. Since we are already using multicloud platforms for our algorithm computing infrastructure, cloud data storage is natural and could be integrated easily. The user data could be fed as inputs more seamlessly into the computing components.
Cloud video storage is cost optimized compared to SQL and NoSQL. Video files would consume a disproportionate amount of data on SQL/NoSQL servers.
Cloud video storage promotes performance efficiency as well. SQL and NoSQL would inefficiently handle the transfer of huge video files with high throughput/demand. This issue would be mitigated with cloud storage.

## Status
Accepted 


## Consequences
Cloud video storage promotes operational excellence, cost reduction, and efficiency.
However, cloud video storage provides more complexity rather than using a standard SQL server. Additional, perhaps slightly less common skillsets would be required (cloud data storage). Cloud based video storage services are slightly more niche of a concept than SQL databases.
