# Django Channels Sample 

## Prerequisite
- Python 3.10 and greater
- Postgres
- Redis (Optional. For django channel layer)
- virtualenv (Optional but strongly encourage)

## Installation
- First copy the content in .env.example to .env file at root dir
- Fill in the value for .env
- Then run:
> python -m pip install -r requirements.txt
- Then run:
> python app/manage.py migrate
- Then run:
> python app/manage.py runserver
- Now access your app at http://localhost:8000/

## Usage
- Your app will have 2 main API doc embedded in:
1. http://localhost:8000/api/schema/redoc
2. http://localhost:8000/api/schema/swagger-ui

This will include all the API registered to the main router

- To test on the websocket, please access:
1. http://localhost:8000/chat

Enter the room name and you can start chat using websocket.
