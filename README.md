# API Design

## Database

SQL

## Schema

![schema](<./personid%20(int).png>)

## API

| Path        | HTTP Verb | Action |
| ----------- | --------- | ------ |
| /people     | GET       | index  |
| /people     | POST      | create |
| /people/:id | GET       | show   |
| /people/:id | PUT       | update |
| /people/:id | DELETE    | delete |

- /people => will get personId, name, age and houseID
