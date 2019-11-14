# Normalisation
Look at the following database tables and normalise them. For each table idenitfy which *normal forms* you are applying. Don't draw out the database tables or construct class diagrams, simply provide your answer in the form of a simple database schema e.g. for a films table example:
```
 films={id(PK),title,year duration,certificate_id(FK)}
```

## Question 1
**Superheros**
| id | name          | first_appearance | power1       | power2              | power3              |
|----|---------------|------------------|--------------|---------------------|---------------------|
| 1  | Black Panther | 1966             | Night Vision | Superhuman Strength | null                |
| 2  | Spiderman     | 1962             | Wallcrawling | Heightened Senses   | Superhuman Strength |
| 3  | Storm         | 1975             | Flight       | Control of Elements | null                |

## Question 2
**Films**
| id | title              | year | starring                                        |
|----|--------------------|------|-------------------------------------------------|
| 1  | Jaws               | 1975 | Roy Scheider, Robert Shaw, Richard Dreyfuss     |
| 2  | Winter's Bone      | 2010 | Jennifer Lawrence, John Hawkes |
| 3  | Do The Right Thing | 1989 | Danny Aiello, Ossie Davis             |

## Question 3
| id | title              | year | director_id | director_lastname | director_firstname |
|----|--------------------|------|-------------|-------------------|--------------------|
| 1  | Jaws               | 1975 | 7           | Spielberg         | Steven             |
| 2  | Winter's Bone      | 2010 | 45          | Granik            | Debra              |
| 3  | Do The Right Thing | 1989 | 3           | Lee               | Spike              |


## Question 4
| recipe_id | ingredient_id | quantity | ingredient_name |
|-----------|---------------|----------|-----------------|
| 1         | 1             | 2        | egg             |
| 1         | 2             | 125g     | butter          |
| 1         | 3             | 125g     | flour           |
| 2         | 1             | 3        | egg             |
| 2         | 2             | 1tsp     | butter          |

## Question 5
| id | dr_id | patient_id | dr_name     | patient_name  | date_time        | room |
|----|-------|------------|-------------|---------------|------------------|------|
| 1  | 1     | 1          | Jakub Nowak | Kate Atherton | 01/01/2021 10:00 | s13  |
| 2  | 1     | 2          | Sadia Afzal | Sunil Laxman  | 01/01/2021 10:15 | s5   |
| 3  | 2     | 3          | Jakub Nowak | Kate Hutton   | 12/03/2021 15:30 | s13  |
| 4  | 2     | 2          | Jakub Nowak | Sunil Laxman  | 04/04/2021 12:15 | s7   |
