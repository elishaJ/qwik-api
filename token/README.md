
## API Reference

#### Get OAuth Access Token
```http
  GET /token
```

| Parameter       | Type     | Description                                 |
| :-------------- | :------- | :------------------------------------------ |
| `email` | `string` | **Required**. Access token |
| `api_key`     | `string` | **Required**. API Key generated on Cloudways Platform API Section|

##### Response
```json
{
    "token": "rJExcll8AaBuWwUvDInRc3z3a565F1AaIEeYAHc7"
}
```