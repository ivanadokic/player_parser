# README
* Ruby version '2.6.1'

# WHAT IT DOES:
This is a Ruby program that makes a single set of players records by parsing data from 3 different record files and then display these records sorted in 3 different ways. A player record consists of a last name, first name, gender, data of birth, and favorite color. A record consists of the following 5 fields: last name, first name, gender, date of birth and favorite color. 

### GOAL:
Using Ruby language, parse the following set of 3 input files

file1:
Kournikova Anna F F 6-3-1975 Red
Hingis Martina M F 4-2-1979 Green
Seles Monica H F 12-2-1973 Black

file2:
Smith | Steve | D | M | Red | 3-3-1985
Bonk | Radek | S | M | Green | 6-3-1975
Bouillon | Francis | G | M | Blue | 6-3-1975

file3:
Abercrombie, Neil, Male, Tan, 2/13/1943
Bishop, Timothy, Male, Yellow, 4/23/1967
Kelly, Sue, Female, Pink, 7/12/1959

and produce the following output:

Output 1:
Hingis Martina Female 4/2/1979 Green
Kelly Sue Female 7/12/1959 Pink
Kournikova Anna Female 6/3/1975 Red
Seles Monica Female 12/2/1973 Black
Abercrombie Neil Male 2/13/1943 Tan
Bishop Timothy Male 4/23/1967 Yellow
Bonk Radek Male 6/3/1975 Green
Bouillon Francis Male 6/3/1975 Blue
Smith Steve Male 3/3/1985 Red

Output 2:
Abercrombie Neil Male 2/13/1943 Tan
Kelly Sue Female 7/12/1959 Pink
Bishop Timothy Male 4/23/1967 Yellow
Seles Monica Female 12/2/1973 Black
Bonk Radek Male 6/3/1975 Green
Bouillon Francis Male 6/3/1975 Blue
Kournikova Anna Female 6/3/1975 Red
Hingis Martina Female 4/2/1979 Green
Smith Steve Male 3/3/1985 Red

Output 3:
Smith Steve Male 3/3/1985 Red
Seles Monica Female 12/2/1973 Black
Kournikova Anna Female 6/3/1975 Red
Kelly Sue Female 7/12/1959 Pink
Hingis Martina Female 4/2/1979 Green
Bouillon Francis Male 6/3/1975 Blue
Bonk Radek Male 6/3/1975 Green
Bishop Timothy Male 4/23/1967 Yellow
Abercrombie Neil Male 2/13/1943 Tan


## INPUT FILE INFORMATION
======================
Each file contains one person’s information per line.
The properties of a person are delimited by the following:

space (” “)
comma (“,”)
pipe (“|”)
You may assume that there are no delimiters in any of the properties themselves. Some properties (e.g. gender) are represented differently, depending on the delimiter.
Dates are represented in American format (month, day, year).

The order of properties is different for each format. The pipe-delimited file lists each record as follows:
LastName | FirstName | MiddleInitial | Gender | FavoriteColor | DateOfBirth

The comma-delimited file looks like this:
LastName, FirstName, Gender, FavoriteColor, DateOfBirth

The space-delimited file looks like this:
LastName FirstName MiddleInitial Gender DateOfBirth FavoriteColor

OUTPUT INFORMATION AND DISPLAY REQUIREMENTS
===========================================
Create and display 3 different views of the recordset.

Output 1 – sorted by gender (females before males) then by last name ascending
Output 2 – sorted by birth date, ascending then by last name ascending
Output 3 – sorted by last name, descending

Ensure that fields are displayed in the following order: last name, first name, gender, date of birth, favorite color.
Display dates in the format M/D/YYYY.

# HOW TO RUN IT:
1. cd into player_parser
2. Install the Ruby dependencies `bundle install`
3. Type 'rake display_records' in terminal to see players output
4. Type 'rake test' in terminal to view all tests
