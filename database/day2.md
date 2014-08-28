
-column order is always fixed
Rows are not stored in any order

Example of Creating Table-------------
CREATE TABLE pilot (
	fname	varchar(15), //upto 15 not always allocating 15
	lname	varchar(15),
	license_num 	integer,  -- Pilot license ID
	birthdate	date
);

DataTypes---------------
smallint, real, percision, date, time, timestamp, interval

\d <name of database> //shows the list of relations

Example of Inserting information
INSERT INTO pilot
  VALUES ('Charles', "Lindberg', 69, '2/4/1902');
 
 DROP TABLE  //deletes the entire table

Creating Table Constraints---------------

CREATE TABLE pilot (
	fname	varchar(15), 
	lname	varchar(15) NOT NULL,
	license_num 	serial PRIMARY KEY, //serial means it auto increments so no worries
	birthdate	date NOT NULL
); 

Owner_license_num	integer reference pilot(license_num), //means its a forign key from the feild 
num_engines			samllint CHECK(num_engines > 0)

INSERT INTO pilot
  VALUES ('Charles', "Lindberg', DEFAULT, '2/4/1902'); //the default will allow for it to auto-increment 

INSERT INTO pilot (fname, lname, birthdate)
  VAULES(etc..) //forgin keys must exist to be used