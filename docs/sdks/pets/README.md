# pets

### Available Operations

* [create_pets](#create_pets) - Create a pet
* [list_pets](#list_pets) - List all pets
* [show_pet_by_id](#show_pet_by_id) - Info for a specific pet

## create_pets

Create a pet

### Example Usage

```python
import hqtan_petstore_2


s = hqtan_petstore_2.HqtanPetstore2()


res = s.pets.create_pets()

if res.status_code == 200:
    # handle response
```


### Response

**[operations.CreatePetsResponse](../../models/operations/createpetsresponse.md)**


## list_pets

List all pets

### Example Usage

```python
import hqtan_petstore_2
from hqtan_petstore_2.models import operations

s = hqtan_petstore_2.HqtanPetstore2()

req = operations.ListPetsRequest(
    limit=548814,
)

res = s.pets.list_pets(req)

if res.pets is not None:
    # handle response
```

### Parameters

| Parameter                                                                | Type                                                                     | Required                                                                 | Description                                                              |
| ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ |
| `request`                                                                | [operations.ListPetsRequest](../../models/operations/listpetsrequest.md) | :heavy_check_mark:                                                       | The request object to use for the request.                               |


### Response

**[operations.ListPetsResponse](../../models/operations/listpetsresponse.md)**


## show_pet_by_id

Info for a specific pet

### Example Usage

```python
import hqtan_petstore_2
from hqtan_petstore_2.models import operations

s = hqtan_petstore_2.HqtanPetstore2()

req = operations.ShowPetByIDRequest(
    pet_id='provident',
)

res = s.pets.show_pet_by_id(req)

if res.pet is not None:
    # handle response
```

### Parameters

| Parameter                                                                      | Type                                                                           | Required                                                                       | Description                                                                    |
| ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
| `request`                                                                      | [operations.ShowPetByIDRequest](../../models/operations/showpetbyidrequest.md) | :heavy_check_mark:                                                             | The request object to use for the request.                                     |


### Response

**[operations.ShowPetByIDResponse](../../models/operations/showpetbyidresponse.md)**
