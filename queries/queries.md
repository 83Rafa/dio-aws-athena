
### Queries 


- Query soma de casos por continente

```
SELECT continent, SUM(new_cases) 
FROM "covid-db"."world_covid_data" 
GROUP BY continent;
```
- Query total de mortes por continente

```
SELECT continent, SUM(new_deaths) 
from "covid-db"."world_covid_data" 
group by continent;
```
- Query total de vacinas aplicadas 

```
SELECT continent, SUM(people_vaccinated) 
FROM "covid-db"."world_covid_data"
GROUP BY continent;
```
- Query média de mortes entre homens fumantes

```
SELECT AVG(new_deaths)
FROM "covid-db"."world_covid_data"
GROUP BY "male_smokers";
```
