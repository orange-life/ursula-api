# Ursula API

Exposes [Umbral](https://github.com/nucypher/pyUmbral)'s re-encryption proxy (an "Ursula") as an HTTP API. Obviously, this works off the chain but is distributed.

## Requirements

 - Python 3, pip 3
 - `pip install -r requirements.txt`

## Usage

 - `uvicorn app:app --reload` for development
 - `uvicorn app:app` for something resembling production

## Caveats

 - No built-in node discovery - this means you'll need a list of known nodes. Adding more nodes requires a change in this list in all the clients that are using it.
 - No blockchain level guarantees
