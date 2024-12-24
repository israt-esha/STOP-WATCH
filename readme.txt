https://israt-esha.github.io/STOP-WATCH/
This is a stop watch app. The SQL command for this app are following below



1. Create a Database
CREATE DATABASE StopwatchApp;


2. Create a Table for Recorded Times
USE StopwatchApp;

CREATE TABLE Records (
    id INT AUTO_INCREMENT PRIMARY KEY,
    user_name VARCHAR(100) NOT NULL,
    recorded_time TIME NOT NULL,
    recorded_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);


3. Insert Recorded Times
INSERT INTO Records (user_name, recorded_time)
VALUES ('John Doe', '00:05:30');


4. Fetch Recorded Times
Retrieve all stopwatch records:

SELECT * FROM Records;


5. Delete a Record (if necessary)
DELETE FROM Records
WHERE id = 1;
