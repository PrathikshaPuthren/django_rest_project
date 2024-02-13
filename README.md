# API Documentation

## List Stocks Endpoint

- **URL**: `/list-stocks/`
- **HTTP Method**: GET
- **Authentication**: Token authentication required
- **Permissions**: Only admin users can access this view
- **Description**: Returns a list of all stocks available.

### Response:
- **Status Code**: 200 OK
- **Content Type**: application/json

```json
[
    {
        "sku": "ABC123",
        "name": "Product Name 1",
        "category": "Category 1",
        "tags": ["Tag1", "Tag2"],
        "stock_status": "In Stock",
        "available_stock": 100
    },
    {
        "sku": "XYZ456",
        "name": "Product Name 2",
        "category": "Category 2",
        "tags": ["Tag3", "Tag4"],
        "stock_status": "Out of Stock",
        "available_stock": 0
    },
    ...
]
