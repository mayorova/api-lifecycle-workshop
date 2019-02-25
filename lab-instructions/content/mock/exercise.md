---
title: "Exercise"
weight: 1
---

## Expose a Mock of the ACME Brewery API!

As the ACME Brewery API matures, the sales representative of the ACME Brewery already found his first customers. In this exercise, you will have to **expose a mock of the ACME Brewery API** so that future customers can start their implementation ahead and provide feedback early.

- Install [Postman](https://www.getpostman.com/downloads/)
- Load [this collection](postman_collection.json) in Postman
- Examine the provided examples
- Discover the mocks generated by [Microcks]({{< param microcks_url >}}/#/services)
- Try to use the generated mock using the following URLs:

```sh
curl -D - {{< param microcks_url >}}/rest/Beer+Catalog+API/1.0/beer?page=0
```

```sh
curl -D - {{< param microcks_url >}}/rest/Beer+Catalog+API/1.0/beer/Weissbier
```

```sh
curl -D - {{< param microcks_url >}}/rest/Beer+Catalog+API/1.0/beer/findByStatus/available
```

```sh
curl -D - {{< param microcks_url >}}/rest/Beer+Catalog+API/1.0/beer/findByStatus/out_of_stock
```

To complete your understanding, explain **how the mock is generated** and **how the future customers of ACME can use it to develop their implementation ahead**.