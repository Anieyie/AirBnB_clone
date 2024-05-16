# AirBnB Clone Project

### Project Description
Welcome to the AirBnB clone project! This project is the first step towards building a complete web application similar to AirBnB. In this project, we will develop a command interpreter to manage AirBnB objects. The command interpreter will serve as the foundation for future enhancements, including HTML/CSS templating, database storage, API development, and front-end integration.

**The command interpreter will allow us to:**

Create a new object (e.g., a new User or Place)
Retrieve an object from a file
Perform operations on objects (e.g., count, compute stats)
Update attributes of an object
Destroy an object


## Command Interpreter
### How to Start It
To start the command interpreter, you need to execute the console.py file. The interpreter can be run in both interactive and non-interactive modes.

### Interactive Mode
To start the command interpreter in interactive mode, run the following command:
__$ ./console.py__

You should see the prompt (hbnb) indicating that the command interpreter is running and waiting for your commands.

### Non-Interactive Mode
You can also run the command interpreter in non-interactive mode by piping commands directly into it. For example:

$ echo "help" | ./console.py

## How to Use It
Once the command interpreter is running, you can use various commands to manage your AirBnB objects. The following commands are available:
help: Displays a list of available commands.
quit: Exits the command interpreter.
EOF: Exits the command interpreter.
create <class_name>: Creates a new instance of a class.
show <class_name> <id>: Displays the string representation of an instance based on the class name and id.
destroy <class_name> <id>: Deletes an instance based on the class name and id.
all [<class_name>]: Displays all instances of a class. If no class name is provided, displays all instances.
update <class_name> <id> <attribute_name> <attribute_value>: Updates an instance based on the class name and id by adding or updating an attribute.

**Examples**
Below are some examples of how to use the command interpreter.

Example 1: Creating a New User
$ ./console.py
(hbnb) create User
<new_user_id>
(hbnb) quit

Example 2: Showing a User
$ ./console.py
(hbnb) show User <user_id>
[User] (<user_id>) {'id': '<user_id>', 'created_at': '<creation_time>', 'updated_at': '<update_time>', ...}
(hbnb) quit

Example 3: Updating a User's Name
$ ./console.py
(hbnb) update User <user_id> name "John Doe"
(hbnb) show User <user_id>
[User] (<user_id>) {'id': '<user_id>', 'created_at': '<creation_time>', 'updated_at': '<update_time>', 'name': 'John Doe', ...}
(hbnb) quit

Example 4: Deleting a User
$ ./console.py
(hbnb) destroy User <user_id>
(hbnb) quit

Example 5: Viewing All Users
$ ./console.py
(hbnb) all User
[User] (<user_id_1>) {'id': '<user_id_1>', 'created_at': '<creation_time_1>', 'updated_at': '<update_time_1>', ...}
[User] (<user_id_2>) {'id': '<user_id_2>', 'created_at': '<creation_time_2>', 'updated_at': '<update_time_2>', ...}
(hbnb) quit


**Requirements**
Python 3.8.5
Works on Ubuntu 20.04 LTS

Installation
Clone the repository:
git clone https://github.com/your_username/AirBnB_clone.git
Navigate to the project directory:
cd AirBnB_clone
Make the console.py script executable:
chmod +x console.py

**Running Tests**
Unit tests are provided for all major functionalities. To run the tests, execute the following command:
$ python3 -m unittest discover tests

## AUTHORS
Anieyie Asuquo - https://github.com/Anieyie/
Faith-Jackson - https://github.com/Faith-Jackson/
