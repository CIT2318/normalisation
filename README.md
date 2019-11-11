| id | name          | first_appearance | power1       | power2              | power3              |
|----|---------------|------------------|--------------|---------------------|---------------------|
| 1  | Black Panther | 1966             | Night Vision | Superhuman Strength | null                |
| 2  | Spiderman     | 1962             | Wallcrawling | Heightened Senses   | Superhuman Strength |
| 3  | Storm         | 1975             | Flight       | Control of Elements | null                |

| id | name          | first_appearance |
|----|---------------|------------------|
| 1  | Black Panther | 1966             |
| 2  | Spiderman     | 1962             |
| 3  | Storm         | 1975             |

| id | name                |
|----|---------------------|
| 1  | Night Vision        |
| 2  | Wallcrawling        |
| 3  | Flight              |
| 4  | Control of Elements |
| 5  | Superhuman Strength |
| 6  | Heightened Senses   |

| character_id | power_id |
|--------------|----------|
| 1            | 1        |
| 1            | 5        |
| 2            | 2        |
| 2            | 6        |
| 2            | 5        |
| 3            | 3        |
| 3            | 4        |

Need another 1st normal form example comma separated values e.g. film and locations
| id | title              | year | starring                                        |
|----|--------------------|------|-------------------------------------------------|
| 1  | Jaws               | 1975 | Roy Scheider, Robert Shaw, Richard Dreyfuss     |
| 2  | Winter's Bone      | 2010 | Jennifer Lawrence, John Hawkes |
| 3  | Do The Right Thing | 1989 | Danny Aiello, Ossie Davis             |

| id | title              | year |
|----|--------------------|------|
| 1  | Jaws               | 1975 |
| 2  | Winter's Bone      | 2010 |
| 3  | Do The Right Thing | 1989 |

| id | last_name | first_name |
|----|-----------|------------|
| 1  | Scheider  | Roy        |
| 2  | Shaw      | Robert     |
| 3  | Dreyfuss  | Richard    |
| 4  | Hawkes    | John       |
| 5  | Aiello    | Danny      |
| 6  | Davis     | Ossie      |
| 7  | Lawrence  | Jennifer   |

| film_id | actor_id |
|---------|----------|
| 1       | 1        |
| 1       | 2        |
| 1       | 3        |
| 2       | 4        |
| 3       | 5        |
| 3       | 6        |
| 2       | 7        |

2nd normal form
recipe ingredients
student module marks

3rd normal form example
| id | title              | year | director_id | director_lastname | director_firstname |
|----|--------------------|------|-------------|-------------------|--------------------|
| 1  | Jaws               | 1975 | 7           | Spielberg         | Steven             |
| 2  | Winter's Bone      | 2010 | 45          | Granik            | Debra              |
| 3  | Do The Right Thing | 1989 | 3           | Lee               | Spike              |

| id | title              | year | director_id |
|----|--------------------|------|-------------|
| 1  | Jaws               | 1975 | 7           |
| 2  | Winter's Bone      | 2010 | 45          |
| 3  | Do The Right Thing | 1989 | 3           |

| id | director_lastname | director_firstname |
|----|-------------------|--------------------|
| 1  | Spielberg         | Steven             |
| 2  | Granik            | Debra              |
| 3  | Lee               | Spike              |



| id | dr_id | patient_id | dr_name     | patient_name  | date_time        | room |
|----|-------|------------|-------------|---------------|------------------|------|
| 1  | 1     | 1          | Jakub Nowak | Kate Atherton | 01/01/2021 10:00 | s13  |
| 2  | 1     | 2          | Sadia Afzal | Sunil Laxman  | 01/01/2021 10:15 | s5   |
| 3  | 2     | 3          | Jakub Nowak | Kate Hutton   | 12/03/2021 15:30 | s13  |
| 4  | 2     | 2          | Jakub Nowak | Sunil Laxman  | 04/04/2021 12:15 | s7   |

1st normal form
| id | dr_id | patient_id | dr_last_name | dr_first_name | patient_last_name | patient_first_name | date_time   | time  | room |
|----|-------|------------|--------------|---------------|-------------------|--------------------|-------------|-------|------|
| 1  | 1     | 1          | Nowak        | Jakub         |  Atherton         | Kate               | 01/01/2021  | 10:00 | s13  |
| 2  | 1     | 2          | Afzal        | Sadia         | Laxman            | Sunil              | 01/01/2021  | 10:15 | s5   |
| 3  | 2     | 3          | Nowak        | Jakub         | Hutton            | Kate               | 12/03/2021  | 15:30 | s13  |
| 4  | 2     | 2          | Nowak        | Jakub         | Laxman            | Sunil              | 04/04/2021  | 12:15 | s7   |

2nd normal form
| id | dr_id | patient_id | date        | time  | room |
|----|-------|------------|-------------|-------|------|
| 1  | 1     | 1          | 01/01/2021  | 10:00 | s13  |
| 2  | 1     | 2          | 01/01/2021  | 10:15 | s5   |
| 3  | 2     | 3          | 12/03/2021  | 15:30 | s13  |
| 4  | 2     | 2          | 04/04/2021  | 12:15 | s7   |

| id | last_name | first_name |
|----|-----------|------------|
| 1  | Nowak     | Jakub      |
| 1  | Afzal     | Sadia      |

| id | last_name | first_name |
|----|-----------|------------|
| 1  | Atherton  | Kate       |
| 2  | Laxman    | Sunil      |
| 3  | Hutton    | Kate       |
