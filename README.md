# products

Dokumentation för produkt APIs.


## Api Endpoint för att lista alla produkter

[http://products.arcada.nitor.zone/api/list-products.php](http://products.arcada.nitor.zone/api/list-products.php)
```JSON
{  
   "status":200,
   "products":[  
      {  
         "id":0,
         "name":"Heineken",
         "price":"2",
         "description":"pale lager beer",
         "category":"lager",
         "picture":"url",
      },
      {  
         "id":1,
         "name":"Carlsberg",
         "price":"2",
         "description":"Probably the best beer in the world",
         "category":"pilsner",
         "picture":"url",
      }
   ]
}
```


## Api Endpoint för att lägga till en produkt

[http://products.arcada.nitor.zone/api/add-product.php](http://products.arcada.nitor.zone/api/add-product.php)
```JSON
{  
   "status":200,
   "products":[  
      {  
         "id":0,
         "name":"Heineken",
         "price":"2",
         "description":"pale lager beer",
         "category":"lager",
         "picture":"url",
      }
   ]
}
```


## Api Endpoint för att söka efter produkter

Behöver parametern "search" (search term). Söker igenom namn och description efter söktermen och listar ut resultaten. Ersätt space med "+".

[http://products.arcada.nitor.zone/api/search.php?search="lager+beer"](http://products.arcada.nitor.zone/api/search.php?search="lager-beer")
```JSON
{  
   "status":200,
   "products":[  
      {  
         "id":0,
         "name":"Heineken",
         "price":"2",
         "description":"pale lager beer",
         "category":"lager",
         "picture":"url",
      },
      {  
         "id":1,
         "name":"Carlsberg",
         "price":"2",
         "description":"Probably the best beer in the world",
         "category":"pilsner",
         "picture":"url",
      }
   ]
}
```
