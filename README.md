# 이력서

## 링크

Github: [https://github.com/hngfu](https://github.com/hngfu)

## 코드스쿼드

### Store App

<img src="https://user-images.githubusercontent.com/38850628/58293206-84d20680-7dff-11e9-8b41-1bf2dd55201b.gif" width="400" style="max-width:100%;">

<img src="https://user-images.githubusercontent.com/38850628/58293521-aed7f880-7e00-11e9-8d1f-b3b40b72042c.png" width="400" style="max-width:100%;">

#### JSON 형식의 데이터로 상품을 표시하고 해당 상품을 구매할 수 있는 앱. <br> (구매 사실은 슬랙의 webHook으로 표현)

- `dataTask`를 사용하여 JSON 데이터를 받아와 화면에 표시.
- `downloadTask`를 사용하여 이미지는 Cache 처리.
- `uploadTask`를 사용하여 구매정보 POST.
- `CocoaPod`으로 'Toaster'를 설치하여 Cell 클릭 시 해당 정보 Toast로 띄움.
- `Reachability`를 사용하여 인터넷 연결 상태에 따라 다르게 동작하도록 함.
- `AutoLayout` 적용.

링크: [https://github.com/hngfu/swift-storeapp](https://github.com/hngfu/swift-storeapp)

----

### Photo App

<img src="https://user-images.githubusercontent.com/38850628/60394552-2d8f2680-9b61-11e9-83be-f0b7b37b2277.gif" width="400" style="max-width:100%;">

#### Photos Library를 이용한 사진 앱.

- `PHAsset`을 사용하여 사진 이미지를 Cell에 표시.
- `AVAssetWriter`를 사용하여 3개 이상의 이미지로 3초 길이 비디오를 제작할 수 있도록 함.
- Asset에 필터를 적용하거나 revert를 통해 필터를 제거할 수 있도록 함.
- Photo Library를 Observing 하여 변경되면 업데이트하도록 함.
- `UIMenuItem`을 사용하여 이미지를 저장할 수 있도록 함.
- `Instruments`를 사용하여 네트워크 성능을 측정하여 효율적으로 이미지를 다운로드하도록 함.
- `AutoLayout` 적용.

링크: [https://github.com/hngfu/swift-photoapp](https://github.com/hngfu/swift-photoapp)

----

### CardGame App (Klondike Solitaire)

<img src="https://user-images.githubusercontent.com/38850628/54986018-38cc3680-4ff5-11e9-862b-efa2d4e45583.gif" width="400" style="max-width:100%;">

#### 더블 탭과 드래그를 이용한 카드게임 앱.

- `UIGestureRecognizer`를 사용하여 드래그할 수 있도록 함.
- `Animation` 적용.
- `AutoLayout` 적용.

링크: [https://github.com/hngfu/swift-cardgameapp](https://github.com/hngfu/swift-cardgameapp)

----

### Universal App

<img src="https://user-images.githubusercontent.com/38850628/60598551-d5b62100-9de7-11e9-90a7-6f361eadae4f.png" width="400" style="max-width:100%;">

#### 국제화, 지역화, 파편화를 이용한 영화배우 프로필 앱.

- `System Region`에 해당하는 배우의 정보를 `System Language`로 표시. <br> (단, 생일 정보의 Language는 Region의 설정된 대로 나오도록 함)
- iOS 11.0 이상일 때 `UIFontMetrics`에서 `scaledFont`의 기능을 활용하도록 함.
- `AutoLayout` 적용.

링크: [https://github.com/hngfu/swift-universalapp](https://github.com/hngfu/swift-universalapp)

----

### WebView App

<img src="https://user-images.githubusercontent.com/38850628/56403593-ff59b480-629c-11e9-9af1-879586b8bd42.png" width="400" style="max-width:100%;">

#### 메뉴 정보를 JSON 형식으로 가져와서 콘솔 창에 출력해주는 웹뷰 앱.

- js 코드를 인젝션 하여 원하는 태그의 데이터를 JSON 형식으로 가져오도록 함.
- 특정 메뉴를 호출하는 경우 `SafariViewController`로 띄우도록 함.

링크: [https://github.com/hngfu/swift-webviewapp](https://github.com/hngfu/swift-webviewapp)

----

### Address App

<img src="https://user-images.githubusercontent.com/38850628/55726605-22899600-5a4b-11e9-92f6-5d763b2ddbdb.png" width="400" style="max-width:100%;">

#### 초성 검색도 가능한 연락처 앱.

- 유니코드로 한글을 분석하여 초성 검색이 가능하도록 함.
- 애플 샘플 코드 중 `MGCContactStore` 클래스를 활용.
- `indexTitle` 설정.

링크: [https://github.com/hngfu/swift-addressbookapp](https://github.com/hngfu/swift-addressbookapp)


## 개인프로젝트

### HngfuIsSwift

<img src="https://user-images.githubusercontent.com/38850628/61694529-9c306000-ad6c-11e9-80f3-210eee6377e0.jpg" width="400" style="max-width:100%;">

- 단축키를 이용해 사이트를 새 창으로 띄워주는 앱.
- 사용 기술: chrome.storage API, html, javascript

Chrome Web Store: [https://chrome.google.com/webstore/detail/hngfuisswift/mkklklabflcildhpimhojcclkndjcpja?hl=ko](https://chrome.google.com/webstore/detail/hngfuisswift/mkklklabflcildhpimhojcclkndjcpja?hl=ko)

[Chrome Web Store](https://chrome.google.com/webstore/category/extensions?hl=ko)에서 `HngfuIsSwift`로 검색 가능


## 발표

### 오토 레이아웃만으로 구현한 신기한 스크롤 뷰

오토 레이아웃 만으로 구현한  
아래로 끌면 사진이 커지는 스크롤 뷰

<img width="400" src="https://user-images.githubusercontent.com/38850628/61694525-9b97c980-ad6c-11e9-9db4-80177637fc31.gif">

[스크롤 뷰 code 링크](https://github.com/hngfu/presentation/tree/master/asset/FirstLayout)

### 흥푸의 추일함타

추상화, 일반화, 함수, 타입에 대하여...

<img width="600" src="https://user-images.githubusercontent.com/38850628/61694524-9b97c980-ad6c-11e9-824a-61c140b94916.png">

[추일함타.pdf 링크](https://github.com/hngfu/presentation/blob/master/asset/%ED%9D%A5%ED%91%B8%EC%9D%98%20%EC%B6%94%EC%9D%BC%ED%95%A8%ED%83%80%20ver.2.pdf)

### Hngfu's UnitTest

단위 테스트는 무엇이고 어떻게 하는 걸까?

<img width="600" src="https://user-images.githubusercontent.com/38850628/61694528-9c306000-ad6c-11e9-9802-ae6beb7d2855.png">

[Hngfu's UnitTest.pdf 링크](https://github.com/hngfu/presentation/blob/master/asset/Hngfu's%20UnitTest.pdf)

### 코드 파티

점점 짧아지고 간결해지는 진화하는 fizz buzz 코드  
그리고 직접 만든 operator

<img width="600" src="https://user-images.githubusercontent.com/38850628/61694527-9b97c980-ad6c-11e9-8c27-f650a6c303de.png">

[코드 파티.pdf 링크](https://github.com/hngfu/presentation/blob/master/asset/%EC%BD%94%EB%93%9C%ED%8C%8C%ED%8B%B0%202019-01-08.pdf)
