# carlist-database
A wikidata query to generate a list of vehicles.

#1 - Visit the URL
https://query.wikidata.org

Enter the query below

```
PREFIX wd: <http://www.wikidata.org/entity/>
PREFIX wdt: <http://www.wikidata.org/prop/direct/>
PREFIX wikibase: <http://wikiba.se/ontology#>
PREFIX p: <http://www.wikidata.org/prop/>
PREFIX v: <http://www.wikidata.org/prop/statement/>
PREFIX q: <http://www.wikidata.org/prop/qualifier/>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>

SELECT ?p ?pLabel
WHERE {
	?p wdt:P176 wd:Q9584 
       
  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en" .
  }      
}
```

#3 - Improvements
Over time this query will be expanded to all road vehicles and whatever properties are listed..etc..trim, model, transmission...etc
