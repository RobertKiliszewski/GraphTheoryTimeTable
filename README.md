# Graph Theory      

This repository is for my Graph Theory Project where I was Asked to design a Graphical Database using Neo4j for my college Timetable due on 
the 23rd of April.

The requirement was to create  a database storing Lecturers, Room numbers, Modules, Days of the Week, Hours of the day which i Have included
in my Graphical database as nodes.

All of these nodes are connected via a relationship.

The Relationships in my database are as follow = Year - Month - Day - Hours - Groups - Modules - Rooms - Lecturers.

# Why Have I Done So?      

The Reason for the relationship to be in that order is so that everything is well organized and there is no need for separate nodes for each
day of the week.

By connecting these nodes this way the timetable database is layed out in the same order as they are mentioned above.

# Neo4j
Neo4j was a tricky language to fgure out at the start but as I used more and more of it it became very easy and understandable.

The Queries that I used in my database are as follow:

* CREATE (sem1:Year{name:"2016"})
* MATCH (d:Day {name:"Monday"}), (t:Time {name: "9:00"})
  Create (d)-[:AT]->(t)
* MATCH (n) where ID(n)=23 delete n
* MATCH (y:Year {name:"2016"})-[r]-()
  DELETE r
  
Match is only an example of one of the relationships I have done where Monday has a time and the relationship is AT for the reason that 
Monday -------AT--------> Time

# Screenshots of Labels
## Groups
![Groups](https://cloud.githubusercontent.com/assets/15819582/25318030/bb6283ac-287d-11e7-8200-d569bd12516a.png)

## Lecturers
![Lecturers](https://cloud.githubusercontent.com/assets/15819582/25318031/bb7ae0c8-287d-11e7-8bd6-fc72a0e0e277.png)

## Modules
![Modules](https://cloud.githubusercontent.com/assets/15819582/25318032/bb920a46-287d-11e7-8b90-5dcf8d5dd8f7.png)

## Months
![Months](https://cloud.githubusercontent.com/assets/15819582/25318033/bb921f40-287d-11e7-8894-e46f9131611b.png)

## Rooms
![Rooms](https://cloud.githubusercontent.com/assets/15819582/25318035/bb92e9fc-287d-11e7-9574-b9eb2d9079fa.png)

## Times
![Times](https://cloud.githubusercontent.com/assets/15819582/25318034/bb929dd0-287d-11e7-8523-dda3c1d2565b.png)




