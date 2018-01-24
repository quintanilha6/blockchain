# Blockchain app
## Description

Getting to know a bit more about decentralized applications, I dived a bit more into blockchain use and so, what better then do one myself?
Following the help of this [example](https://hackernoon.com/learn-blockchains-by-building-one-117428612f46), I ended up finishing a Blockchain for transactions. The app takes a tour through the use and 'how does it work' process, as well as its integrity as a network, making use of Consensus algorithm where the longest valid chain is always authoritative.
I Used postman to test all the functionabilities with HTTP Requests.

## Requisites 

Python 3.6+

Flask

Requests lib

## Run

Set different ports on last lines of blockchain.py, to run the app in different servers.
python blockchain.py (for each port)

#### GET

 /mine - Mine a new block

 /chain - Gets the current chain

 /nodes/resolve - Iterates all nodes and gets the longest if it's a valid one

#### POST

 /transactions/new - Creates a new transaction in the current block

Example of JSON raw body argument:

{
	"sender": "some address",
	"recipient": "some other adress",
	"amount": 6
}

  ----------------------------------------------------
  
 /nodes/register - Registers a new node in a given address
 
Example of JSON raw body argument:

{
	"nodes": ["http://127.0.0.1:5000"]
}
