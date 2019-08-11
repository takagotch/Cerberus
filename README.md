### Cerberus
---
https://github.com/TedGoas/Cerberus

.py
https://github.com/pyeve/cerberus

```py
v = Validator({'name': {'type': 'string'}})
v.validate({'name': 'john doe'})

v = Validator()
v.validate(document, schema)

schema = {'name': {'type': 'string'}, 'age': {'type': 'integer', 'min': 10}}
document = {'name': 'Little Joe', 'age': 5}
v.validate(document, schema)
v.errors

document = {'name': 'john doe'}
v(document)

schema = {'name': {'type': 'string', 'maxlength': 10}}
v.validate({'name': 'john', 'sex': 'M'}, schema)

v.schema = {}
v.allow_unknown = True
v.validate({'name': 'john', 'sex': 'M'})
```

```sh
pip install cerberus
python setup.py test
pip install tox
tox
```

```
```

