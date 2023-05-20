### Navigator.replace

```dart
MaterialButton(
            onPressed: () {
              Navigator.replace(context,
                  oldRoute: MaterialPageRoute(
                    builder: (context) =>
                        HomePage(title: 'My Home Page', count: 0),
                  ),
                  newRoute: MaterialPageRoute(
                    builder: (context) => NewNewPage(),
                  ));
            },
            child: Text('NewNewPage'),
            color: Colors.grey,
          )
```

### Navigator.pushAndRemoveUntil

```dart
Navigator.pushAndRemoveUntil(
context, 
MaterialPageRoute(builder: (BuildContext context) => HomePage()),
(route) => false);)
```

1. 열려있는 모든 창을 끔
2. 그리고는 새창으로 감
3. 이 방법으로 push를 통해 열려있는 모든 창을 pop