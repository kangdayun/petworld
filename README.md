Readme_20185280_강다윤

Android Studio Version 4.1
AVD : Pixel 2, API 30, Target Android 11.0(Google Play), Resolution 1080 x 1920: 420dpi

#java
FifthActivity(본인) : 동네별(지하철역) 친구목록 / text file을 이용한 listview & searchview 기능 구현
FourthActivity(일부분) : 사이즈별 친구목록 / Information class의 get method를 이용하여 adapter에 value들을 add함
Information(본인) : Firebase Realtime Database에서 받아온 reference를 하나씩 가져오기 위한 class
MainActivity(일부분) : 로그인 화면 / Context, IdStorage와 getIdStorage를 추가하여 MsgAdapter에서 현재 User ID 값을 가져올 수 있게 함.
MsgAdapter(공통) : SeventhActivity(나의 친구목록)을 위한 Adapter
SeventhActivity(본인) : 나의 친구목록 / 파이어베이스에 '프로젝트명'-'friend'-'User ID' 형식을 만들고, adapter를 이용하여 나의 친구목록에 친구의 프로필이 추가되도록 함.
SixthActivity(일부분) : Information class의 get method를 이용하여 adapter에 value들을 add함

#res/drawble
dog.jpg : MainActivity backgroud image
dog_friend_2.jpg : ThirdActivity background image
dogimage.jpg : users' profile image
petfoot.jpg : 꾸미기에 활용

#res/font
nanumsquare_aceb.ttf : 모든 textview에 font 적용

#res/layout
activity_fifth.xml(본인) : 지하철역 listview & searchview
activity_seventh.xml(본인) : 나의 친구목록 listview
activity_sixth.xml(본인) : 동네별 친구목록 listview
listview_msg.xml(본인) : 나의 친구목록 custom

#res/raw
subway.txt : 지하철 역 이름이 담긴 text file

#res/values
styles.xml : 어플 주요 색상 선정, 타이틀바 제거

---------------------------------------------------------------------------------------------
팀 이력 관리 (날짜별)

9/22~ 아이디어 회의(모두)
       
9/24 아이디어 선정 (김정엽)

9/25 시장조사 & 기능 초안 (모두)

11/2 Zoom 회의
      모프 개요 토의, blueprint 작성(김정엽)
11/6
- 전반적인 뼈대완성(로그인 페이지, 회원가입페이지) (노지민), (김정엽)
- 사진 회전현상 해결(김정엽)
- 회원가입 유효성검사 (노지민), (김정엽)
- Local DB에 저장 기능 구현 (노지민), (김정엽)

11/7
- Subway.csv -> text 파일로 바꾼 뒤 리스트뷰 생성 (강다윤)

11/12
대면 회의
- 어플 방향성 수정, 새로운 방향성 제시 (김정엽)
- 로그인 기능 구현(김정엽)
- firebase 리스트뷰를 이용(김정엽)
- firebase 연동 방법 연구 (모두)
- Station 리스트뷰에 메뉴 버튼에 지하철역 검색 기능 추가 구현 (강다윤)
Zoom 회의
- firebase에서 연동 기능 (노지민)

11/16
Zoom 회의
- 커스텀 리스트뷰 적용 방법 연구 (모두)
- firebase에서 데이터가져오기 (노지민)
- firebase에서 가져온 데이터 심플리스트에 추가하기 (노지민)
- 아이디 중복 기능 구현 (오류발생) 추후 삭제 (노지민)
- 로그인 기능 구현 (노지민),(김정엽)
- 아이디 중복 검사 기능 구현(김정엽)
- 아이디, 비밀번호 찾기 구현(김정엽)
- 기존 발견된 오류들 수정(김정엽)
- 저장한 데이터에서 id, pw, petname, size, kinds, station 따로 따로 가져오기 (강다윤)
- Information.java 파일 생성 (강다윤)
- FourthActivity 조금 수정 (강다윤)

11/17
- 이용약관, 개인정보 정책 팝업 완성(김정엽)
- 로그아웃 기능 구현(김정엽)
- 커스텀 리스트뷰 완성 (노지민)
- 선택별 회원정보 보기 기능 (노지민)
- 친구 추가기능 알고리즘 구현 (노지민)
- 친구 추가 기능 구현 (노지민)
- 친구목록 리스트 만들 때 체크박스 (강다윤) -> 데이터베이스 저장 문제로 다시 뺌
- 자신의 id 찾는 방법. 가져오는 방법 (강다윤)
Zoom 회의
- 처음에 user child 하위에 friend child 생성 -> 문제 발생 -> user child 와 동등한 위치에 생성되도록 수정(강다윤)
- 친구목록 Activity 생성(강다윤)

11/18
카카오톡 연락 (개인 역할 분담)
- 대표 색깔 선정, UI 디자인 통일, background 이미지, icon 이미지, Font 적용 (강다윤)
- 채팅기능 구현 및 디자인(노지민)
- 채팅방 레이아웃 수정(김정엽)
- 그 전까지의 디자인 오류 수정(김정엽)
- 채팅방 디자인 외 어플의 전체적인 디자인 틀 수정(모두)

11/19
Zoom 회의
 - 발바닥 아이콘 추가 (강다윤)
- 18일 UI 수정할 때 타이틀바 삭제 -> 문제 발생 -> 역 검색 메뉴 사라짐-> 검색 기능을 메뉴말고 바로 뷰에 보이도록 다시 구현 (강다윤)
- 액티비티 전환 간 오류 수정(김정엽)
- 채팅 시 자동 스크롤 기능 연구 (모두)
- 주석 정리 (모두)
- 어플 예외처리, 오류 잡기(로그아웃 기능) (모두)
- 최종오류체크 (모두)
