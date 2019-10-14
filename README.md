# list_view

A new Flutter project.

## Getting Started

ListView is same like a column and row widget, ListView is like a layout, it's can be set Horizontal and Vertical. The widgets inside the ListView is never overfloat or Scrollable.

```dart
ListView(
  children: <Widget>[
    Row(
      mainAxisAlignment: MainAxisAlignment.spaceAround,
      children: <Widget>[
        RaisedButton(
          child: Text('TAMBAH'),
          onPressed: () {
            setState(() {
              widgets.add(Text(
                'Ini data ke-$counter',
                style: TextStyle(fontSize: 20, color: Colors.teal),
              ));
              counter++;
            });
          },
        ),
        RaisedButton(
          child: Text('KURANG'),
          onPressed: () {
            setState(() {
              widgets.removeLast();
              counter--;
            });
          },
        )
      ],
    ),
    Column(
      crossAxisAlignment: CrossAxisAlignment.start,
      children: widgets,
    )
  ],
)
```
