```python
container = []
def shred(List):
    for i in range(len(List)):
        if (type(List[i]) == list):
            shred(List[i])
        else: container.append(List[i])
    return
def eliminate(nestedList):
    shred(nestedList)
    copy = container.copy()
    container.clear()
    return copy

```
<span style="color:blue">--------------------------------------------------------------------------------------------------------------------------
    </span>

### the nested list must be input as list not as string directly to the function below ↓
 eliminate (<font color='red'>*the list*</font>)
 or as example .. eliminate (<font color='red'> [[1,'a',['cat'],2],[[[3]],'dog'],4,5] </font>) 
 
 <span style="color:blue">--------------------------------------------------------------------------------------------------------------------------
    </span>
    
 
```python
eliminate([[1,'a',['cat'],2],[[[3]],'dog'],4,5])

```
output : ` [1, 'a', 'cat', 2, 3, 'dog', 4, 5]`

```python
eliminate([[1, 2], [3, 4], [5, 6, 7]])

```
output : `[1, 2, 3, 4, 5, 6, 7]`