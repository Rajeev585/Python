# `Python`

### `Constants`, `Classes`, `Methods`, `Protected Methods` and `Dunder Methods`
```python
# Get all the predefined constants, classes and methods in a module:
dir(module)
```

## `Constants`
- Constants are defined with all characters in `uppercase`
- e.g. COMPANY_NAME
- Find all the `constants` defined inside a module.
```python
print(list(filter(lambda c : c.isupper(), dir(module))))
```

## `Classes`
- Classes are defined with first character in `uppercase`
- e.g def Class_Name(object):
- Find all the `classes` defined inside a module.
```python
print(list(filter(lambda c : c.istitle(), dir(module))))
```

## `Methods`
- `Methods` are defined with `lowercase`
- e.g. def method_name():
- Find all the `methods` defined inside a module.
```python
print(list(filter(lambda c : c.islower(), dir(module))))
```

### `Dunder Methods`
- Methods defined which starts and ends with `__` ( Double underscore )
- e.g def `__init__(self)`
- Find all the `dunder methods` defined inside a module.
```python
print(list(filter(lambda c : c.startswith('__'), dir(module))))
```

### `Protected Methods`
- Methods defined which starts with `_` ( Single Underscore )
- e.g def \_calculate_salary(self):
- Find all the `protected methods` defined inside a module.
```python
print(list(filter(lambda c : c.startswith('_') and not c.startswith('__'), dir(module))))
``` 
