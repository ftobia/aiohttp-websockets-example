aiohttp websocket example
=========================

This is a simple example of an asyncio websocket server and client using Python 3.6 and the [aiohttp](http://aiohttp.readthedocs.io/en/stable/index.html) library.

Getting started with Docker
---------------------------
If you don't already have Docker installed, [get it here](https://www.docker.com/get-docker).

To start the client and the server, run:

    docker-compose run --rm aiows-client

To start the server independently, run:

    docker-compose up aiows-server

You can test to see if the server is running correctly by visiting `http://localhost:8080/` in your favorite browser.

Getting started without Docker
------------------------------
Make sure [Python 3.6](https://www.python.org/downloads/release/python-360/) or greater is installed.

Create a virtual environment and install dependencies:

    python3.6 -m venv env
    source env/bin/activate
    pip install -r requirements.txt

Run the server:

    python server.py

In a different terminal, run the client:

    source env/bin/activate
    python client.py
