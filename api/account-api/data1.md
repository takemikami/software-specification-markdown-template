# Data1

Data1 access API.

Relative Datastore: Data1

## APIs

### Get List

Endpoint: GET ``<service-domain>/account/{account id}/data1``

Parameter:  
None. (In the future, Search & Filter options will come.)

Output: List of Data1 Model

### Get Detail

Endpoint: GET ``<service-domain>/account/{account id}/data1/{data1 id}``

Output: Data1 Model

### Create

Endpoint: POST ``<service-domain>/account/{account id}/data1``

Input: Data1 Model

### Update

Endpoint: PUT ``<service-domain>/account/{account id}/data1/{data1 id}``

Input: Data1 Model

### Delete

Endpoint: DELETE ``<service-domain>/account/{account id}/data1/{data1 id}``

## Model

Data1:

- Data1ID
- Name
- Body
- Something
