A request to:

http://localhost:5001/api/v0/object/get?arg=/ipfs/QmPE6xb88LKNkwptiAsKNQ2Tryd8S8r9CBs1t9fXh9cY

Returns JSON like:

```json
{
  "Links": [
    {
      "Name": "viz.html",
      "Hash": "QmfY5W7vwrD9FycZNg3zikZSpcRwPDwDJp21b3NqMM8dw5",
      "Size": 4743
    }
  ],
  "Data": "\u0008\u0001"
}
```

Ideal future format of recursive call to `object/links`:

{
  "Hash": "Qmcav25eTinMV632w9zdyXsFENDz5FCWjrMEVU7Nzy2v98",
  "Links": [
    {
      "Name": "app.js",
      "Hash": "QmZs8mitpfSZM8TaFas9WaDVF77aQvb47UEPR1g1quoQq9",
      "Size": 500
    },
    {
      "Name": "lib",
      "Hash": "QmSXq83RU9YFnxGS7N29gBqjMXTg3qHERzrfFZxKYCGknM",
      "Size": 520503,
      "Links": [
        {
          "Name": "d3.js",
          "Hash": "QmbgWP6n7wmczy9YP79FpDRUjYhyjVKjdDHTm9SS9nadZR",
          "Size": 336528
        }
      ]
    }
  ]
}

