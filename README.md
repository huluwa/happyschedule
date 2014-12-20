<a href="https://travis-ci.org/snooplsm/happyschedule"><img width="90" height="20" src="https://travis-ci.org/snooplsm/happyschedule.svg"></a>

HappySchedule is a full fledged app for Transit.  Currently the transit agencies supported are NJ Transit, Long Island Rail Road, Metro North, and Septa.

The main components of the app are

1.  Generation of schedule as an sqlite database.
2.  Library containing core functionality of the android application
3.  Individual applications for NJ Rails, NJ Transit, LIRR, Metro North, SEPTA

Software Required
-----------------

-  python and any libraries accompanied by networkx
-  java, android sdk


Generating a schedule
---------------------

navigate to the trainapp folder

type <code>python graph_builder.py njtransit ${absolute.path.to.create.database.zip}</code> 

this will create a file in the proposed location (should put it in flavor/res/raw/database_db.zip 

again you could also do this for lirr, metro-north, septa.  Each agency is the folder name found in gtfs and overrides where you can put your gtfs data and custom overriding code respectively.
