<!-- Start SDK Example Usage [usage] -->
```python
import hqtan_petstore_2

s = hqtan_petstore_2.HqtanPetstore2()


res = s.pets.create_pets()

if res.status_code == 200:
    # handle response
    pass
```
<!-- End SDK Example Usage [usage] -->