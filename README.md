# DevOps Practical Project
Fortune Teller Application

## Table of Contents
- [Project Overview](#project-overview)
- [Project Management](#project-management)
  * [Trello Board](#trello-board)
  * [Risk Assessment Matrix](#risk-assessment-matrix)
  * [Project Timeline](#project-timeline)
- [Databases](#databases)
- [Development](#development)
- [Testing](#testing)
- [Deployment](#deployment)
- [Further Analysis](#further-analysis)
- [Licensing and Copyright](#licensing-and-copyright)
 - [Contributors](#contributors)
 - [Acknowledgements](#acknowledgements)

## Project Overview
The purpose of this project is to create a functional Create, Read, Update, Delete (CRUD) fortune teller application with four services by using appropriate tools, technologies and methodologies. Inclusive of effective project management practices, utilising a MySQL database, C# and ASP.net for the full-stack development, testing functions and using Azure DevOps to create a pipeline to deploy the application to an app service.

## Project Management
This section will discuss the timeline, trello board, tasks and risks for the project.

###  Trello Board
<img width="959" alt="trello board" src="https://user-images.githubusercontent.com/82107035/121024165-e0c81780-c79b-11eb-9215-f2a154dd0dcd.PNG">

Every use case is inclusive of generating random objects to return it to the user.

<img width="305" alt="use case" src="https://user-images.githubusercontent.com/82107035/117555019-782e3380-b053-11eb-8ae7-62f8b42e1fde.PNG">


### Risk Assessment Matrix
<img width="482" alt="risks" src="https://user-images.githubusercontent.com/82107035/121039125-baf53f80-c7a8-11eb-8956-c4f01c3f8494.PNG">

###  Project Timeline
<img width="545" alt="project plan" src="https://user-images.githubusercontent.com/82107035/121048546-d19e9500-c7ae-11eb-8d45-8bdc40e9c7aa.PNG">


## Databases
Two tables – artist, album
ArtistID and songID are primary keys
Created two tables within a database to persistently store data for the project.

<img width="379" alt="databasearchitecture" src="https://user-images.githubusercontent.com/82107035/117578191-15857800-b0e5-11eb-8f8e-e1be8ee5e3a4.PNG">

Above shows the database architecture that will be used.


View Tables in Playlist Database.

<img width="202" alt="sqlshowtablesindb" src="https://user-images.githubusercontent.com/82107035/117554707-37351f80-b051-11eb-9c15-fc8e7b69a729.PNG">

View everything within the playlist table.

<img width="689" alt="selectallfromplaylists" src="https://user-images.githubusercontent.com/82107035/117554723-56cc4800-b051-11eb-8575-8ae09c4752b1.PNG">

View everything within the songs table.

<img width="689" alt="songstable" src="https://user-images.githubusercontent.com/82107035/117586663-6f039c00-b111-11eb-8929-645284b058f1.PNG">


## Development
The development of the application was done using C# and ASP.Net. Below are screenshots of the final application.

<img width="685" alt="viewplaylist" src="https://user-images.githubusercontent.com/82107035/117554638-e1f90e00-b050-11eb-9c9f-ed766a4a59bf.PNG">

<img width="722" alt="viewsongs" src="https://user-images.githubusercontent.com/82107035/117554660-fb9a5580-b050-11eb-8edc-207d1ab7403c.PNG">


## Testing
<img width="213" alt="tests" src="https://user-images.githubusercontent.com/82107035/117554760-9d21a700-b051-11eb-81ab-92e548e4586d.PNG">

Testing Analysis: I tested the functions in playlists. The testing has proved that it can access and connect to my database. It has proved that the functions work and then redirect to relevant pages. The testing is useful for future purposes because you don't have to worry about something failing or missing something.


## Deployment
This app was deployed to Azure App Service
<img width="960" alt="appservice" src="https://user-images.githubusercontent.com/82107035/117578669-4666ac80-b0e7-11eb-94f7-7ea0c0168a0f.PNG">

<img width="671" alt="appconnectiontoazuredb" src="https://user-images.githubusercontent.com/82107035/117578664-44045280-b0e7-11eb-94fa-8b055caee0f8.PNG">



## Further Analysis
Overall Risk Analysis: From revisiting the risk analysis, time estimations were inaccurate in the project plan, I needed more time allocated for development, testing, reaching out for support and understanding each aspect of the project. 
 
Known Issues: Not testing the songs controller because it was time consuming. Didn't create a CI/CD pipeline as there was an authorisation error when running the Yaml pipeline.
Found a bug from the testing, passing in CreatedAt as a different value in the binding model compared to "DateTime.Now" which showed differences in time. Limited time to do repository patterns so I sought help from my career advisor and we decided to use a more time-efficient method for testing - installing a Nuget Package (FrameworkCoreIn Memory) rather than creating an interface.

Future Implementation: Adding additional tables, such as adding albums to playlists. Create a yaml pipeline for the project. Use the repository patterns and interfaces for testing.

## Licensing and Copyright
© Ezra Turner, QA Limited, Avanade

## Contributors
- Ezra Turner <ezra.turner@avanade.com>

## Acknowledgements
- Dara Oladapo
- Nick Pribyl
- Ben Hesketh
- Victoria Sacre
