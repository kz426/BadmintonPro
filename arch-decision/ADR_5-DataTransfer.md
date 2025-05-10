# ADR 5: Data Transfer
BadmintonPro requires a secure and fast data transfer protocol in order to transfer user data to and between the cloud servers as well as return the personalized advice to the user promptly.

## Decision 
We will use REST API to transfer data between the various components, from the local client licensed applications to the cloud servers and back.

## Rationale 
REST API not only supports .NET. It also integrates well with cloud servers. 
REST API promotes operational excellence due to the relative ease of development and maintenance.
REST API promotes security due to the many security protocols available.
REST API is scalable due to its stateless nature.
Event Driven architecture was also considered but rejected. This would likely have been more scalable and lead to faster performance. However, it is more complicated than a simple REST API. This could potentially slightly stunt operational excellence. We are considering delivery timelines/turnaround in this project heavily, as we believe in the potential popularity of the product. Event Driven architecture also does not integrate as well into the design mentioned in the first 4 ADRs as well as REST APIs.

## Status
Accepted

## Consequences
The result is a well integrated, secure, and easy to work on, data transfer protocol. 
Scalabilty is neutered due to having to reject Event Driven Architecture.
REST APIs aren't used with live data, reducing the potential of our application.
REST APIs may be slightly inefficient if the data files (especially very long anonymized recordings) take up huge file size.
