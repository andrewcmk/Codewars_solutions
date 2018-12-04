
<h4>
Kata: </br>
Implement the function unique_in_order which takes as argument a sequence and turns a list of tems without any elements with the same value next to each other and preserving the original order of elements.
</h4>
</br>


For example:</br>

unique_in_order('AAAABBBCCDAABBB')  ==  ['A', 'B', 'C', 'D', 'A', 'B'] </br>
unique_in_order('ABBCcAD')          ==  ['A', 'B', 'C', 'c', 'A', 'D'] </br>
unique_in_order([1,2,2,3,3])        ==  [1,2,3] </br>


```python
def unique_in_order(iterable):
    foo = []
    for item in iterable:
        if len(foo) < 1 or not item == foo[len(foo) -1]:
            foo.append(item)
    return foo

```
