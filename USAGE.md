<!-- Start SDK Example Usage -->
```python
import hqtan_petstore_2


s = hqtan_petstore_2.HqtanPetstore2()


res = s.pets.create_pets()

if res.status_code == 200:
    # handle response
```
<!-- End SDK Example Usage -->