# Notes on jupyter notebooks

# A hidden_cell annotation

Supposedly this an annotation for removing a cell from being pushed to git.  I have not tested it yet, but I learned 
about it at the 2023 IBM TechXchang conference.
```
@hidden_cell
```

# Hiding output

This will hide a cells output. Particulary good for `pip install` cells.

```
@collapse
```
