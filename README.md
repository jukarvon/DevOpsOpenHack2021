[![Board Status](https://dev.azure.com/OpenHackNovember/ff8ef51d-a0d7-4615-9b94-0ebd982dd9fa/f9e509d7-071f-4912-ad98-390c7314daf0/_apis/work/boardbadge/dac03a18-ef1b-457b-858f-8e42db9f180d)](https://dev.azure.com/OpenHackNovember/ff8ef51d-a0d7-4615-9b94-0ebd982dd9fa/_boards/board/t/f9e509d7-071f-4912-ad98-390c7314daf0/Microsoft.RequirementCategory)
---
page_type: sample
languages:
- csharp
- java
- go
- javascript
- powershell
products:
- azure
description: "The DevOps open hack event is designed to foster learning via implementing DevOps practices with a series of challenges."
urlFragment: openhack-devops-team
---

# My Driving Team APIs

The DevOps open hack event is designed to foster learning via implementing DevOps practices with a series of challenges.

## Architecture

The application used for this event is a heavily modified and recreated version of the original [My Driving application](https://github.com/Azure-Samples/MyDriving).

The team environment consists of the following:

* Azure App Service for Linux which has four APIs deployed:

  * POI (Trip Points of Interest) - CRUD API written in .Net Core 3.1 for points of interest on trips
  * Trips - CRUD open API written in golang 1.11 for trips connected to the client application
  * UserProfile - CRUD open API written in Node.JS for the users of the client application
    > Note:PATCH/POST operations not functional
  * User-Java - API written in Java with POST and PATCH routes plus swagger docs routes for the users of the client application.
* Mobile Apps - for iOS and Android which will display driving trip data

## Getting Started

To understand each of the components above in more detail, please visit the readme files inside the root folder of each corresponding part of the application.

### Prerequisites

It is useful but not required to have a basic knowledge of the following topics:

* Azure App Services
* Azure Container Registry and Docker
* GitHub, Azure DevOps (formally VSTS) or Jenkins

## Resources

The provisioning of this environment for proctors can be found in the [DevOps Openhack Proctor](https://github.com/Azure-Samples/openhack-devops-proctor) Github repository.
