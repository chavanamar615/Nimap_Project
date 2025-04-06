## Client-Project Management API ##
This is a Django REST API that helps manage clients, their projects, and assigned users.
You can create clients, assign projects, and view projects for logged-in users.

Features:-
Create, update, delete clients
Create and assign projects to clients
Assign registered users to projects
List projects assigned to the logged-in user
Filter projects by client ID

Installation:-
Clone the repository:
git clone https://github.com/chavanamar615/Nimap_Project.git
cd Nimap_Project
Create a virtual environment:
python -m venv env
source env/bin/activate  # For Windows: env\Scripts\activate
Install dependencies:
pip install -r requirements.txt
Apply migrations:
python manage.py migrate
Create a superuser (admin):
python manage.py createsuperuser
Run the server:
python manage.py runserver

API Endpoints:-
GET /clients/ – List all clients
POST /clients/ – Create a new client
GET /clients/:id/ – Retrieve a client
DELETE /clients/:id/ – Delete a client
POST /clients/:id/projects/ – Create a project for a client
GET /projects/ – List all projects for the logged-in user
GET /projects/?client_id=ID – Filter projects by client

Author:-
Amar




