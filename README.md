# SQL
Data Science Foundations Create a Table
CREATE TABLE friends (
  id INTEGER,
  name TEXT,
  birthday DATE
);

INSERT INTO friends (id, name, birthday)
VALUE (1, 'Ororo Munroe', '1940-05-30');

SELECT * FROM friends;

INSERT INTO friends(id, name, birthday)
VALUE (2, 'Laurence Miller', '1989-02-20');

INSERT INTO friends(id, name, birthday)
VALUE (3, 'Elisee Diakonidze', '2014-03-11');

UPDATE friends
SET name = 'Storm'
WHERE  id = 1;
ALTER TABLE friends
ADD email TEXT;
UPDATE friends
SET email = 'storm@codecademy.com'
WHERE id = 1;
UPDATE friends
SET email = 'Laurence@codecademy.com'
WHERE id = 2;
UPDATE friends
SET email = 'Elisee@codecademy.com'
WHERE id = 3;
DELETE FROM friends
WHERE id = 1;

SELECT * FROM friends;
