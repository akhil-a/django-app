Steps to run django server

1. create a folder named project
2. build or run the docker compose file
	docker-compose build
	or
	sudo docker-compose run server django-admin startproject project .
3. Connect database. Edit the file project/settings.py like below
	DATABASES = {
 	   'default': {
        	'ENGINE': 'django.db.backends.postgresql',
        	'NAME': 'postgres',
        	'USER': 'postgres',
        	'HOST': 'db',
        	'PORT': 5432,
    	   }
	}
4. Start the containers using up command
	docker-compose up
