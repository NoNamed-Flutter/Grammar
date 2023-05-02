- List(배열), index(순서)
    
    List<String> Vsc = [’Flutter’, ‘Dart’, ‘Code’, ‘Factory’];
    
    List<int> nums = [1, 2, 3, 4, 5, 6];
    
    ---
    
    print(Vsc); << [Flutter, Dart, Code, Factory]
    
    print(nums); << [1, 2, 3, 4, 5, 6] 으로 출력
    
    ---
    
    print(Vsc[0]); << Flutter
    
    print(Vsc[1]); << Dart
    
    ---
    
    print(Vsc.length); << 4가 출력
    
    Vsc.add(’C’);
    
    print(Vsc) << [Flutter, Dart, Code, Factory, C]가 출력
    
    Vsc.remove(’C’);
    
    print(Vsc) << [Flutter, Dart, Code, Factory]가 출력
    
    print(Vsc.indexOf(’Dart’)); << 1
    
- Map
    
    Map<String, bool> isHarryPotter = {
    
    ‘Harry Potter’ : true,
    
    ‘Ron Weasley’ : true,
    
    ‘Ironman’ : false,
    
    };
    
    print(isHarryPotter); 위 출력
    
    isHarryPotter.addAll({
    
    ‘Spiderman’ : false,
    
    });
    
    그냥 isHarryPotter[’Hulk’] = false;를 해도 추가됨
    
    print(isHarryPotter); Spiderman이 추가되서 출력
    
    print(isHarryPotter[’Ironman’]); << false가 출력 value값이 출력
    
    isHarryPotter.remove(’Ironman’); << Ironman 삭제
    
    print(isHarryPotter.keys); << key들만 출력
    
    print(isHarryPotter.values); << values들만 출력
    
    ---
    
- Set
    
    final Set<String> names = {
    
    ‘Flutter’,
    
    ‘Dart’,
    
    ‘C’,
    
    };
    
    print(names); << {FLutter, Dart, C}출력
    
    ++똑같은 C를 넣으면 똑같은게 안생기고 알아서 중복처리를
    
    names.add(’Python’);
    
    names.remove(’Python;);
    
    print(names.contains(’Flutter’)) << true(Flutter가 있는지 확인)

    - enum
    
    ```dart
    enum Vsc {
      Flutter,
      Dart,
      Python,
    }
    
    void main() {
      Vsc vsc = Vsc.Flutter;
    	//enum '변수명' = enum.enum의변수명
      if (vsc == Vsc.Flutter) {
        print("Flutter입니다");
      } else if (vsc == Vsc.Dart) {
        print("Dart입니다");
      } else {
        print("Python");
      }
    }
    ```