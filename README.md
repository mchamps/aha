This is in no way associated with Aha.io. For Aha.io API documentation, please visit https://aha.io/api.

## Extracting Data From Aha.io

### Postman Collection

In this repository I have included a Postman collection for getting started with data extraction from Aha.io.

### Extracting Data via Python w/ ahapy

- https://pypi.org/project/ahapy/
- https://github.com/henkhaus/ahapy


Install ahapy:

```
pip install ahapy
```

Example python for how to get all initiatives:

```python
from ahapy import AhaV1

aha = AhaV1('yourAHAsubdomain', 'yourAPIkey')

data = aha.query('initiatives')

for i in data:
    print(i)
```
