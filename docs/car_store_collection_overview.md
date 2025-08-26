# Car_store - E2E stable (brand+car) - overview

- Source: `21563877-86fc0407-cd06-4575-a376-6cb822943746`
- Default baseUrl: `http://localhost:3001`

| Name                                    | Method   | Path                                                    |
|:----------------------------------------|:---------|:--------------------------------------------------------|
| 02 - CREATE brand (random)              | POST     | {{baseUrl}}/brands                                      |
| 03 - CREATE car (random, link to brand) | POST     | {{baseUrl}}/cars                                        |
| 04 - UPDATE car (PATCH)                 | PATCH    | {{baseUrl}}/cars/{{carId}}                              |
| 05 - GET car with relations             | GET      | {{baseUrl}}/cars/{{carId}}?_expand=brand&_embed=reviews |
| 06 - GET brand cars includes our car    | GET      | {{baseUrl}}/brands/{{brandId}}/cars                     |
| 07 - DELETE car (cleanup)               | DELETE   | {{baseUrl}}/cars/{{carId}}                              |
| 08 - DELETE brand (cleanup)             | DELETE   | {{baseUrl}}/brands/{{brandId}}                          |
