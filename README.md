#JsonApiClient

fork of: [chingor13/json_api_client v1.0.1](https://github.com/chingor13/json_api_client)


##Remove BelongsTo Attributes During Create And Update
This branch removes belongs_to attributes when sending a post request. This is because the belongs to attributes are sent in the url, and therefore are redundant. Sending redundant params in the body can affect api's that throw exceptions on unpermitted params.