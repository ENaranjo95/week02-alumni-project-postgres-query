# 🔢 Week02 Alumni Project: PostgreSQL Query

### Goal: Build a Simple DB and submit a photo of the results of a complicated query

### What it should look like:

At least 20 students in your database. The query should return all students who graduated, live in Boston, and are under 30 in ascending order based on id.

| id    | first_name     | last_name   | cohort | grad status | age | city | state | neighborhood |
| ---------|:-------------:|:-------------:|:------:|:------:|:------:|:------:|:------:| ------:|
|   05  | Sarah | Sanders | 2017a | graduated | 22 | Boston | MA | JP |
|   11  | Jamal | Wehadababyitsaboy | 2017b | graduated | 23 | Boston | MA | Roxbury |
|   13  | Queen | Elizabeth | 2018a | graduated | 29 | Boston | MA | Dorchester |
|   17  | Bob | Rainbow | 2018b | graduated | 27 | Boston | MA | Dorchester |

```
Command to create table:

CREATE TABLE alumni(
  id INTEGER,
  first_name VARCHAR(30),
  last_name VARCHAR(30),
  cohort VARCHAR(5),
  grad_status TEXT,
  age INTEGER,
  city TEXT,
  state VARCHAR(2),
  neighborhood TEXT
)
```

```
Command to insert values:

INSERT INTO alumni(
  id,
  first_name,
  last_name,
  cohort,
  grad_status,
  age,
  city,
  state,
  neighborhood
)

VALUES(
 /* Enter data here */
)

```

```
Command to build table:

SELECT *
FROM alumni
WHERE grad_status = 'graduated'
AND city = 'Boston'
AND age < 30
ORDER BY id;

```


![alt text](img/alumniSQL.png)

```
I completed the challenge: 5
I feel good about my code: 4
I'm not sure if I am running to many conditionals and if the order of the conditinals matter. Also included on my README is the commands to build my table, insert values in my table, and how I built my table.
```
