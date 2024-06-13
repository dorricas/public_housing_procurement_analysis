# SISE2601 Project data description
================
Team 4

Elect results:
Rows: 12,545
Columns: 51

information about the last elections results in every ballot box in the country.  

- ballot id – id of each ballot box. an integer number.
- Committee symbol – the ballot's geographical areas. Each area gets a number in range 1 to 20,
  ballot boxes inside IDF bases get 99.
- settlement name – the settlement of the ballot box.
- settlement ID – settlement's id of each ballot box.
- Ballot num – a float number that identifies the ballot box in its settlement. It can repeat
  itself in different settlements.
- BZB – number of eligible voters registered to the ballot box.
- Voters – number of votes in the ballot box.
- Rejected – number of uncounted votes in the ballot box.
- Accepted – number of counted votes in the ballot box.
- The rest of the variables are all the parties and how many votes each party got.


Properties by rooms:
Rows: 843
Columns: 14

Each record represents a settlement, a floor number, and the number of public housing properties
 in the country which are from that settlement and on that floor number.  

- CityLMSName – string of the settlement's name.
- Floor – floor number. Integer.
- OneRooms – number of one room apartments that exist in the settlement and on the floor number.
- TwoRooms – number of two rooms apartments that exists in the settlement and on the floor number.
  And it continues this way until TenRooms, and MoreRooms (more than 10) variables.


Property purchases:
Rows: 208
Columns: 7

Information about public housing property purchasing per settlement & year.  

- Lamas code – identification number of a settlement.
- Year – 2017 – 2024.
- Lamas name – the settlement's name.
- 3 rooms apartments – number of purchased 3 rooms apartments.
- 4+ rooms apartments – number of purchased 4 or more rooms apartments.
- average price (NIS) 3 rooms apartments – the average purchase price of 3 rooms apartment.
- average price (NIS) 4+ rooms apartments – the average purchase price of 4 or more rooms apartment.


Vacant apartments:
Rows: 277
Columns: 14

List of public housing apartments that have been available for more than 3 months.  

- CityLmsName – settlement's name.
- CityLmsCode – settlement id, number.
- NumOfRooms – number of rooms in the apartment (a float number because there're apartments
  with half-rooms).
- Floor – apartment's floor number.
- TotalArea – area of the apartment in square meter.
- CompanyName – the company that owns the apartment.
- StatusChangeDate – date the apartment has been available from.
