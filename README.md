# Openlog Specification

Example will be in example.openlog

Sample regex for parsing can be found in spec.regex.

### Start Identification Regexs

```python
todo_pattern = r"^\*\s*\[([\sx])*\]\s*\:.*" #starts like * [ ] :
logtime_pattern = r"^\*\s*(\d{1,2})\:?(\d{2})\s*\-\s*(\d{1,2})\:?(\d{2})\s*\:.*"
```

### Line tokens Identification Regex
```python
logline_pattern =  r"\s*([^\@\#\[\]\\]*(\\[\@\#\[\]\\])*)+(\@\w+\s*)*(\#\w+\s*)*(\[\w+\])?\.?$"
```
