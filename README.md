
# Article API Documentation

This API allows you to create, read, update, and delete articles.


## Base URL

The base URL for this API is [here](https://web-production-5865.up.railway.app/)




## API Reference

#### Get all items

```http
  GET /
```

### Example Response

```
{
    "id": 1,
    "title": "First Title of Article",
    "description": "hello world"
},
{
    "id": 2,
    "title": "Second Title of Article",
    "description": "hello world 2"
}
```

#### Create an Article

```http
POST /
```

| Parameter | Type     | Description                | Max Length     |
| :-------- | :------- | :------------------------- | :------- |
| `title` | `string` | **Required**. Title for the article | `100` |
| `description` | `string` | **Required**. Description for the article | `500` |



### Example Response

```
{
    "id": 10,
    "title": "New Article",
    "description": "hello world"
}
```

### Retrieve an Article

```http
GET /<id>
```

### Example Response

```
{
    "id": 10,
    "title": "10th Article",
    "description": "hello world 10"
}
```


### Update an Article

```http
GET /<id>
```

| Parameter | Type     | Description                | Max Length     |
| :-------- | :------- | :------------------------- | :------- |
| `title` | `string` | **Required**. Title for the article | `100` |
| `description` | `string` | **Required**. Description for the article | `500` |


### Example Response

```
{
    "id": 10,
    "title": "Updated Title",
    "description": "hello world 10"
}
```


### Delete an Article

```http
GET /<id>
```

| Parameter | Type     | Description                | Max Length     |
| :-------- | :------- | :------------------------- | :------- |
| `title` | `string` | **Required**. Title for the article | `100` |
| `description` | `string` | **Required**. Description for the article | `500` |
