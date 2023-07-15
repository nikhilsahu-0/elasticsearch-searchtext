# elasticsearch-searchtext
Welcome to the elasticsearch-searchtext repository! This repository contains the source code 
for text-search REST API with nodejs.

## Prerequisites
Before running this project, ensure that you have the following prerequisites installed on your
local system:

Docker [https://www.docker.com/get-started]

## Getting Started

To get started with the project, follow the steps below:
### 1. Clone the repository to your local machine:
   ```
   git clone https://github.com/nikhilsahu-0/elasticsearch-searchtext.git
   ```
### 2. Change into the project directory:
   ```
   cd elasticsearch-searchtext
   ```
### 3. Build and start the project using Docker Compose:
   ```
   docker-compose up
   ```
This command will download the necessary dependencies, build the project, and start the server.
By default, the server will be accessible at http://localhost:3000.
### 4. Verify that the server is running:
Open your preferred api testing tool like `postman` make a http request
  ```
  GET localhost:3000/quotes?text=love&limit=3&page=2
  ```
or any terminal like `power shell` on pc and make cURL calls
  ```
  curl localhost:3000/quotes?text=good&limit=10&page=2
  ```
If the server is running successfully, you should see a json response.
### 5. Elasticsearch will be exposed on port 9200. You can access it using the following URL: http://localhost:9200.

## Configuration

The project provides a few configuration options that you can modify based on your requirements. These configurations can be found in the docker-compose.yml file:
```
SERVICE_NAME: The name of the service/container.
SERVICE_PORT: The port on which the server will listen.
ELASTICSEARCH_PORT: The port on which Elasticsearch will be exposed.
```
Feel free to adjust these configurations as needed.
