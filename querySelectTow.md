QUESITO 1

```sql
SELECT count(id) FROM university.students
WHERE year(`enrolment_date`) = "2019"

SELECT count(id) FROM university.students
WHERE year(`enrolment_date`) = "2020"
```

QUESITO 2

```sql
SELECT count(*) FROM university.teachers
WHERE `office_address` LIKE "Borgo Elga%"
```

QUESITO 3

```sql
SELECT AVG(vote) FROM university.exam_student
WHERE `exam_id` = 1
```

QUESITO 4

```sql
SELECT COUNT(*) FROM university.degrees
WHERE `name` LIKE "%biologia%"
```
