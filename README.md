# Graph Theory      

This repository is for my Graph Theory Project where I was asked to design a Graphical Database using Neo4j for my college Timetable due on 
the 23rd of April.

The requirement was to create  a database storing Lecturers, Room numbers, Modules, Days of the Week, Hours of the day which I Have included
in my Graphical database as nodes.

All of these nodes are connected via a relationship.

The Relationships in my database are as follow = Year - Month - Day - Hours - Groups - Modules - Rooms - Lecturers.

# Why Have I Done So?      

The Reason for the relationship to be in that order is so that everything is well organized and there is no need for separate nodes for each
day of the week.

By connecting these nodes this way the timetable database is sorted out in the same order as they are mentioned above.

# Neo4j
Neo4j (Cypher being the Language) was a tricky to figure out at the start but as I used more and more of it it became very easy and understandable.

The Queries that I used in my database are as follow:

* CREATE (sem1:Year{name:"2016"})
* MATCH (d:Day {name:"Monday"}), (t:Time {name: "9:00"})
  Create (d)-[:AT]->(t)
* MATCH (n) where ID(n)=23 delete n
* MATCH (y:Year {name:"2016"})-[r]-()
  DELETE r
* match (n) return n

  
Match is only an example of one of the relationships I have done where Monday has a time and the relationship is AT for the reason that 
Monday -------AT--------> Time

# Screenshots of Labels
## Database
![DB](https://cloud.githubusercontent.com/assets/15819582/25318036/bb945dd2-287d-11e7-8b4d-09a5863931a0.png)

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

## Days
![Days](https://cloud.githubusercontent.com/assets/15819582/25318037/bb948000-287d-11e7-8118-6737662326e7.png)

# Conclusion

I've learned a lot from doing this project. Firstly I learned a new language (Cypher) and how to use neo4j. Secondly I learned that creating something of this scale is insanely time consuming and requires a lot of patience and concentration not to make mistakes. Thirdly I learned that planning is essential in creating any database of any size.

# References
1. https://neo4j.com/developer/cypher-query-language/
2. https://neo4j.com/docs/developer-manual/current/cypher/clauses/delete/





