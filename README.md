# AirMan-Database-System
This repository contains the design and implementation of the AirMan System for managing airport operations at London Biggin Hill Airport. It includes an ERD diagram, MySQL scripts for database creation, data insertion, and queries, as well as detailed data definitions and system requirements documentation.

## Background
London Biggin Hill Airport is a general aviation airport at Biggin Hill in the London Borough of Bromley, approximately 14 miles south-southeast of Central London. The airfield has been publicly owned by the London Borough of Bromley since 1974 and evolved into a private airfield in 1994 when it was leased by Biggin Hill Airport Ltd. to run it on a commercial basis. It is effectively a public-private partnership. Its commercial potential took a turn for the better when Bombardier announced its European relocation from Amsterdam to London Biggin Hill in 2016. Furthermore, the London Aerospace & Technology College funding was secured in 2018, as was planning for an Airport Hotel.

The airport has a Civil Aviation Authority (CAA) Ordinary Licence that allows flights for the public transport of passengers or flying instruction. The airport specializes in general aviation, handling a spectrum of traffic from private aviation to large business jets. It has no scheduled airline service, as flights using the airport are not permitted to carry fare-paying passengers.

The airport has one runway that can accommodate the take-off and landing of aircraft up to Boeing 737/Airbus A320 size. It is also an Instrument Landing System. Radar air traffic control (ATC) services are provided by Thames Radar at the London Terminal Control Centre. In contrast, procedural approach visual flight rules and air traffic control services are provided by the airport itself.

Biggin Hill is used by many business flights involving business jets and similar-sized aircraft. The airport has a passenger terminal located on the A233 road just south of Leaves Green, which provides facilities for such flights, including departure lounges, a licensed café bar, and customs and immigration facilities.

London Biggin Hill Ltd owns and manages the airfield, which operates national and international flights for private, corporate, and commercial aircraft. It also provides an aircraft home base for aircraft owners, aircraft management companies, and industrial customers, such as Formula One base. As with many organizations that grew organically, Biggin Hill Airport’s information needs are met using a variety of ad-hoc, siloed systems that are not fit for purpose. David Winstanley, CEO of London Biggin Hill Airport, commissioned a new project aimed at replacing these disparate systems into a unified, modular design of systems. The core operations and services that support the Airport’s value proposition to customers are:

1. General operations such as customer and visitor parking, ground transport, security and UK Border Patrol, Heli-shuttle transit services, private airport lounges, baggage handling, contactless travel (a new Covid-19 measure), and aircraft charter.
2. Core operations on the aircraft side include ground handling equipment, maintenance, aircraft cleaning, catering, and hanger facilities are available. Pilot services are also provided. Non-commercial private aircraft are also accommodated and managed.

The CEO has awarded a tender to Irish software development company AirSoft to develop the first module AirMan.

## Project Approach

### Step 1: Creating the ERD Diagram
The first step was to identify the key entities and their attributes based on the project requirements. This was documented in the data definition file, which includes detailed data definitions for each entity.

### Step 2: Designing the Database Schema
Using the identified entities and attributes, an Entity-Relationship Diagram (ERD) was created. The ERD provides a visual representation of the database schema, showing how different entities are related to each other.
<img width="6456" height="6746" alt="AirMan_ERD (2)" src="https://github.com/user-attachments/assets/20387a31-783e-479a-a349-58943a869252" />


### Step 3: Implementing the Database in MySQL
With the ERD as a blueprint, the next step was to implement the database schema in MySQL. This involved creating tables for each entity and defining their relationships.

#### Example Snippet:
<img width="822" height="437" alt="Screenshot 2025-09-01 at 23 15 40" src="https://github.com/user-attachments/assets/22ce528d-d991-4ef0-a614-a2662bb06a1b" />

### Step 4: Verifying the Database Schema
After creating the database schema in MySQL, the schema was reverse-engineered to generate an Entity-Relationship Model (ERM). This step verified that the ERD and ERM models match, ensuring the correct database creation.
<img width="1822" height="1260" alt="AirManERD_reverse_engineering_ERM (1)" src="https://github.com/user-attachments/assets/9679a9f4-26ed-4702-a26a-0c8a6eb4f89d" />

### Step 5: Inserting Data
Mock data was inserted into the tables to demonstrate the system's functionality. This data serves as sample records to test and validate the database operations.

#### Example Snippet:
<img width="1822" height="1260" alt="AirManERD_reverse_engineering_ERM (1)" src="https://github.com/user-attachments/assets/fb38e009-15f5-42c8-9084-767dff852c60" />

### Step 6: Writing SQL Queries for IT Management
The IT management team is interested in important analytics to help them understand and manage the airport operations effectively. Below listed questions were posed, and SQL queries were written to answer these questions.

#### 1. Calculate the landing, service, fuelling, and parking fees for a customer of your choice in February 2024 and indicate if this customer is a corporation.
<img width="822" height="567" alt="Screenshot 2025-09-01 at 23 09 44" src="https://github.com/user-attachments/assets/434765a6-7cae-4a0a-ab51-d65925716453" />

#### 2. List which pilots who are also customers made the most take-offs and landings at the airport in February 2024 and indicate which aircraft they flew by type and registration number.
<img width="820" height="419" alt="Screenshot 2025-09-01 at 23 10 45" src="https://github.com/user-attachments/assets/506d0b3c-37b7-450a-8acf-f5f4085437aa" />

#### 3. List the employees (by employee number, name, and role) who are qualified service personnel who performed routine services on all aircraft owned by a specific corporation in February 2024.
<img width="820" height="419" alt="Screenshot 2025-09-01 at 23 10 45" src="https://github.com/user-attachments/assets/dd59364a-6e96-423f-a193-3f496ebaface" />

#### 4. From the previous list, list all the parts used in a service per aircraft type, part number and part name.
<img width="819" height="444" alt="Screenshot 2025-09-01 at 23 11 40" src="https://github.com/user-attachments/assets/db37485f-7e5a-475d-9d85-02797ea9ff83" />

#### 5. List the names of all aircraft by type, model, and registration number that landed and were refuelled and/or parked and/or cleaned in February 2024 and the total revenue per aircraft and the total revenue to Biggin Hill for that month.
<img width="819" height="499" alt="Screenshot 2025-09-01 at 23 12 12" src="https://github.com/user-attachments/assets/cfbae38d-c855-43ae-a8d3-39dced5c8225" />

## Data Definitions and Normalization
This document provides detailed data definitions for all entities and explains how the database design adheres to the principles of normalization.

## Conclusion
This project aims to design and implement a comprehensive system for managing airport operations within Biggin Hill Airport. By following the structured approach of defining the schema, creating the database, and inserting mock data, the project demonstrates how to manage and analyze airport operations effectively. The SQL queries provide valuable insights and analytics for IT management, ensuring that all operations comply with the airport's policies and are efficiently managed.

For any further information or questions, please refer to the detailed documentation and scripts included in this repository.
