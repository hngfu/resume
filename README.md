# 이력서

## 링크

Github: [https://github.com/hngfu](https://github.com/hngfu)

## 코드스쿼드

### Store App

<img src="https://user-images.githubusercontent.com/38850628/58293206-84d20680-7dff-11e9-8b41-1bf2dd55201b.gif" width="400" style="max-width:100%;">

<img src="https://user-images.githubusercontent.com/38850628/58293521-aed7f880-7e00-11e9-8d1f-b3b40b72042c.png" width="400" style="max-width:100%;">

#### JSON형식의 데이터로 상품을 표시하고 해당 상품을 구매할 수 있는 앱.<br>(구매사실은 슬랙의 webHook으로 표현)

- `dataTask`를 사용하여 json데이터를 받아와 화면에 표시.
- `downloadTask`를 사용하여 이미지는 Cache처리.
- `uploadTask`를 사용하여 구매정보 POST.
- `CocoaPod`으로 'Toaster'를 설치하여 Cell 클릭시 해당 정보 Toast로 띄움.
- `Reachability`를 사용하여 인터넷 연결 상태에 따라 다른 동작하도록 핢.
- `AutoLayout` 적용

링크: [https://github.com/hngfu/swift-storeapp](https://github.com/hngfu/swift-storeapp)

----

### Photo App

<img src="https://user-images.githubusercontent.com/38850628/60394552-2d8f2680-9b61-11e9-83be-f0b7b37b2277.gif" width="400" style="max-width:100%;">

#### Photos Library를 이용한 사진앱.

- `PHAsset`을 사용하여 사진 이미지를 Cell에 표시.
- `AVAssetWriter`를 사용하여 3개 이상의 이미지로 3초 길이 비디오를 제작 만들도록 핢.
- Asset에 필터를 적용하거나 revert를 통해 필터를 제거할 수 있도록 핢.
- Photo Library를 Observing하여 변경되면 업데이트 하도록 핢.
- `UIMenuItem`를 사용하여 이미지를 저장할 수 있도록 핢.
- `Instruments`를 사용하여 네트워크 성능을 측정하여 효율적으로 이미지를 다운로드 받도록 핢.
- `AutoLayout` 적용

링크: [https://github.com/hngfu/swift-photoapp](https://github.com/hngfu/swift-photoapp)

----

### CardGame App (Klondike Solitaire)

<img src="https://user-images.githubusercontent.com/38850628/54986018-38cc3680-4ff5-11e9-862b-efa2d4e45583.gif" width="400" style="max-width:100%;">

#### 더블탭과 드래그를 이용한 카드게임 앱.

- `UIGestureRecognizer`를 사용하여 드래그가 가능하도록 핢.
- `Animation` 적용.
- `AutoLayout` 적용.

링크: [https://github.com/hngfu/swift-cardgameapp](https://github.com/hngfu/swift-cardgameapp)

----

### Universal App

<img src="https://user-images.githubusercontent.com/38850628/60598551-d5b62100-9de7-11e9-90a7-6f361eadae4f.png" width="400" style="max-width:100%;">

#### 국제화, 지역화, 파편화를 이용한 영화배우 프로필 앱.

- `System Region`에 해당하는 배우의 정보를 `System Language`로 표시.<br>(단, 생일정보의 Language는 Region의 설정된 대로 나오도록 핢)
- iOS 11.0 이상인 경우 `UIFontMetrics`에서 `scaledFont`의 기능을 활용하도록 핢.
- `AutoLayout` 적용.

링크: [https://github.com/hngfu/swift-universalapp](https://github.com/hngfu/swift-universalapp)

----

### WebView App

<img src="Images/webViewApp.png" width="400" style="max-width:100%;">

- 설명: 메뉴 정보를 JSON형식으로 가져와서 콘솔창에 출력해주는 앱.

링크: [https://github.com/hngfu/swift-webviewapp](https://github.com/hngfu/swift-webviewapp)

----

### Address App

<img src="Images/addressApp.png" width="400" style="max-width:100%;">

- 설명: 초성검색도 가능한 연락처 앱.

링크: [https://github.com/hngfu/swift-addressbookapp](https://github.com/hngfu/swift-addressbookapp)

----

### VendingMachine App

<img src="Images/vendingMachineApp.png" width="600" style="max-width:100%;">

- 설명: 자판기에 물품, 돈을 추가하거나 물품을 구입할 수있는 앱.

링크: [https://github.com/hngfu/swift-vendingmachineapp](https://github.com/hngfu/swift-vendingmachineapp)

## 개인프로젝트

### HngfuIsSwift

<img src="Images/hngfuisswift.jpg" width="400" style="max-width:100%;">

- 설명: 단축키를 이용해 사이트를 새창으로 띄워주는 앱.
- 사용기술: chrome.storage API, html, javascript

Chrome Web Store: [https://chrome.google.com/webstore/detail/hngfuisswift/mkklklabflcildhpimhojcclkndjcpja?hl=ko](https://chrome.google.com/webstore/detail/hngfuisswift/mkklklabflcildhpimhojcclkndjcpja?hl=ko)

[Chrome Web Store](https://chrome.google.com/webstore/category/extensions?hl=ko)에서 `HngfuIsSwift`로 검색 가능


## 발표

### 코드 파티

점점 짧아지고 간결해지는 진화하는 fizz buzz 코드  
그리고 직접 만든 operator

<img width="600" src="Images/CodeParty.png">

[코드 파티.pdf 링크](https://github.com/hngfu/presentation/blob/master/asset/%EC%BD%94%EB%93%9C%ED%8C%8C%ED%8B%B0%202019-01-08.pdf)

### 흥푸의 추일함타

추상화, 일반화, 함수, 타입에 대하여...

<img width="600" src="Images/흥푸의 추일함타.png">

[추일함타.pdf 링크](https://github.com/hngfu/presentation/blob/master/asset/%ED%9D%A5%ED%91%B8%EC%9D%98%20%EC%B6%94%EC%9D%BC%ED%95%A8%ED%83%80%20ver.2.pdf)

### Hngfu's UnitTest

단위 테스트는 무엇이고 어떻게 하는 걸까?

<img width="600" src="Images/Hngfu's UnitTest.png">

[Hngfu's UnitTest.pdf 링크](https://github.com/hngfu/presentation/blob/master/asset/Hngfu's%20UnitTest.pdf)

### 오토 레이아웃만으로 구현한 신기한 스크롤 뷰

오토 레이아웃 만으로 구현한  
아래로 끌면 사진이 커지는 스크롤 뷰

<img width="400" src="Images/autoLayout.gif">

[스크롤 뷰 code 링크](https://github.com/hngfu/presentation/tree/master/asset/FirstLayout)
