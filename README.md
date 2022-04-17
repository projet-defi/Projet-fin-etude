# Projet-fin-etude
Requete finale sculptures 100%

```json
SELECT ?CollectionLabel (COUNT(?item) AS ?count)
WHERE
{
 ?item wdt:P31/wdt:P279* wd:Q860861.
 ?item wdt:P195 ?Collection.
 ?Collection wdt:P17 wd:Q142.  
OPTIONAL {
 ?item wdt:P18 ?pic .
}
  SERVICE wikibase:label { 
bd:serviceParam wikibase:language "fr,en"}
    
}
GROUP BY ?CollectionLabel
ORDER BY DESC (?count)
```
********************
Requete finale sculptures 10%


```json
SELECT ?CollectionLabel (COUNT(?item) AS ?count)
WHERE
{
 ?item wdt:P31/wdt:P279* wd:Q860861.
 ?item wdt:P195 ?Collection.
 ?Collection wdt:P17 wd:Q142.  
OPTIONAL {
 ?item wdt:P18 ?pic .
}
  SERVICE wikibase:label { 
bd:serviceParam wikibase:language "fr,en"}
    
}
GROUP BY ?CollectionLabel
ORDER BY DESC (?count) 

LIMIT 20
```
********************
peiture 100%
```json
SELECT ?CollectionLabel (COUNT(?item) AS ?count)
WHERE
{
 ?item wdt:P31/wdt:P279* wd:Q3305213.
 ?item wdt:P195 ?Collection.
 ?Collection wdt:P17 wd:Q142.  
OPTIONAL {
 ?item wdt:P18 ?pic .
}
  SERVICE wikibase:label { 
bd:serviceParam wikibase:language "fr,en"}
    
}
GROUP BY ?CollectionLabel
ORDER BY DESC (?count) 
```
********************
 peinture 10%
```json
SELECT ?CollectionLabel (COUNT(?item) AS ?count)
WHERE
{
 ?item wdt:P31/wdt:P279* wd:Q3305213.
 ?item wdt:P195 ?Collection.
 ?Collection wdt:P17 wd:Q142.  
OPTIONAL {
 ?item wdt:P18 ?pic .
}
  SERVICE wikibase:label { 
bd:serviceParam wikibase:language "fr,en"}
    
}
GROUP BY ?CollectionLabel
ORDER BY DESC (?count) 
limit 20
```
