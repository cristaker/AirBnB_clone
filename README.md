# 0x00. AirBnB clone - The console


![alt text](https://user-images.githubusercontent.com/33245729/41383392-58f3dbb8-6f25-11e8-8215-d7c3832c0ae8.png)

## Description


Team Project as part of the second trimester cicle of foundations at Holberton School, the AirBnB project approachs to the first real web developer project, the console is the first step towards building our first full web application: the AirBnB clone. This first step is very important because you will use what you build during this project with all other following projects: HTML/CSS templating, database storage, API, front-end integration.

## Resources


### Read or watch:

* [Python abstract classes](https://blog.teclado.com/python-abc-abstract-base-classes/)
* [cmd module](https://docs.python.org/3.4/library/cmd.html)
* Packages concept page
* [uuid module](https://docs.python.org/3.4/library/uuid.html)
* [datetime](https://docs.python.org/3.4/library/datetime.html)
* [unittest module](https://docs.python.org/3.4/library/unittest.html#module-unittest)
* [args/kwargs](https://yasoob.me/2013/08/04/args-and-kwargs-in-python-explained/)
* [Python test cheatsheet](https://www.pythonsheets.com/notes/python-tests.html)

# More Info


## Execution

The AirBnb Shell runs in both interactive and non interactive mode:

### Interactive
```
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb)
(hbnb)
(hbnb) quit
$
```
### Non-Interactive
```
$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
```

## Usage

The console works both in interactive mode and non-interactive mode, much like a Unix shell. It prints a prompt (hbnb) and waits for the user for input.

Command | Example
---|---
Run the console | ./console.py
Quit the console | (hbnb) quit
Display a help for a command | (hbnb) help (command)
Create an object | (hbnb) create (class)
Show an object | (hbnb) show (class)(id)
Destroy an object | (hbnb) destoy (class) (id)
Show all objects, or all instances of a class | (hbnb) all or (hbnb) all (class)
Update an attribute of an object | (hbnb) update (class) (id) (attribute name) (attribute value)

## Models

All classes used in this project

File | Description | Attributes
---|---|---
[base_model.py](/models/base_model.py) | BaseModel for all classes | id, created_at, updated_at
[user.py](/models/user.py) | User class for the future user information | password, first_name, last_name
[amenity.py](/models/amenity.py) | Amenity class for the future amenity information | name
[city.py](/models/city.py) | City class for future location information | name, state_id
[state.py](/models/state.py) | State class for future accomodation information | name
[place.py](/models/place.py) | Place class for future location information | city_id, user_id, name, description, number_rooms, number_bathrooms, max_guest, price_by_night, latitude, longitude, amenity_ids
[review.py](/models/review.py) | Review class for future user/host review information | place_id, user_id, text


## Authors


[Cristian Sánchez](https://github.com/cristaker)

[Diego Fernando Jojoa Yandún](https://github.com/diegojojoayandun)
