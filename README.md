# Sql-second-task
/*In this we are going to insert values in already created table which we created in task 1 and update by using where condition*/ 

INSERT INTO students (id, name, age) VALUES (1, 'Kaif', 22);
INSERT INTO students (id, name, age) VALUES (2, 'Ravi', 21);
INSERT INTO students (id, name, age) VALUES (3, 'Aman', NULL); -- age missing
INSERT INTO students (id, name) VALUES (4, 'Sana'); -- uses default age 18


INSERT INTO Book (b_id, name, s_id) VALUES (101, 'C Programming', 1);
INSERT INTO Book (b_id, name, s_id) VALUES (102, 'DBMS', 2);
INSERT INTO Book (b_id, name, s_id) VALUES (103, 'Networking', NULL); -- unassigned book


UPDATE students SET age = 23 WHERE id = 1;
UPDATE Book SET s_id = 3 WHERE b_id = 103;


DELETE FROM students WHERE id = 4; -- only if no book assigned
DELETE FROM Book WHERE b_id = 102;
