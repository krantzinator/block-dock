Dockerizing the python blockchain tutorial found [here](https://hackernoon.com/learn-blockchains-by-building-one-117428612f46).

## Instructions

- clone repo
- `cd` into repo
- run `docker build -t dockblock .`
- run `docker run -p 5000:80 dockblock`
- open up your rest client of choice (such as Postman), and hit the following endpoints:
  - GET http://localhost:5000/mine
  - POST http://localhost:5000/transactions/new
    - Body formatted like so:
    ```
    {
	    "sender": "036f66f974cb49aab50bdc86311e1ea5",
	    "recipient": "somewhereselseinspace",
  	    "amount": 3
    }
    ```
  - GET http://localhost:5000/chain
  
