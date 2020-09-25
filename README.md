## What is this?
This is just a simple server providing products API.

## How to start?
The simplest way to run the server is to use docker container. 

```bash
docker run -d -p 3000:80 -v "$PWD"/server/db.json:/data/db.json clue/json-server
``` 
Api provides a list of 10 000 products on route `http://localhost:3000/products`

You can read more about the `api` [here](https://github.com/typicode/json-server).
 - `http://localhost:3000/products/_limit=10` - will provide only 10 products 
 - `http://localhost:3000/products?_limit=10&_start=10` - will provide next 10 products 
