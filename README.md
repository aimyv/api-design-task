# API Design

## Database

SQL

## Schema

![schema](<./personid%20(int).png>)
This schema consists of a person, house and address table.

## API

| Path        | HTTP Verb | Action | Status Code | Response                                               |
| ----------- | --------- | ------ | ----------- | ------------------------------------------------------ |
| /people     | GET       | index  | 200         | Will get all records from the person table             |
| /people     | POST      | create | 201         | Inserts a record into the person table                 |
| /people/:id | GET       | show   | 200         | Will get record (id=personId) from the person table    |
| /people/:id | PUT       | update | 202         | Edits the record (id=personId) from the person table   |
| /people/:id | DELETE    | delete | 204         | Deletes the record (id=personId) from the person table |

| Path       | HTTP Verb | Action | Status Code | Response                                             |
| ---------- | --------- | ------ | ----------- | ---------------------------------------------------- |
| /house     | GET       | index  | 200         | Will get all records from the house table            |
| /house     | POST      | create | 201         | Inserts a record into the house table                |
| /house/:id | GET       | show   | 200         | Will get record (id=houseId) from the house table    |
| /house/:id | PUT       | update | 202         | Edits the record (id=houseId) from the house table   |
| /house/:id | DELETE    | delete | 204         | Deletes the record (id=houseId) from the house table |

| Path         | HTTP Verb | Action | Status Code | Response                                                 |
| ------------ | --------- | ------ | ----------- | -------------------------------------------------------- |
| /address     | GET       | index  | 200         | Will get all records from the address table              |
| /address     | POST      | create | 201         | Inserts a record into the address table                  |
| /address/:id | GET       | show   | 200         | Will get record (id=addressId) from the address table    |
| /address/:id | PUT       | update | 202         | Edits the record (id=addressId) from the address table   |
| /address/:id | DELETE    | delete | 204         | Deletes the record (id=addressId) from the address table |
