# PlaceToBeer - Software Requirements Specification



## Table of Contents



-   [Flashcard Community - Software Requirements Specification](#flashcard-community---software-requirements-specification)



    -   [Table of Contents](#table-of-contents)



    -   [1. Introduction](#1-introduction)



        -   [1.1 Purpose](#11-purpose)

        -   [1.2 Scope](#12-scope)

        -   [1.3 Definitions, Acronyms and Abbreviations](#13-definitions-acronyms-and-abbreviations)

        -   [1.4 References](#14-references)

        -   [1.5 Overview](#15-overview)



    -   [2. Overall Description](#2-overall-description)

		

		 -   [2.1 Vision](#21-vision)

		 -   [2.2 Use Case Diagram](#22-use-case-diagram)

		 -   [2.3 Technology Stack](#23-technology-stack)



    -   [3. Specific Requirements](#3-specific-requirements)



        -   [3.1 Functionality](#31-functionality)

        -   [3.2 Usability](#33-usability)



        -   [3.3 Reliability](#34-reliability)



        -   [3.4 Performance](#35-performance)



        -   [3.5 Supportability](#36-supportability)



        -   [3.6 Design Constraints](#37-design-constraints)



        -   [3.7 Online User Documentation and Help System Requirements](#38-online-user-documentation-and-help-system-requirements)



        -   [3.8 Purchased Components](#39-purchased-components)



        -   [3.9 Interfaces](#310-interfaces)



            -   [3.9.1 User Interfaces](#3101-user-interfaces)

            -   [3.9.2 Hardware Interfaces](#3102-hardware-interfaces)

            -   [3.9.3 Software Interfaces](#3103-software-interfaces)

            -   [3.9.4 Communications Interfaces](#3104-communications-interfaces)



        -   [3.10 Licensing Requirements](#311-licensing-requirements)



        -   [3.11 Legal, Copyright and other Notices](#312-legal-copyright-and-other-notices)



        -   [3.12 Applicable Standards](#313-applicable-standards)



    -   [4. Supporting Information](#4-supporting-information)



## 1. Introduction



### 1.1 Purpose

In the following Software Requirements Specification (SRS) functional and quality requirements for the webapplication PlaceToBeer will be descriped.



### 1.2 Scope

Subsystems:

- Account system:
A user can register an account and change the acccount settings. On the login the saved credentials will be verified. The data is saved in a database.

- Group system:
Each user has the possibilty to create groups. The user can then invite already registered users or invite new ones by a generated email. The creater receives the owner role for the group. Following group roles exists:
	- Owner:
	The owner has full rights to modify all group settings. This includes granting and revoking admin roles and deleting     the group.
    - Admin:
    An admin extends the rights of the regular member by being able removing other admins and members from the group.
    - Member:
    This is the default role for all newly added users. They can modify the group name and invite users. Of cousé they   	 can leave the group at any time.

- Rating system:
Each group member should be able to add locations to the rating list. The rating list contains every proposal ready to be rated. It is devided into two sublists:
	- The <b>unvisited proposals</b> can be marked with "thumbs-up", "neutral", or "thumbs-down". This rating should be based on one's very first impression and indicates the group's attitude towards a proposal.
	- The <b>visited proposals</b> can be rated using a 1 to 5 stars system based on experiences. All this information is used to generate two best-of lists which will be displayed on the dashboard.

The rating workflow starts with the possibility to add a proposal. During this process the user can set the name of the proposal, define the kind of activity (bar, restaurant, etc.), the address, and if it has already been visited. Furthermore, one can choose to which group or groups the location should be proposed. Depending on the selected "visited" status, the location is ordered in the fitting rating sublist.
After the rating process described above they are moved to the corresponding best-of list. The **best-of unvisited proposals** list offers to mark proposals as "already visited". If done so, the proposal returns to the **rating list** but will now appear in the **unvisited proposals** list.

The whole dashboard can be filtered by the activity of the proposal.

- Suggestion generation system:
This system can be used by a group to automatically generate a suggestion depending on the ratings. Any member can initialize this process. To personalize the results to the groups preferences filters can be used to select specific kinds of activities. Moreover it is possible to decide between visited and unvisited proposals.

- Group navigation system
A user can switch between the groups he or she is a member of. The system offers possibilities to accept and decline group invitations and create new groups.

### 1.3 Definitions, Acronyms and Abbreviations



| Term     |                                     |

| -------- | ----------------------------------- |

| **SRS**  | Software Requirements Specification |

| **JSON** | JavaScript Object Notation          |

| **API**  | Application Programming Interface   |

| **MTBF** | Mean Time Between Failures          |

| **MTTR** | Mean Time To Repair                 |

| **DTO**  | Data Transfer Object                |

| **HTTP** | Hypertext Transfer Protocol         |

| **FAQ**  | Frequently Asked Questions          |

| **REST** | Representational State Transfer     |



### 1.4 References



| Title                                                                                                 | Date       |

| ----------------------------------------------------------------------------------------------------- | ---------- |

| [Blog](https://flashcardcommunity.wordpress.com/)                                                     | 17/10/2018 |

| [GitHub](https://github.com/phoenixfeder/fc-com/)                                                     | 17/10/2018 |

| [Spring Boot](https://spring.io/projects/spring-boot)                                                 | 19/10/2018 |

| [ReactJS](https://reactjs.org/)                                                                       | 19/10/2018 |

| [Use Case Diagram](https://github.com/phoenixfeder/fc-com/blob/master/FlashCardCommunityUseCases.png) | 21/10/2018 |



### 1.5 Overview
tbd

## 2. Overall Description



### 2.1 Vision

PlaceToBeer is a webbased platform to propose and rate places and events in your friend group. The idea is to individually rate bars, pubs, clubs, restaurants or wherever you can have fun together located in Karlsruhe.



In the webapp you can create and manage groups with different users. All users should be able to submit newly discovered places to hang out. Each group member can rate places so "best-of" lists can be generated. Automatic suggestions can be generated based on ratings and set filters. After the visit, every member can give a further and more specific rating, which serves to fill another "best-of" list.



### 2.2 Use Case Diagram



### 2.3 Technology Stack



#### 2.3.1 Frontend

- Framework: Angular 2.0

- Language: TypeScript

- IDE: WebStorm

- Testing: tbd



#### 2.3.2 Backend

- Framework: Spring

- Language: Kotlin

- IDE: IntellJ

- Testing: JUnit4

- Database: tbd



#### 2.3.2 Projectmanagement

- Project management tool: YouTrack

- Version control: git and github

- Organizing: Evernote



## 3. Specific Requirements



### 3.1 Functionality
Until december the following usecases are planned to be implemented:
LUCIE

### 3.2 Usability
LUCIE


### 3.3 Reliability
PATRICK

### 3.4 Performance
PATRICK

### 3.5 Supportability
TOM

### 3.6 Design Constraints
tbd

### 3.7 Online User Documentation and Help System Requirements
tbd

### 3.8 Purchased Components
tbd

### 3.9 Interfaces


#### 3.9.1 User Interfaces
LUCIE

#### 3.9.2 Hardware Interfaces
tbd

#### 3.9.3 Software Interfaces
TOM

#### 3.9.4 Communications Interfaces
PATRICK

### 3.10 Licensing Requirements
tbd

### 3.11 Legal, Copyright and other Notices
tbd

### 3.12 Applicable Standards
tbd

## 4. Supporting Information
TOM
