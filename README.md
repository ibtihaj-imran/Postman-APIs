
# JSONPlaceholder APIs

JSONPlaceholder is a valuable resource for developers to quickly integrate API functionality into their projects without the need for a fully implemented backend server. It's widely used in the development community for educational, testing, and experimentation purposes.


## Installation

Install JSON Server:

```bash
  npm install -g json-server

```
Create a JSON File:

```bash
  db.json

```
Start JSON Server:

```bash
  json-server --watch db.json

```
## Navigate
  Navigate to  http://localhost:3000 to see the API. You should see links to /Users and /subjects. Navigate to one of these to see user data from JSONPlaceholder.
## Sample JSONPlaceholder

```javascript
{
  "Users": [
    {
      "subjectID": "1",
      "id": "1",
      "firstname": "jhon",
      "lastname": "doe",
      "age": "26"
    },
    {
      "subjectID": "1",
      "id": "2",
      "firstname": "two",
      "lastname": "doe",
      "age": "26"
    }
  ],
  "subjects": [
    {
      "id": "1",
      "name": "automation"
    },
    {
      "id": "2",
      "name": "devops"
    }
  ]
}

```


## Saved Variables
The URL  http://localhost:3000 is saved by {{baseURl}} globaly in the Variables
## Examples Fetching APIs
The following examples use a base URL of http://localhost:3000

### GET (Getting a Resource)
```javascript
{{baseURL}}/Users/1
```
### GET(Listing all Resources)
```javascript
{{baseURL}}/Users
```
### POST (Creating a Resource)
```javascript
{{baseURL}}/Users
```
### Body
```javascript
{
    "subjectId": "6",
    "id": "6",
    "firstname": "ali",
    "lastname": "hamza",
    "age": "33"

}
```
### PUT (Updating a Resource)
```javascript
{{baseURL}}/Users/6
```
### Body
```javascript
{
      "subjectId": "6",
      "id": "6",
      "firstname": "roma",
      "lastname": "james",
      "age": "25"
}
```
### PATCH (Patching a Resource)
```javascript
{{baseURL}}/Users/6
```
### Body
```javascript
{
      "subjectId": "6",
      "id": "6",
      "firstname": "ali",
      "lastname": "hamza",
      "age": "33"
}
```
### DEL (Deleting a Resource)
```javascript
{{baseURL}}/Users/6
```
### GET (Filtering a Resource)
```javascript
{{baseURL}}/subjects?name={{subject}}
```
### GET (LIsting Nested Resources)
```javascript
{{baseURL}}/subjects/1/Users
```
