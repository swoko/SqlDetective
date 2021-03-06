The SQL Detective Game

Learn the basics of Relational database management by playing the Detective Game. Uncover how database technology can be applied to business situations to help you manage your company information.

# IBM

IBM has a nice game to let people get familiar with sql.
The game teaches relational database concepts and shows how technology can be applied to solving real-life problems.

# Non IBM
This is available for DB2 and informix, I wanted to play it on a postgresql db. As it turned out ok, I wanted to make it easy for others as well. So I added the mysql dialect as well.

# See also

http://www.ibm.com/developerworks/data/tutorials/dm0804moffatt/

# Game scenario

You are an intern working in a security department for a large enterprise. As part of your training, you have been asked to participate in a crime investigation simulation to help locate a missing *thinkpad* laptop.


# Data model

The of the Detective Game database consists of four tables: employee, hardware, lobby, and security. It also shows you the type of information stored in each of these tables:

* The *employee* table stores information about each employee such as their employee number, name, manager, office number, phone number, and badge number.
* The *security* table stores information as to when each employee or visitor badged in and out of the building (date and time).
* The *lobby* table stores the badge number assigned to each visitor by name.
* The *hardware* table stores the serial number and type number for every computer along with its location and the ID of the employee who is its primary user.

```
                                               +------------------+  +-----------------+
                                               | Employee         |  | Hardware        |
                                               |------------------|  |-----------------|
                                               | Employee_ID      |  | Employee_ID     |
                                               | Last_name        |  | Location        |
                           +----------------+  | First_name       |  | Type_number     |
                           | Security       |  | Manager_ID       |  | Serial_number   |
                           |----------------|  | Location         |  +-----------------+
   +------------------+    | Sign_out_date  |  | Extension        |
   | Lobby            |    | Sign_out_time  |  | Gender           |
   |------------------|    | Sign_in_time   |  | Hair_colour      |
   | Badge_number     |    | Badge_number   |  | Badge number     |
   | Last_name        |    +----------------+  | Restricted_access|
   | First_name       |                        +------------------+
   +------------------+
```


# Legal blabla

I am no lawyer, nor do I intend to do something wrong. I just want to solve this puzzle without installing Informix.
I attached the IBM download agreement in the COPYING file. I guess this is a derrived work.
