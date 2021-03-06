# x\-amazon\-apigateway\-documentation Object<a name="api-gateway-swagger-extensions-documentation"></a>

Defines the documentation parts to be imported into API Gateway\. This object is a JSON object containing an array of the `DocumentationPart` instances\.


**Properties**  

| Property Name | Type | Description | 
| --- | --- | --- | 
| documentationParts | Array |   An array of the exported or imported `DocumentationPart` instances\.  | 
| version | String |   The version identifier of the snapshot of the exported documentation parts\.  | 

## x\-amazon\-apigateway\-documentation Example<a name="api-gateway-swagger-extensions-documentation-example"></a>

 The following example of the API Gateway extension to Swagger defines `DocumentationParts` instances to be imported to or exported from an API in API Gateway\. 

```
{ ...
  "x-amazon-apigateway-documentation": {
    "version": "1.0.3",
    "documentationParts": [
       {
         "location": {
           "type": "API"
       },
        "properties": {
          "description": "API description",
          "info": {
            "description": "API info description 4",
            "version": "API info version 3"
          }
        }
      },
      {
         … // Another DocumentationPart instance
      }
    ]
  }
}
```