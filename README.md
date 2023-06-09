# Agile
Agile is an iterative way to project management and software development that helps teams deliver products faster. Instead of developing complete project and then launch it a once, an agile team delivers work in a small and incremental way.

`Sprint`:`(cycle)`
A sprint is a short time period in which a scrum team works to complete a set amount of work.
A sprint can be of 1 week, 2 weeks or max 3 weeks in Agile Methodology

`Sprint Planning and Estimation`:
Sprint planning is a first meeting in the sprint. The purpose of sprint planning and estimation is to define what all tasks can be delivered in the sprint.
The product owner set the goal of the sprint, development team then estimates the task (how much time the task will take to complete) and plans who will work on what.

`Q1. What if task required more time than sprint time?`
--- In this case we again divide task into smaller part or tasks.
`Q2. What if task is taking more time than expected time or not completed in sprint.`
-- We spill over it to another sprint with valid explanations or reasons.
`Q3. Story point?`
- 13 means complete sprint
- 8 means 7 working days
- 5 means  5 working days
- 3 means 2-3 days

`Q) What are scrum ceremonies?`
- Sprint planning and estimation
- Daily stand-up
- Sprint review
- Retrospect meeting
- Backlog grooming


`Daily stand-up`:
What we did yesterdat, what we are planning to do today and any roadblocks to do todays task

`Sprint review`:
This meeting happens generally at the end of spring and In this meeting the team show what we have developed in this sprint and receives early feedback.

`Retrospect meeting`:
The is the last meeting of the sprint, in this meeting the team discuss What all good things are done by team, What all things we learned, what all thing team did not do well and discuss action items to improve the mistakes in this spring.

`Backlog grooming`:
Backlog grooming is a regular Meeting where backlog items are discussed, reviewed, and prioritized by product managers, product owners, and the rest of the team. The primary goal of backlog grooming is to keep the backlog up-to-date and ensure that backlog items are prepared for upcoming sprints.


~~Release cycle: In our company, we have a monthly release cycle.~~


# Docker
#### Docker config file

```
FROM openjdk:17(jdk version of project)
ADD/COPY target/JAR_FILE_NAME YOUR_NEW_NAME_FOR_JAR_FILE(This can be kept same as original)
ENTRYPOINT ["java", "-jar", "Your new jdk file name from above line"] 
```

Docker commands
- `docker images` - to check all the images
- `docker build -t 'name of image you want to give':'tag name' .` (this dot at the end says that jar is present in the root dirctory)   -> this is to create image
- `docker run -p new_port_number:current_port_number image_name_to_run_on_docker` -> this is to run docker image on docker container
- `docker rmi -f $(docker images -aq)` -> to remove all iamges
- `docker rm -f $(docker ps -aq)` -> to remove all container
- `docker pull`
