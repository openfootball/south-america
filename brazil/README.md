# Brazil


## Build Your Own `brazil.db` Copy


Try in your working folder (that is, `/brazil`):

```
$ sportdb build
$ sportdb --verbose build     # or for more (verbose) details incl. debug info
```

This will

- setup a new single-file SQLite database e.g. `./sport.db`
- read in all datasets in plain text (`.txt`)

That's it. Try:

```
$ sqlite3 sport.db

SQLite version 3.7.16
Enter ".help" for instructions
Enter SQL statements terminated with a ";"

sqlite> .tables

alltime_standing_entries  events_grounds            names
alltime_standings         events_teams              parts
assocs                    games                     persons
assocs_assocs             goals                     places
badges                    grounds                   props
cities                    group_standing_entries    rosters
continents                group_standings           rounds
counties                  groups                    seasons
countries                 groups_teams              states
country_codes             langs                     taggings
districts                 leagues                   tags
event_standing_entries    logs                      teams
event_standings           metros                    usages
events                    munis                     zones

sqlite> select * from countries;

1|Brazil|brazil|br|1|BRA|||192380000|8514215|||f|t|f|f|

sqlite> select * from teams;

1|corinthians|Corinthians|COR|SC Corinthians Paulista|Corinthians São Paulo|||t|||||f|
2|saopaulo|São Paulo|SAO|São Paulo FC|FC São Paulo|1||t|||||f|
3|santossp|Santos|SAN|Santos SP|Santos FC|FC Santos|Santos Futebol Clube|1||t|||||f|
4|palmeiras|Palmeiras|PAL|Palmeiras SP|SE Palmeiras|1||t|||||f|
5|pontepreta|Ponte Preta|PON|AA Ponte Preta|Associação Atlética Ponte Preta|1||t|||||f|
6|botafogo|Botafogo|BOT|Botafogo RJ|Botafogo FR|Botafogo de Futebol e Regatas|1||t|||||f|
7|flamengo|Flamengo|FLA|CR Flamengo|Flamengo RJ|Flamengo Rio de Janeiro|1||t|||||f|
8|fluminense|Fluminense|FLU|Fluminense FC|Fluminense RJ|Fluminense Rio de Janeiro|1||t|||||f|
9|atleticomg|Atlético Mineiro|CAM|C Atlético Mineiro|Atlético MG|1||t|||||f|
10|cruzeiro|Cruzeiro|CRU|Cruzeiro EC|Cruzeiro MG|Cruzeiro Esporte Clube|1||t|||||f|
11|americamg|América Mineiro|AMG|América MG|América FC|América Futebol Clube|1||t|||||f|
12|gremio|Grêmio|GRE|Grêmio RS|Grêmio Porto Alegre|Grêmio FBPA|1||t|||||f|
...

```

And so on.



## Questions? Comments?

Send them along to the
[Open Sports & Friends Forum/Mailing List](http://groups.google.com/group/opensport).
Thanks!
