# Project Item-Catalog
Create a restaurant menu app where users can add, edit, and delete restaurants and menu items in the restaurants.

## Setup and run the project
### Prerequisites
* Python 2.7
* Vagrant 1.9.1
* VirtualBox 2.5.5

##Vagrant & Virtualbox Config
```
https://github.com/udacity/fullstack-nanodegree-vm
```

### Google Credentials
```
- Update client_secrets.json file with
```
- Client Secret
```
- Client ID
```
- Project ID
```
```

** These are available in your Google API Console.

### How to Run
1. Install VirtualBox and Vagrant
2. Place the Item Catalog folder in your Vagrant directory
3. Launch Vagrant

```
$ Vagrant up 
```

5. Login to Vagrant
```
$ Vagrant ssh
```
```
6. Change directory to `/vagrant`
$ Cd /vagrant
```

7. Initialize the database
```python
$ Python database_setup.py
```

a. Install the required Oauth Clients from Google

```
pip install --upgrade google-api-python-client oauth2client
```

8. Populate the database with some initial data
```python
$ Python menus.py
```

9. Launch application
```python
$ Python project.py
```

10. Open the browser and go to http://localhost:5000


### JSON endpoints
#### Returns JSON of all restaurants

```
/restaurants/JSON
```
#### Returns JSON of specific menu item

```
/restaurants/<int:restaurant_id>/menu/<int:menu_id>/JSON
```
#### Returns JSON of menu

```
/restaurants/<int:restaurant_id>/menu/JSON

```


#### References
https://github.com/udacity/fullstack-nanodegree-vm

