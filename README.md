# API Design

## Database

SQL

## Schema

![schema](<./personid%20(int).png>)
This schema consists of a person, house and address table.

## API

| Path        | HTTP Verb | Action |
| ----------- | --------- | ------ |
| /people     | GET       | index  |
| /people     | POST      | create |
| /people/:id | GET       | show   |
| /people/:id | PUT       | update |
| /people/:id | DELETE    | delete |

- /people => will get personId, name, age and house (which refers to houseId in house table)

| Path       | HTTP Verb | Action |
| ---------- | --------- | ------ |
| /house     | GET       | index  |
| /house     | POST      | create |
| /house/:id | GET       | show   |
| /house/:id | PUT       | update |
| /house/:id | DELETE    | delete |

- /house => will get houseId, address (which refers to addressId in address table), owner, numOfPeople

| Path         | HTTP Verb | Action |
| ------------ | --------- | ------ |
| /address     | GET       | index  |
| /address     | POST      | create |
| /address/:id | GET       | show   |
| /address/:id | PUT       | update |
| /address/:id | DELETE    | delete |

- /address => will get addressId, postcode, streetAddress
