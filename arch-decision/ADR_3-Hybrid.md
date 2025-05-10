# ADR 3: Hybrid 
It was noticed during the mock press release, that many potential customers were concerned about the mandatory disclosure of video footage of themselves in order to use the product. Not only did this reduce consumer desire for the product, but it also presents legitimate security concerns that we should address in order to protect the customer base.

## Decision 
We will utilize a hybrid model for our software architecture. Licensed local software will be used to convert the user's video footage into versions where they would appear as "wireframe models" if somehow the video was leaked. The local software would be able to operate outside of internet connection, and be highly secure. After this operation is done locally, the anonymized wireframe data would be sent to the cloud video storage servers. In this way, the architecture would be a hybrid between cloud, and locally licensed software.

## Rationale 
Privacy would be maximized with this decision. User data will be highly secure. Operations involving the user's video footage would be done completely locally. They would only transfer data to the cloud servers that is necessary to analyze form and body movement. 
Performance Efficiency would also be achieved. Our algorithms would more easily analyze wireframe model data. Without extraneous data such as backgrounds and faces, the algorithm could work more efficiently.

Fully cloud-based architecture was rejected. If this happened, then the user's private video footage would be exposed to attack, presenting privacy concerns. 

## Status
Accepted

## Consequences
User data will be highly secure. Anonymized data is not only efficient to process, but ensures privacy.
Anonymizing data and then sending it to the servers in this hybrid way, requires another layer, more expertise, and the development of a licensed pricing model. There is no way to prevent users from lending their software for free to others, for example. 
There is added complexity due to the hybrid nature.
