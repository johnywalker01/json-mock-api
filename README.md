
# JSON mock API

> This project is for mocking a sample JSON api


## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Reference](#reference)
- [License](#license)


---

## Installation

> install npm packages

```shell
$ npm install
```

## Usage
> To start up your API, run the command below in your terminal:
```shell
$ json-server --watch src/db.json
```

Test your newly created endpoint on any API testing tool, such as Postman or CURL.
> To make a GET request for all employees, run the command below
```shell
$ curl http://localhost:3000/employees
```

The response should be as below. Note that it is an array with all the employees.
```json
[
  {
    "id": 1,
    "first_name": "John",
    "last_name": "Doe",
    "email": "johndoe@abc.com",
    "gender": "Male",
    "status": "Terminated"
  },
  {
    "id": 2,
    "first_name": "Jane",
    "last_name": "Doe",
    "email": "janedoe@abc.com",
    "gender": "Female",
    "status": "Retired"
  },
  {
    "id": 3,
    "first_name": "Alice",
    "last_name": "Doe",
    "email": "alicedoe@abc.com",
    "gender": "Female",
    "status": "Suspended"
  },
  {
    "id": 4,
    "first_name": "Bob",
    "last_name": "Doe",
    "email": "bobdoe@abc.com",
     "gender": "Male",
    "status": "Active"
  }
]
```
To make a GET request for a specific employee, append the `id` of the employee to the endpoint `/employees/4`. You can then run the command below.
```shell
$ curl http://localhost:3000/employees/4
```
The response should be as below. Note that it is an object with the specific employee details of the employee whose `id` is 4.
```json
{
  "id": 4,
  "first_name": "Bob",
  "last_name": "Doe",
  "email": "bobdoe@abc.com",
  "gender": "Male",
  "status": "Active"
}
```
## Reference
To learn more about the tool, have a look at the <a href="https://github.com/typicode/json-server" target="_blank">JSON Server Documentation</a>.


## License

[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)

- **[MIT license](http://opensource.org/licenses/mit-license.php)**