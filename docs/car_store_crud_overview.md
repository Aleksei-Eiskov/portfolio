# Car_store - CRUD collection - overview

- Source: `21563877-9eef265e-807b-4478-ab4f-939873db0428`
- Variables:
  - `baseUrl` = `http://localhost:3001`
  - `carId` = `1`
  - `brandId` = `4`

| Group               | Name                           | Method   | Path                                                                 |
|:--------------------|:-------------------------------|:---------|:---------------------------------------------------------------------|
| Health & Admin      | GET - /health                  | GET      | {{baseUrl}}/health                                                   |
| Health & Admin      | POST - /reset                  | POST     | {{baseUrl}}/reset                                                    |
| Cars                | GET - /cars (list)             | GET      | {{baseUrl}}/cars                                                     |
| Cars                | GET - /cars (filters)          | GET      | {{baseUrl}}/cars?brandId={{brandId}}&price_gte=20000&price_lte=40000 |
| Cars                | POST - /cars (create)          | POST     | {{baseUrl}}/cars                                                     |
| Cars                | GET - /cars/:id                | GET      | {{baseUrl}}/cars/{{carId}}                                           |
| Cars                | GET - /cars/:id with relations | GET      | {{baseUrl}}/cars/{{carId}}?_expand=brand&_embed=reviews              |
| Cars                | PATCH - /cars/:id (price)      | PATCH    | {{baseUrl}}/cars/{{carId}}                                           |
| Cars                | PUT - /cars/:id (replace)      | PUT      | {{baseUrl}}/cars/{{carId}}                                           |
| Cars                | DELETE - /cars/:id             | DELETE   | {{baseUrl}}/cars/5                                                   |
| Brands              | GET - /brands                  | GET      | {{baseUrl}}/brands                                                   |
| Brands              | GET - /brands/:id              | GET      | {{baseUrl}}/brands/?id=5                                             |
| Brands              | GET - /brands/:id/cars         | GET      | {{baseUrl}}/brands/{{brandId}}/cars                                  |
| Brands              | PATCH - /brands/:id (update)   | PATCH    | {{baseUrl}}/brands/{{brandId}}                                       |
| Brands              | PUT - /brands/:id (replace)    | PUT      | {{baseUrl}}/brands/{{brandId}}                                       |
| Brands              | POST - /brands (create)        | POST     | {{baseUrl}}/brands                                                   |
| Brands              | DELETE - /brand/:Id            | DELETE   | {{baseUrl}}/brands/7                                                 |
| Reviews             | GET - /cars/:id/reviews        | GET      | {{baseUrl}}/cars/{{carId}}/reviews                                   |
| Search & Pagination | GET - /cars search             | GET      | {{baseUrl}}/cars?q=tesla                                             |
| Search & Pagination | GET - /cars sort & page        | GET      | {{baseUrl}}/cars?_sort=price&_order=asc&_page=1&_limit=3             |
