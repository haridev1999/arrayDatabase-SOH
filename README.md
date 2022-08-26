# arrayDatabase-SOH 

Secret of Happiness was a project with the idea that you can keep track track of your seven Fs responsible for your happiness throughout the various 
points in your life. The seven Fs  being Family, Fitness, Faith, Field, Finance, Fun, Friends

Base Address : https://secretofhappiness-array.herokuapp.com

Endpoints : 3

Endpoint 1 : /create : This is a post request which creates a record in the database. The body should be given in a JSON format and the response will be in a string format.
The input body should be of the format : 
{
	"family":8,
	"fitness":2,
	"faith":2,
	"field":5,
	"finance":5,
	"fun":8,
	"friends":8
}
and you will get a response like this'Data Updated Successfully'.Saying that the data has been updated to the database successfully 

Endpont 2 : /all : This is a get request which is used to retrieve all the records done in the dataase. This endpoint uses no input. And it gives you a response as an array of objects.
For a database containing 2 entries, the response would look something like this :
[
	{
		"family": 8,
		"fitness": 2,
		"faith": 2,
		"field": 5,
		"finance": 2,
		"fun": 8,
		"friends": 8,
		"slNo": 1,
		"date": "2022-08-26T06:08:51.655Z"
	},
	{
		"family": 8,
		"fitness": 2,
		"faith": 2,
		"field": 5,
		"finance": 5,
		"fun": 8,
		"friends": 8,
		"slNo": 2,
		"date": "2022-08-26T06:18:47.777Z"
	}
]

Endpoint 3 : /focus : This is also a get request that retrieves all the areas where your values are less than three and needs your extra focus. 
This endpoint also does not need any input and gives an array of strings as a response. which would look something like this:
["fitness","faith","finance"]
