# SpringBootRestApi
As a part of my learning Java journey, I followed a tutorial on creating a basic SpringBoot REST API.

## Prerequisits 
A suitable editor that will run Java applications.
A REST client such as Insomnia - https://insomnia.rest/

## Run
Clone this repo. 
Install dependencies and Run. 
The Application will run on port localhost:8080.
You will first need to make a POST request with a JSON body to further interact with the api. It should look something similar to:
`
{
	"name" : "firstName lastName"
}
`

## Methods

#### POST /api/v1/person
Returns an empty body and 200 repsonse code. The request accepts a JSON body in the format:
`
{
	"name" : "firstName lastName"
}
`

#### GET /api/v1/person

returns a list of all people stored.

#### GET /api/v1/person/:id
returns a person by id

#### DELETE /api/v1/person/:id
returns an empty body. Indicates a successful request with a 200 response code.

#### PUT /api/v1/person/:id
This Method allows you to replace a name. Add the id of the person you want to change to the end of the url and pass a JSON body:
`
{
	"name" : "firstName lastName"
}
`
You will recieve a 200 response code and an empty body. You can check that this has worked by calling a GET to: /api/v1/person
