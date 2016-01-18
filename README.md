# Tournament Results
Udacity Full Stack Web Development - Project 3: Item Catelog
## Synopsis

This is my third in a series of projects through Udacity's **Full Stack Web Development** course.  For this project I have developed an application that provides a list of items within a variety of categories, as well as provide a user registration and authentication system.

## Important Files / Folders

* **Vagrantfile :** Contains vagrant machine
* **pg_config :** configuration for vagrant machine
* **application.py :** Python script with main Flask application
* **database_setup.py :** Python script for sqlalchemy schemas
* **client_secrets.json :** JSON formatted file containing OAuth information for Google login
* **static :** Folder that contains css, fonts, js and images
* **templates :** Folder that contains all HTML templates

## Instructions

1. Install [Vagrant](http://vagrantup.com/) and [VirtualBox](https://www.virtualbox.org/)
2. Clone this repository

```
$ git clone https://github.com/Mec-iS/nanodegree-fullstack-final
```

3. Optional: Replace `client_secrets.json` with JSON from Google project
4. Optional: If you replaced `client_secrets.json` you'll need to replace `data-clientid` on line 61 in `login.html`
4. Launch the Vagrant VM
	1. Open shell and navigate to vagrant folder
	2. Type `vagrant up`
5. SSH into the Vagrant VM
	1. Type `vagrant ssh`
6. Navigate to the correct folder ie `cd /vagrant/catalog`
7. Initialize the databse
	1. Type `python database_setup.py` (Note that the database is empty by default)
8. Run the Flask web server
	1. Type `python application.py`
9. In your browser visit `http://localhost:5000` to view the application (note that you will not be able to add/edit/delete items unless logged in)
