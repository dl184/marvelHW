ANSWERS

<!-- 1. Return ALL the data in the 'movies' table. -->
SELECT * FROM movies;

<!-- 2. Return ONLY the name column from the 'people' table -->
SELECT * FROM people;

<!-- 3. Oh bother! Someone at CodeClan spelled Campbell's name wrong! Change it to reflect the proper spelling (change 'Cambel Millar' to 'Campbell Miller'). -->
UPDATE people SET name = 'Cambell Miller' WHERE name = 'Cambel Millar'; 

<!-- 4. Return ONLY your name from the 'people' table. -->
SELECT name FROM people WHERE name = 'Derek Leach';

<!-- 5. The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table. -->
DELETE FROM movies WHERE title = 'Batman Begins';

<!-- 6. Create a new entry in the 'people' table with the name of one of the instructors. -->
INSERT INTO people (name) VALUES ('COLIN');


<!-- 7. Oh no! Nefarious G5 instructor Alan Russell has decided to hijack our movie evening! Remove him from the table of people. -->
DELETE FROM people WHERE name = 'Alan Russell';


<!-- 8. The cinema has just heard that they will be holding an exclusive midnight showing of 'Avengers: Infinity War'!! Create a new entry in the 'movies' table to reflect this. -->
INSERT INTO movies (title, year, show_time) VALUES ('Avengers: Infinity War', 2018, '12:00');
<!-- 9. The cinema would also like to make the Guardian movies a back-to-back feature. Update the 'Guardians of the Galaxy' show time from 16:50 to 20:00 -->
UPDATE movies SET show_time = '16:50 to 20:00' WHERE show_time = '16:50';



## Extension

<!-- 1. Research how to delete multiple entries from your table in a single command. -->

DELETE FROM movies WHERE id between 1 and 3;
