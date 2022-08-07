# 0x00. AirBnB clone - The console
`Group project` `Python` `OOP`

### Concepts
For this project, we expect you to look at these concepts:

- [Python packages](https://alx-intranet.hbtn.io/concepts/66)
- [AirBnB clone](https://alx-intranet.hbtn.io/concepts/74)

# Background Context
*Welcome to the AirBnB clone project!*
Before starting, please read the *AirBnB* concept page.

> *[vIDEO](https://youtu.be/E12Xc3H2xqo)*

### First step: Write a command interpreter to manage your AirBnB objects.
> This is the first step towards building your first full web application: the AirBnB clone. This first step is very important because you will use what you build during this project with all other following projects: HTML/CSS templating, database storage, API, front-end integration…

> Each task is linked and will help you to:

- put in place a parent class (called `BaseModel`) to take care of the initialization, serialization and deserialization of your future instances
- create a simple flow of serialization/deserialization: Instance <-> Dictionary <-> JSON string <-> file
- create all classes used for AirBnB (`User`, `State`, `City`, `Place`…) that inherit from BaseModel
- create the first abstracted storage engine of the project: File storage.
- create all unittests to validate all our classes and storage engine

## What’s a command interpreter?
Do you remember the Shell? It’s exactly the same but limited to a specific use-case. In our case, we want to be able to manage the objects of our project:

- Create a new object (ex: a new User or a new Place)
- Retrieve an object from a file, a database etc…
- Do operations on objects (count, compute stats, etc…)
- Update attributes of an object
- Destroy an object

# Resources
*Read or watch:*

- [cmd module](https://alx-intranet.hbtn.io/rltoken/8ecCwE6veBmm3Nppw4hz5A)
- *packages* concept page
- [uuid module](https://alx-intranet.hbtn.io/rltoken/KfL9TqwdI69W6ttG6gTPPQ)
- [datetime](https://alx-intranet.hbtn.io/rltoken/1d8I3jSKgnYAtA1IZfEDpA)
- [unittest module](https://alx-intranet.hbtn.io/rltoken/IlFiMB8UmqBG2CxA0AD3jA)
- [args/kwargs](https://alx-intranet.hbtn.io/rltoken/C_a0EKbtvKdMcwIAuSIZng)
- [Python test cheatsheet](https://alx-intranet.hbtn.io/rltoken/tgNVrKKzlWgS4dfl3mQklw)


## User's steps:
### Interactive Mode
```python
> $ ./console.py
> (hbnb) help
> 
> Documented commands (type help <topic>):
> ========================================
> EOF  help  quit
> 
> (hbnb)
> (hbnb)
> (hbnb) quit
> $
```

### Non-Interactive Mode
```python
> $ echo "help" | ./console.py
> (hbnb)
> 
> Documented commands (type help <topic>):
> ========================================
> EOF  help  quit
> (hbnb)
> $
> $ cat test_help
> help
> $
> $ cat test_help | ./console.py
> (hbnb)
> 
> Documented commands (type help <topic>):
> ========================================
> EOF  help  quit
> (hbnb)
> $
```


## description of the command interpreter

| Description             | Command                                                                |
| ----------------- | ------------------------------------------------------------------ |
| Creates an instance of a class | `create <class>` |
| Retrieves all instances of a class | `<class>.all()` |
| Retrieves the number of instances of a class | `<class>.count()` |
| Retrieves an instance based on its id | `<class>.show(<id>)` |
| Prints the string representation of an instance of a class based on class name and id | `show <class> <id>` |
| Prints all string representations of all instances | `all` |
| Prints all string representations of all instances based on class name | `all <class>` |
| Updates an attribute of an instance based on class name and id | `update <class> <id> <attribute name> "<attribute value>"` |
| Destroys an instance based on its id | `<class>.destroy(<id>)` |
| Deletes instance of a class based on class name and id | `destroy <class> <id>` |
| 	Exits the program | `EOF` |
| 	Exits the program | `quit` |


> # *collaborator:*
> 1. [Ann Wahome](https://github.com/AnnWahome)
> 2. [John Muthabuku](https://github.com/John-thabuks)