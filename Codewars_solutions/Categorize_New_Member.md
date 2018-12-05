<h4>kata</h4>
The Western Suburbs Croquet Club has two categories of membership, Senior and Open. They would like your help with an application form that will tell prospective members which category they will be placed.
</br>
To be a senior, a member must be at least 55 years old and have a handicap greater than 7. In this croquet club, handicaps range from -2 to +26; the better the player the lower the handicap.
</br>

<h4>Input</h4>
Input will consist of a list of lists containing two items each. Each list contains information for a single potential member. Information consists of an integer for the person's age and an integer for the person's handicap.
</br>
Note for F#: The input will be of (int list list) which is a List>

<h4>Example Input</h4>
[[18, 20],[45, 2],[61, 12],[37, 6],[21, 21],[78, 9]]
</br>

<h4>Output</h4>
Output will consist of a list of string values (in Haskell: Open or Senior) stating whether the respective member is to be placed in the senior or open category.
</br>

<h4>Example Output</h4>
["Open", "Open", "Senior", "Open", "Open", "Senior"]
</br>

<h4>solution</h4>

```python
def openOrSenior(data):
    list = []
    for age, handicap in data:
        if age >= 55 and handicap > 7:
            list.append('Senior')
        else: list.append('Open')
    return list
```

