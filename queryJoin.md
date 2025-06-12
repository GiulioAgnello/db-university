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
SELECT *
FROM `departments`
JOIN `degrees`
ON `departments`.`id` = `department_id`
WHERE `departments`.`name` = "dipartimento di neuroscienze"
AND `degrees`.`level` = "magistrale"
```

QUESITO 3

```sql
SELECT
`course_teacher`.`course_id`,
 `course_teacher`.`teacher_id`
FROM `exams`
JOIN `courses`
ON `course_id` = `courses`.`id`
JOIN `course_teacher`
ON `courses`.`id` = `teacher_id`
WHERE `teacher_id` = 44
```

QUESITO 4

```sql
SELECT
`students`.`id`,
`students`.`name`,
`students`.`surname`,
`degrees`.*,
`departments`.`name`
FROM `students`
JOIN `degrees`
ON `degree_id` = `degrees`.`id`
JOIN `departments`
ON `department_id` = `departments`.`id`
ORDER BY `surname` ASC, `students`.`name` ASC
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
