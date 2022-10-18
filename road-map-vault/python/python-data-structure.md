___
# classes
```python
class Item:
    def __init__(self, itemType = None):
        self.itemType = itemType
```
___
# instances
```python
item = Item(itemType = 'myItemType')
```

## instances use cases
### insntance vs listInstances
```python
itemList = [
    Item(itemType = 'myItemType'),
    Item(itemType = 'myOtherItemType'),
    Item(itemType = 'myThirdItemType')
]

for item in itemList:
    ###- do something with the item here
    myMethod(item)
```

### equals
```python
from python_helper import ObjectHelper

class User:
    def __init__(self, name, father):
        self.name = name,
        self.father = father

user_father = User('pedro', None)
user_1 = User('samuel', user_father)
user_2 = User('samuel', user_father)

assert ObjectHelper.equals(user_1, user_2), f'should be equals {user_1} == {user_2}'
assert user_1 == user_2, f'should not be equals {user_1} == {user_2}'
```
___
# functions
```python
def myMethod(something):
    ###- do something
    return True
```

## functions use cases
- ### wrong use
```python
###- COMPLETELY WRONG!!!!!
myMethod(Item)

###- RISCKY!!!!
myMethod(itemList[2])
```
- ### correct use
```python
myMethod(item)
```

___ 
# utilities
- python-helper
	https://github.com/SamuelJansen/python-helper/tree/master/python_helper/api/src/service

