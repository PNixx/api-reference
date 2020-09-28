# Product recommendations

Service provides access to product recommendations endpoint.

## Request product recommendations

### HTTP Request

`GET https://api.rees46.com/recommend`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
did | true | Device ID. You get it from `init` method in SDK.
shop_id | true | Your API key
seance | true | Temporary user session ID
recommender_type | true | Always `dynamic`
recommender_code | true | ID of product recommendations block. You get it from blocks management UI.
locations | false | Location ID
extended | false | Supports: `1` or empty. If `1`, it will return all information about recommended products. If omit, it returns only products IDs.
