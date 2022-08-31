## Extracting Data From Aha.io

### Postman Collection

I have included a Postman collection for getting started with data extraction from Aha.io.

### Extracting Data via Python w/ ahapy

https://pypi.org/project/ahapy/

```python
from ahapy import AhaV1

aha = AhaV1('yourAHAsubdomain', 'yourAPIkey')

data = aha.query('initiatives')

for i in data:
    print(i)
```
