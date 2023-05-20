### Navigator.push

```dart
Navigator.push(context, MaterialPageRoute(builder: (context) ⇒ NextPage()),);
```

1. 현재 페이지를 스택에 삭제
2. NextPage라는 이름을 가진 페이지로 이동

### Navigator.pop

```dart
Navigator.pop(context);
```

1. 현재 페이지를 스택에서 제거 
2. 이전 페이지로 이동
3. 만약 스택에 페이지가 없다면 앱이 종료