# Django-Vue

- Private Suggestions Portal collaboratively by utilizing Django Rest Framework 3 for the backend and VueJS 3, with Pinia for the frontend. This platform enables users to submit suggestions and vote, on them. The project is stored in an repository and launching it requires minimal setup. The code is designed to be review friendly facilitating effortless deployment.

## Installation with Docker

Build and start on wsl only

```bash
 docker-compose up --build
```

To create superuser run in another wsl

```bash
docker exec -it inventar-django /bin/bash

python manage.py createsuperuser

```

## Frontend Installation

```bash
  cd Django-Vue/front
```

Install the required Node.js packages:

```bash
  npm install
```

Start the frontend app:

```bash
  npm run dev
```

## Backend Installation

Open a new terminal and go to the backend directory:

```bash
  cd Django-Vue/reviews
```

```bash
python -m venv env

.\env\Scripts\activate
```

Install Django Packages

```bash
  pip install djangorestframework django-cors-headers
```

```bash
  python manage.py migrate
```

Create a superuser for the Django project:

```bash
  python manage.py createsuperuser
```

```bash
  python manage.py runserver
```
