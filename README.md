# MongoDB Fundamentals Assignment - Bookstore

## Overview

This project contains scripts to populate a MongoDB database with sample book data and example MongoDB queries to interact with the data.

## Prerequisites

- [Node.js](https://nodejs.org/) installed on your machine
- A running MongoDB instance (default connection is to `mongodb://127.0.0.1:27017/`)
- MongoDB shell or MongoDB Compass to run queries

## Setup and Running the Scripts

### 1. Populate the Database with Sample Books

The `insert_books.js` script connects to your local MongoDB instance, drops the existing `books` collection if it exists, and inserts sample book data.

To run the script:

```bash
node insert_books.js
```

Make sure your MongoDB server is running before executing the script.

If you want to use a different MongoDB connection URI (e.g., MongoDB Atlas), update the `uri` variable in `insert_books.js` accordingly.

### 2. Running MongoDB Queries

The `queries.js` file contains example MongoDB queries for various operations such as finding, updating, deleting, aggregating, and indexing books.

You can run these queries in the MongoDB shell or MongoDB Compass.

For example, to run the queries in the MongoDB shell:

1. Start the MongoDB shell by running:

```bash
mongo
```

2. Switch to the `plp_bookstore` database:

```js
use plp_bookstore
```

3. Copy and paste the queries from `queries.js` into the shell to execute them.

## Notes

- The sample data includes a variety of books with different genres, authors, and publication years.
- The queries demonstrate common MongoDB operations and aggregation pipelines.
- Modify the scripts and queries as needed for your own use cases.

## Troubleshooting

- Ensure MongoDB is running and accessible at the connection URI specified in `insert_books.js`.
- If you encounter connection issues, verify your MongoDB server status and network settings.

## License

This project is for educational purposes.
