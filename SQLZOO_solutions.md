# SQLZOO Solutions

Solutions for [SQLZOO Tutoral](http://sqlzoo.net/wiki/SQL_Tutorial).

## Sections:

1. [SELECT basics](#select-basics)
2. [SELECT from WORLD](#select-from-world)
3. [SELECT from NOBEL](#select-from-nobel)
4. [SELECT in SELECT](#select-in-select)
5. [SUM and COUNT](#sum-and-count)
6. [JOIN](#join)
7. [More JOIN](#more-join)
8. [Using NULL](#using-null)
9. [Self JOIN](#self-join)

## SELECT basics

Some simple queries to get you started

1.  The example uses a WHERE clause to show the population of 'France'. Note that strings should be in 'single quotes';

Modify it to show the population of Germany

```sql
  SELECT population FROM world
    WHERE name = 'Germany'
```

2.  Checking a list The word IN allows us to check if an item is in a list. The example shows the name and population for the countries 'Brazil', 'Russia', 'India' and 'China'.

Show the name and the population for 'Sweden', 'Norway' and 'Denmark'.

```sql
  SELECT name, population FROM world
    WHERE name IN ('Sweden', 'Norway', 'Denmark');
```

3.  Which countries are not too small and not too big? BETWEEN allows range checking (range specified is inclusive of boundary values). The example below shows countries with an area of 250,000-300,000 sq. km. Modify it to show the country and the area for countries with an area between 200,000 and 250,000.

```sql
  SELECT name, area FROM world
    WHERE area BETWEEN 200000 AND 250000
```
