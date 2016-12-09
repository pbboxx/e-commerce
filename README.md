Django E-commerce
======


Usage
-----
Clone the repository (or use your own fork):

$ git 
Enter the directory:

$ cd e-commerce/
Install all dependencies:

$ pip install -r requirements.txt
Set SECRET_KEY environment variable.

Note

Secret key should be a unique string only your team knows. It’s serious as this key is used to ensure security of your installation. Consult Django’s documentation for details.

We try to provide usable default values for all of the settings. We’ve decided not to provide a default for SECRET_KEY as we fear someone would inevitably ship a project with the default value left in code.
$ export SECRET_KEY='<mysecretkey>'
Prepare the database:

$ python manage.py migrate
Install front-end dependencies:

$ npm install
Note

If this step fails go back and make sure you’re using new enough versions of Node.js and npm.
Prepare front-end assets:

$ npm run build-assets
Run like a normal django project:

$ python manage.py runserver


