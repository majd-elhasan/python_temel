```python
def Reverse(List):
    List.reverse()
    for i in range(len(List)):
        if (type(List[i]) == list):  
            Reverse(List[i])
def input_list(inputList):
    Reverse(inputList)
    return inputList

```
<span style="color:blue">--------------------------------------------------------------------------------------------------------------------------
    </span>

### the nested list must be input as list not as string directly to the function below ↓
 input_list (<font color='red'>*the list*</font>)
 or as example .. input_list (<font color='red'> [[1, 2], [3, 4], [5, 6, 7]] </font>) 
 
 <span style="color:blue">--------------------------------------------------------------------------------------------------------------------------
    </span>
    
 
```python
input_list([[1, 2], [3, 4], [5, 6, 7]])

```
output : ` [[7, 6, 5], [4, 3], [2, 1]]`