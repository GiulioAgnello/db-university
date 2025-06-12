QUESITO 1

```sql
SELECT count(id), YEAR`enrolment_date` FROM `students`
GROUP BY YEAR(`enrolment_date`)

CORRETTO DOPO REVISIONE
```

QUESITO 2

```sql
SELECT count(`id`), `office_address`
FROM `university.teachers`
GROUP BY `office_address`

CORRETTO DOPO REVISIONE
```

QUESITO 3

```sql
SELECT AVG(`vote`), `exam_id`
FROM `university.exam_student`
GROUP BY `exam_id`

CORRETTO DOPO REVISIONE
```

QUESITO 4

```sql
SELECT COUNT(`id`), `department_id`
FROM `university.degrees`
GROUP BY `department_id`

CORRETTO DOPO REVISIONE
```
