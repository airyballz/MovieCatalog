
Simply run the following commands:

    pip install Flask
	pip install SQLAlchemy
	pip install Flask-GoogleLogin

As the app uses Google for authentication as the next step you have to obtain a client id and client secret from Google:

1. Go to the [Google Developer Console](https://console.developers.google.com/project).
2. Create a new project.
3. Go to **APIs & auth - Consent screen** and select a valid Email address.
4. Go to **APIs & auth - Credentials** and create a new Client ID.
5. Enter **http://localhost:8000/oauth2callback/** in the **Authorized redirect URIs** field.
6. Open the **project.py** file and replace the **<Client ID\>** and **<Client Secret\>** placeholders with your client id and your client secret.

Next you have to create the genres database. To do so run

	python database_setupy.py

To start the app simply run
	
	python project.py
