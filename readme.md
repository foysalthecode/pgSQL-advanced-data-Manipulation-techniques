# ALTER

    Rename table

    Add/Drop column

    Rename column

    Modify data type

    Setting Deafault Value

    Add/Drop Constraint

# SELECT

> The SELECT statement is used to retrieve data from one or more tables and can be customized with conditions, sorting, and other clauses.

    GROUP
    JOIN
    SELECT
    ORDER
    FROM
    OFFSET
    HAVING
    DISTINCT
    WHERE
    LIMIT

## using select

    1 select first_name from students
    2 select first_name,age from students
    3 select * from students

## column alias

> select first_name as "First Name" from students;

## sorting

> select first_name,blood_group,country,age from students order by age desc

## Distinct (find the unique value or keyword)

> select distinct course from students

## Filtering --> Operator and select students from the thailand

> select * from students where country = 'thailand'

## select students with 'A' grade in physics

> select * from students where grade = 'A'

## select student from nepal or from bangladesh

> select * from students where country = "nepal" or country = "Bangladesh"

## select students with grade "A" or "B" in mathematics or physics

> select * from students where (grade = "A" or grade = "B") and (course = "mathematics" or course = "physics")

# AND Operator

<!-- select students from nepal where the age is 20 -->

> select * from students where country = "Nepal" and age = 20

## select students from the nepal or from Bangladesh and the age is 20

> select * from students where (country = "Nepal" or country = "Bangladesh") and age = 20

## comparison operator

<!-- select students older than 20 -->

> select _ from students where age > 20
> select _ from students where age < 20

## serve all data except nepal

> select * from students where country != "Nepal"
<!-- we can use <> this instead of != -->
> select * from students where country <> "Nepal"

## select student whose age is between 20 and 22  
> select * from student where age between 20 and 22 

> select distinct age from students

## select students from bangladesh,india, or nepal

<!-- > select * from students where country = "Bangladesh" or country = "India" or country = "Nepal" -->

> select * from students in (bangladesh,india,nepal) 



