# FriendFinder

#Week of 13 HW: Friend Finder - Node and Express Servers

### Folder Structure

* Create a folder called FriendFinder. Directories so it matches the following:

	```
	FriendFinder
		- app
			- data
				- friends.js
			- public
				- home.html
				- survey.html
			- routing
				- apiRoutes.js
				- htmlRoutes.js
		- node_modules
		- package.json
        - README.md
		- server.js
	```

# Friend Finder Application

## Description

*Friend Finder* implements friend matching based on the user's responses to a ten question survey. The user responds to questions with values from 1 (Strongly Disagree) to 5 (Strongly Agree). When the survey is submitted, an existing user record closest to the current user's responses is found and returned. The closest set of user responses is defined as the set with the lowest absolute difference for all ten questions combined.

## Convert Metric and Score
   * Convert each user's results into a simple array of numbers (ex: `[5, 1, 4, 4, 5, 1, 2, 5, 4, 1]`).
   * With that done, compare the difference between current user's scores against those from other users, question by question. Add up the differences to calculate the `totalDifference`.
     * Example:
       * User 1: `[5, 1, 4, 4, 5, 1, 2, 5, 4, 1]`
       * User 2: `[3, 2, 6, 4, 5, 1, 2, 5, 4, 1]`
       * Total Difference: **2 + 1 + 2 =** **_5_**


*Friend Finder* application is meant to simulate a simple dating app. The application is implemented using a [Node.js](https://nodejs.org/en/) and [Express](https://expressjs.com/) 

## Demo Heroku
	
*Friend Finder* is deployed to Heroku. Please check it out [here](https://friendfinderyoung.herokuapp.com/)..

## Demo Gitgub

*Friend Finder* is deployed to Git. Please check it out [here](https://github.com/youngtae1386/FriendFinder)..

## Installation - GitHub

To install the application follow the instructions below:

	git clone git@github.com:angrbrd/friend-finder.git
	cd friend-finder
	npm install
	
## Running Locally

To run the application locally and access it in your browser, first set the `PORT` environment variable to the value of your choice. An example is shown below.

	export PORT=3000
	
After the `PORT` environment variable has been set, run the Node.js application with the command below.

	node server.js
	
The application will now be running locally on `PORT`, in this case that is port 3000. You can then access it locally from your browser at the URL `localhost:PORT`, in this case `localhost:3000`.