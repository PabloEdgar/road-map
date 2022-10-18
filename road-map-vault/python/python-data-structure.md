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


