# ADR 4: UI
BadmintonPro needs to be accessible and reach users no matter what brand of device they use. The UI must allow the user to upload their video data, anonymize it, and receive guidance on their play promptly.

## Decision 
We will use .NET MAUI in order to make the UI accessible for users of Android, iOS, PC, and Mac.

## Rationale 
.NET MAUI promotes operational excellence. Since the UI is universal across all platforms, insignificant additional effort will have to be invested into each type of device. In addition, it allows us to implement as much UI as possible into a singular codebase.
Avalonia UI and Flutter were also considered. They were ultimately rejected in favor of .NET MAUI for its libraries, workflows, and high quality integration ability.

## Status
Accepted

## Consequences
.NET MAUI improves workflow efficiency by allowing a single codebase to contain a majority of the UI that will be used across various devices.
.NET MAUI also provides ample support as well. 
.NET MAUI is somewhat new. There is a risk for performance drops with .NET MAUI. It is an emerging framework that may require additional overhead to function at its best.
