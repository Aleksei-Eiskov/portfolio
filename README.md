# QA Portfolio - Car_store API, Postman collections and QA artifacts

**This repo contains:**
- Postman collections with standard CRUD requests and an end-to-end scenario
- public HTML and Markdown pages to preview collections without downloading JSON
- sample QA PDFs: bug reports, test cases, a regression checklist, and xmind maps

## **Live docs**
- GitHub Pages - [https://aleksei-eiskov.github.io/qa-portfolio-aleksei/](https://aleksei-eiskov.github.io/portfolio/)
- Files in repo - [docs/](./docs/)

## **Postman collections**
| Name | What's inside | File |
| - | - | - |
| Car_store - E2E stable (brand+car) | Create brand, create car linked to brand, update, relations, cleanup | [`postman/collections/21563877-86fc0407-cd06-4575-a376-6cb822943746.json`](./postman/collections/21563877-86fc0407-cd06-4575-a376-6cb822943746.json) |
| Car_store - CRUD collection | Basic CRUD for cars and brands, search, sorting, pagination | [`postman/collections/21563877-9eef265e-807b-4478-ab4f-939873db0428.json`](./postman/collections/21563877-9eef265e-807b-4478-ab4f-939873db0428.json) |

Quick preview without Postman:
- E2E overview - [`docs/car_store_collection_overview.md`](./docs/car_store_collection_overview.md)
- CRUD overview - [`docs/car_store_crud_overview.md`](./docs/car_store_crud_overview.md)


## Run locally
### Node
```bash
npm install
npm start
```

## **Docker**
docker build -t car_store .
docker run -p 3001:3001 car_store
# or
docker compose up --build

## **Key endpoints**
GET  /health
POST /reset

GET    /cars

POST   /cars

GET    /cars/:id

PUT    /cars/:id

PATCH  /cars/:id

DELETE /cars/:id


GET    /brands

GET    /brands/:id

GET    /brands/:id/cars

GET    /cars/:id/reviews

## QA PDFs
- Bug report examples - [bag-reports.pdf](./bag-reports.pdf)
 
- Test case examples - [test-cases.pdf](./test-cases.pdf)

- Regression checklist - [Regression.pdf](./Regression.pdf)
 
- XMind maps:
  - [Export list to CSV x_mind.pdf](./Export%20list%20to%20CSV%20x_mind.pdf)
  - [Comments and Mentions in a Document x_mind.pdf](./Comments%20and%20Mentions%20in%20a%20Document%20x_mind.pdf)
