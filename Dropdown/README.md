## DropdownButton
Creates a dropdown with 4 options. Normally would have a underline. To remove it add a Container in the underline property.

```
DropdownButton<String>(
    underline: Container(),
    value: _value,
    value: _value,
    items: ['Option1', 'Option2', 'Option3', 'Option4']
        .map((String value) {
    return DropdownMenuItem<String>(
        value: value,
        child: new Text(value),
    );
    }).toList(),
    onChanged: (String? update) {
    setState(() {
        _value = update!;
    });
    },
),
```

