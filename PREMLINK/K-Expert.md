# K-Expert

중국인 타겟의 한국 뷰티 서비스 '찐' 리뷰 플랫폼

## Web

<a href="https://youtu.be/Bm9cZo092_E">
<img src = "https://github.com/user-attachments/assets/7c92d14e-b188-4c76-8a7b-017d8c5edf0d" width = 600/>
</a>

⬆ 이미지를 클릭하시면 서비스를 간략하게 보실 수 있는 영상으로 이동합니다.(Youtube)
<br/>

### 사용 기술

- Front-end: Next.js
- Back-end: NestJS
- Infra: AWS (EC2, VPC, Route 53, Amplify, CloudFront, CloudWatch, ELB, S3..)
- Database: MongoDB
- Analytics: Plausible (On-premise)
- Logging: AWS CloudWatch, Sentry
  <br/>

### 주저리주저리

#### 대박나면 어쩌지?

'서비스 출시하고 대박나서 사람들 엄청 몰리면 어쩌지?'라는 고민을 했었다.
그래서 사람들이 매우 몰렸을 때를 가정하고 서비스를 구축했다.

인프라 구축할 때 고가용성을 염두에 두어 가용 영역(Availity Zone)을 분리하고 이용량이 올라가면 자동으로 Scale-Out 하도록 구현했다. 그리고 보안도 신경 써서 subnet도 public/private을 나누어 private의 경우에는 NAT Gateway를 통해 인터넷 통신을 하도록 구현했다. 대박 나서 사용자들이 몰려 내가 했던 수고들이 빛을 발했으면 좋았을 텐데 살짝 아쉬운 마음이 있다.

#### 웹 어플리케이션 배포

Next.js 배포 시 매우 쉽게 사용할 수 있는 Vercel을 두고 굳이 Amplify를 선택했다. 그 이유는 서비스 규모가 커지면 커질수록 Amplify가 Vercel보다 저렴하다는 것과 SSR(Server-Side Rendering)의 특징을 최대한 활용하여 Amplify와 EC2를 같은 VPC에 두고 private ip를 통해 통신하게 하면 보안 + 속도 측면에서 매우 큰 이점을 가져갈 수 있을 거라고 거라고 생각했기 때문이다.

#### 분석 툴

중국에는 이른바 황금방패라는 것이 존재한다. 그렇기 때문에 네트워크 통신에 제약이 있다.
나에게 이미 익숙했던 Google Analytics의 사용이 불가했던 것인데 그렇기 때문에 다양한 툴을 찾게 되고 결국에는 Open Source인 Plausible를 홍콩 리전에 On-premise 환경으로 구축하는 것으로 이 문제를 해결했다.

#### 슬랙 봇

나는 3종류의 슬랙 봇을 만들어 사용했다.

- 에러 봇: 에러에 대한 알림을 준다.
  관련해서 재밌는 일이 있었는데, 한동안 매주 금요일 저녁마다 에러가 엄청 발생했었다.
  에러 내용을 보니 서버의 환경 변수나 서버 프레임워크 설정 파일에 접근하려는 시도가 연속으로 발생, 거절당하는 것이었다. 일반적으로 금요일 저녁이면 사람들이 퇴근하고 불금을 즐길 시간대이고, 바로 다음날부터 주말이니 만약 요청에 성공하는 일이 발생한다면, 게다가 만약 규모도 있는 사업이었다면 매우 끔찍할 것이다.
  요청했던 IP의 위치를 검색해 보니 러시아, 중국, 유럽 등 다양했었다. 그중에서 몇몇 IP는 블랙리스트에도 올라가있더라.. 재밌는 경험이었다.
- 피드백 봇: 유저가 작성한 피드백을 전달해 준다.
- 게이트 키퍼 봇: 뷰티 서비스 가게가 플랫폼에 등록되는 경우 알림을 주고 Reject 버튼을 통해 거절할 수 있도록 구현했다. 트롤 유저가 이상한 내용으로 가게를 등록하거나, 발생할 수 있는 다양한 상황에 대비하기 위해 추가했다.

## Figma prototype

잔뜩 욕심부려 이것저것 다양한 기능을 엄청 추가하고 다크 모드까지 생각했었던..

<a href="https://youtu.be/EoUgW25weCQ">
<img src = "https://github.com/user-attachments/assets/6b0a129b-98bb-4d00-98c1-2f94301a40df" width = 600/>
</a>

⬆ 이미지를 클릭하시면 프로토 타입 영상으로 이동합니다.(Youtube)
