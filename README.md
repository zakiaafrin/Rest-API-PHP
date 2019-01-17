# Rest-API-PHP
Try in git bash:
==================

1.Obtain all data:
curl -i -X GET http://localhost/my-rest-api/api/robots

2.Search a data by its name:
curl -i -X GET http://localhost/my-rest-api/api/robots/search/Astro

3.Search a data by its id:
curl -i -X GET http://localhost/my-rest-api/api/robots/3

4.Insert a new data:
curl -i -X POST -d '{"name":"C-3PO","type":"Droid","year":1977}' http://localhost/my-rest-api/api/robots

5.Try to insert a new data with the name of an existing robot:
curl -i -X POST -d '{"name":"C-3PO","type":"Droid","year":1977}' http://localhost/my-rest-api/api/robots

6.Update a datat with an unknown type:
curl -i -X PUT -d '{"name":"ASIMO","type":"humanoid","year":2000}'

7.delete a data:
curl -i -X DELETE http://localhost/my-rest-api/api/robots/1