# ItemsCatalog
Restaurants and Menu items


Prerequisites :
Python 3.0
Vagrant
VirtualBox


Steps to run :

1) Install VirtualBox and Vagrant
2) Clone this repo
3) Unzip and place the Item Catalog folder in your Vagrant directory
4) Launch Vagrant
    $ Vagrant up 
5) Login to Vagrant
    $ Vagrant ssh
6) Change directory to /vagrant
    $ Cd /vagrant
7) Initialize the database
    $ Python database_setup.py
8) Populate the database with some initial data
    $ Python database_populator.py
9) Launch application
    $ Python project.py
10) Open the browser and go to http://localhost:5000


JSON endpoints
Returns JSON of all restaurants
    /restaurants/JSON
Returns JSON of specific menu item
    /restaurants/<int:restaurant_id>/menu/<int:menu_id>/JSON
Returns JSON of menu
    /restaurants/<int:restaurant_id>/menu/JSON
