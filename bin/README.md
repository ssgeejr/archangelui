# archangelui
ArchAngel UI [broken out for module building]

Test notes:

### Running the test outside of a container
```
[devops@cicd ~]$ curl --header "Content-Type: application/json" --request POST --data '{"car_model":"Compass"}' http://localhost:8880/archangel/query
{ "_id" : { "$oid" : "5b88933b087cf319fe2ee763" }, "id" : 10, "first_name" : "Mercie", "last_name" : "Schumacher", "car_model" : "Compass", "car_year" : 2011, "city" : "Wangq" }
```


### Running the test inside of a container
```
[devops@cicd ~]$ curl --header "Content-Type: application/json" --request POST --data '{"car_model":"Compass"}' http://archangelms:8080/archangel/query
{ "_id" : { "$oid" : "5b88933b087cf319fe2ee763" }, "id" : 10, "first_name" : "Mercie", "last_name" : "Schumacher", "car_model" : "Compass", "car_year" : 2011, "city" : "Wangq" }
```


