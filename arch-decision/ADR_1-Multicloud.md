# ADR 1: Multicloud 
BadmintonPro requires an operational backbone capable of processing significant amounts of user generated data, including computationally intensive video analytics that analyze body movements and badminton form. The architecture demands performance, availablility, scalability, cost-efficiency, and reliability.
## Decision 
We will implement a Multicloud architecture in response to these needs. We will use multiple cloud platforms to accomplish the algorithmic generation of user advice based on their badminton form and movements. AWS and Azure are examples of effective cloud platforms that could be used.
## Rationale 
The multicloud solution promotes operational excellence by letting IT staff focus on key business needs, while as many services as possible are outsourced.
The multicloud solution promotes security by outsourcing a secure infrastructure.
The multicloud solution promotes reliability. Availability and robustness should peak since multiple clouds are available in order to cover for each other in case of outages.
Things such as CDNs and highly scalable data stores contribute to low latency and therefore, increased performance efficiency.
Cost is optimized in a multicloud solution because we will only pay for what we need.

We had to deny one cloud in this decision. One cloud would compartmentalize the skillsets needed in our human capital. It could further optimize cost. However, one cloud is not feasible given the scope of our operations. We plan to make our product accessible worldwide and highly available, with a very low error rate. The robust nature of multicloud ultimately resulted in our decision. And finally, the benefits corresponding to the AWS Well-Architected Framework made a cloud solution a must, compared to any non-cloud solution.

## Status
Accepted

## Consequences
The architecture is highly robust and efficient. The cloud allows for the outsourcing of key services which both improve quality and free human resources up for other tasks. The architecture adheres to many pillars of the AWS Well-Architected Framework as well.

There are negative consquences. Cost, initial implementation, and complexity are all things we will have to deal with since we chose a multicloud solution. The scope and total timeline of the project will likely be expanded as a result.
