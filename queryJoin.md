QUESITO 1

```sql
SELECT
`students`.*
FROM `students`
JOIN `degrees`
ON `degree_id` = `degrees`.`id`
WHERE `degrees`.`name` = "corso di laurea in economia"
```

QUESITO 2

```sql
SELECT * FROM university.courses
WHERE cfu > "10"
```

QUESITO 3

```sql
SELECT *
FROM university.students
WHERE
YEAR(`date_of_birth`) < "1995"
```

QUESITO 4

```sql
SELECT * FROM university.courses
WHERE period = "I semestre"
AND `year` = "1"
```

QUESITO 5

```sql
SELECT * FROM university.exams
WHERE
`date` = "2020-06-20"
AND
`hour` > "14:00:00"

```

QUESITO 6

```sql
SELECT * FROM university.degrees
WHERE `level` = "magistrale"
```

QUESITO 7

```sql
SELECT count(id) FROM university.departments;
```

QUESITO 8

```sql
SELECT COUNT(*) FROM university.teachers
WHERE `phone` IS NULL
```
