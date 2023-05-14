ListView란?

→ 일반적으로 사용하는 스크롤 위젯

ListView를 사용하는 3가지 방법

1. 일반적인 ListView
- listview를 Expanded로 감싸준다
    
    ![스크린샷 2023-05-14 111457](https://github.com/ljyo2o9/EDITH/assets/126755727/341bd121-76a7-4ffc-adb3-34cde6b95d3b)
    
Expanded를 사용하는 이유

- ListView는 부모 위젯의 높이에 따라 높이를 맞춤
- Column의 높이는 무한임
- ListView의 높이도 무한으로 지정되어 에러가 생김
1. ListView.builder
- ListView.builder를 사용

![스크린샷 2023-05-14 111520](https://github.com/ljyo2o9/EDITH/assets/126755727/8e5b1f02-d38f-482b-926b-3847feb26538)

사용방법

- ListView에 사용할 LIst를 정하고
- itembuilder를 사용하여 item을 itemcount에 맞춘다
- 그리고는 ListVIew를 구성후 사용

사용하는 이유

- 화면에 보여지는 리스트를 그때그때마다 호출함
- 보이는 부분만 불러오기 가능
    
    ++ ListView보다 효율적으로 화면을 구성할 수 있음
    
1. LIstView.separated
- ListView.separated는 구분선
    
    ![스크린샷 2023-05-14 103838](https://github.com/ljyo2o9/EDITH/assets/126755727/f94206ab-0152-4721-bf42-5b7f26fdab14)


사용방법

- ListView.builder와 사용방법은 같다
- 다만 구분선이 추가된 형태라고 생각하면 편하다

사용하는 이유

- 마찬가지로 구분선을 사용하기위해 사용함