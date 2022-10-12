# API Design

## Database

SQL

## Schema

![schema](<./personid%20(int).png>)
This schema consists of a person, house and address table.

## API

| Path        | HTTP Verb | Action | Status Code |
| ----------- | --------- | ------ | ----------- |
| /people     | GET       | index  | 200         |
| /people     | POST      | create | 201         |
| /people/:id | GET       | show   | 200         |
| /people/:id | PUT       | update | 202         |
| /people/:id | DELETE    | delete | 204         |

- /people => will get personId, name, age and house (which refers to houseId in house table)

| Path       | HTTP Verb | Action | Status Code |
| ---------- | --------- | ------ | ----------- |
| /house     | GET       | index  | 200         |
| /house     | POST      | create | 201         |
| /house/:id | GET       | show   | 200         |
| /house/:id | PUT       | update | 202         |
| /house/:id | DELETE    | delete | 204         |

- /house => will get houseId, address (which refers to addressId in address table), owner, numOfPeople

| Path         | HTTP Verb | Action | Status Code |
| ------------ | --------- | ------ | ----------- |
| /address     | GET       | index  | 200         |
| /address     | POST      | create | 201         |
| /address/:id | GET       | show   | 200         |
| /address/:id | PUT       | update | 202         |
| /address/:id | DELETE    | delete | 204         |

- /address => will get addressId, postcode, streetAddress
