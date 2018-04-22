To install json-server user:
    $ npm install -g json-server

The data available in the server is specified in the file db.json

Example of valid of json

{
    "drivers": [
        {
            "id": 1,
            "name": "Carlos",
            "age": 21,
            "email": "carlos@vw.com"
        },
        {
            "id": 2,
            "name": "Paco",
            "age": 32,
            "email": "paco@vw.com"
        }
    ],
    "crafters": [
        {
            "id": 1,
            "model": "VW Crafter",
            "plates": "FGH 7548"
        }
    ]
}

To run the server, use:
    $ json-server db.json

You will be able to use restful requests in the routes "crafters" and "drivers". Example:
GET http://localhost:3000/crafters
GET http://localhost:3000/crafters/1
POST http://localhost:3000/crafters
PUT http://localhost:3000/crafters/1
DELETE http://localhost:3000/crafters/1

You can save the current state of the json file, with modifications (insertions and deletions).
By pressing s + enter at any time while the server is running.

Video tutorial
https://egghead.io/lessons/javascript-creating-demo-apis-with-json-server