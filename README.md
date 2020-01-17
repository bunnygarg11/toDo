# Node Todo App

A Node app built with MongoDB, Mocha and swagger. For demonstration purposes only.

- Node provides the RESTful API. 
- Swagger for API documentation. 
- MongoDB to store data.
- Mocha and Chai for testing node API
- Seeding dummy data

## Requirements

- [Node and npm](http://nodejs.org)
- MongoDB: Make sure you have your own local or remote MongoDB database URI configured.

## Installation

1. Clone the repository
2. Go to app directory `cd todo`
3. Install the application: `npm install`
4. Edit env file according to your configuration(if required) `.env`
5. To populate dummy data set `SEED_DB = true` in `.env` file
6. Start the server: `node server/app.js`
7. View in browser at `http://localhost:3000`
8. To run test: `npm test`

## Application comprise of two module : 
# CSV Data Import Module Feature 
- Contain list of client in `client collection`.
- Import request from CSV file URL into `order collection`.
- Only import request of clients(present in client collection).
- Check CSV file url validation.
- Check the data format of CSV.

# Assign Request To Butler Module Feature
- Contain list of request in `request collection`.
- Allocates requests to butlers.
- Each individual client should be allocated to one butler as much as possible.
- Each butler has a maximum of 8 working hours.
