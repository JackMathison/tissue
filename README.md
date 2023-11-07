# MIST 4610 Group Project

# Group Members
1. Jack Mathison
2. John Hulsey
3. Carson Whitt
4. Marco Young
5. Hayes Herzog

# Problem Description

The task at hand is to model and build a relational database for the general workings of a football team. The central entity in the model is the 'team' entity. The team operates in conjunction with players, staff, coaches in order to track equipment, injuries, events, donations, and rental of facilities. We are interested in modeling these relationships and populating the entities and their attributes with sample data. We are also interested in performing functioning queries on the data so that we can generate reports and build insight about operations within the football team.

# Data Model

In this football team database, the entities represent the various aspects and participants involved in managing a football organization. Each entity is equipped with attributes that provide details essential to the organization's operation, such as personal information, roles, and activities within the team structure.

The team entity holds central information about each football team, including its unique identifier, name, average age of players, mascot, and the captain's name. It is directly related to several other entities that provide a comprehensive view of the team's functioning. For instance, each team is associated with multiple staff members; this one-to-many relationship indicates that a team has various staff members fulfilling different roles, identified by their names, contact information, and specific position within the team.

Coaches are crucial to a team's performance and are tracked in the database by their full name, experience, specialty, and contact info. Each coach is linked to one football team, following the one-to-many relationship paradigm, suggesting that while a coach is dedicated to a single team, the team could have multiple coaches, one or many for different aspects of the game such as offense, defense, and special teams.

The player entity captures detailed information on every individual player, including their first and last name, date of birth, contact info, and position on the team. Each player is associated with one team, hinting at an exclusive contract situation. While a player can only play for one team, by nature, a team has multiple players.

Sponsor entities are external supporters of the football team. They are detailed by their name and contact information. Sponsors are linked to donations, where each sponsor can make multiple donations, but each donation is specifically tied to one sponsor and one team, emphasizing the targeted support sponsors provide to the teams.

Donations are financial contributions made by sponsors, recorded with details such as the amount, date, and the related sponsor and team. The entity reflects the financial support structure behind sports teams, with many donations potentially supporting a single team.

Football teams require equipment, and the equipment entity tracks each item by name, quantity, and condition. Players use the equipment, which leads to the equipment_checkout entity, indicating a many-to-one relationship where multiple pieces of equipment are checked out by players over time. The checkout process is logged with dates for accountability and management.

Players may, unfortunately, suffer injuries, which are recorded in the specific_injury entity. This entity captures the association between a player and their injury, the type of which is detailed in the injury entity. Injuries are characterized by the affected body part and the severity, acknowledging that one injury type can be associated with multiple instances of player injuries.

The facility entity manages the locations where football activities occur, including their name, type (e.g., stadium, training ground), and availability. Facilities are rented for events, as tracked by the rental_of_facility entity, which also logs the renting party's name and contact information. Since multiple facilities might be rented for a single event, such as a tournament, this creates a one-to-many relationship with the event entity.

Lastly, events are any significant occurrences, like games or tournaments, associated with the team. The event entity captures details like the event's name, date, type (e.g., game, practice, meeting), and result.

Overall, this football team database is designed to comprehensively represent and manage the complex interactions, activities, and components that make up a professional football team's ecosystem. From the individuals who play, coach, and manage, to the logistical elements of equipment and facilities, the database's entities and their interrelationships provide a structured insight into the team's operations.

![280933374-689f3f19-eb51-4e6c-9147-0c7bc3c6946d](https://github.com/JackMathison/tissue/assets/148248948/fc1fb6d6-86b9-4368-accd-3b3ce0362f1b)
![280935441-1eb363f5-3d52-4f7c-9ee3-f41c403d2428](https://github.com/JackMathison/tissue/assets/148248948/14c6ed8b-8537-4bed-9061-4958c8669d68)
![280935527-a1e044e3-de85-4c12-8b80-e358c739294f](https://github.com/JackMathison/tissue/assets/148248948/39f6eedf-dc93-4aaa-aeae-e81886655dd8)
![280935564-60528420-6ece-4f74-92fd-df8e78855b93](https://github.com/JackMathison/tissue/assets/148248948/c191ec9c-5804-4062-b319-c284d4f1ae15)
![280935639-0362cbcb-48e0-4134-9fef-0411f4154b36](https://github.com/JackMathison/tissue/assets/148248948/6c0421e6-e7ad-4571-82f8-acd1643af214)
![280935692-c5596454-aadc-485e-b67f-33de52033296](https://github.com/JackMathison/tissue/assets/148248948/4eb0ca37-de45-42dd-a71d-4c6e3a8adc83)
![280935736-18fcadc3-d25a-487d-b849-84b38ecaef84](https://github.com/JackMathison/tissue/assets/148248948/7fcff337-9847-4466-bb29-7f0f49351e83)
![280935811-3505ecaa-a985-4089-8d85-249b3601473d](https://github.com/JackMathison/tissue/assets/148248948/e339028c-5fb9-4f4f-b99b-44545d7136fb)
![280935854-46848010-25ab-4b27-af28-bb04963fdeba](https://github.com/JackMathison/tissue/assets/148248948/a6c9aadd-18c4-4a42-9dd6-b332f29418d2)
![280935943-c12eb111-9d7b-45ff-9a66-16acb3f4c9c5](https://github.com/JackMathison/tissue/assets/148248948/b4e293ba-0f19-413f-a5a6-1e894b8907e5)
![280935989-27d93c9d-e4d5-4825-8ff1-4b0307e3dc9b](https://github.com/JackMathison/tissue/assets/148248948/bb21375a-ee6b-486f-9b95-fbc1b40e5e3e)
![280936026-b4964f17-dad2-48a4-a9b7-e6046d6494f6](https://github.com/JackMathison/tissue/assets/148248948/0344f131-2f36-492c-bc8b-68ea13fa0d9b)
![280936110-6587a198-e53e-420b-9d81-e57d4b9e70ff](https://github.com/JackMathison/tissue/assets/148248948/8e009fed-f047-46b3-aeca-aa33473215e7)
![280936139-4b776c94-09cd-4acf-83ec-82a34adbb244](https://github.com/JackMathison/tissue/assets/148248948/f7a72114-dedb-43eb-b934-3c911d33e29a)
