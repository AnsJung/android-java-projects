# 네이버 검색 앱
### 사용 언어
* 자바(Java)
### 사용한 API
* 네이버 오픈 API 검색
  * 책 검색
  * 영화 검색
  * 오타변환
### 특징
* Naver Open API 사용
* Retrofit 사용 - Custom Converter를 구현하여 XML과 Json을 하나의 컨버터로 데이터를 변환
* Object Animator 사용
* Animation을 사용하여 Dialog Animation 구현
* RecyclerView - Custom ItemDecoration 사용
* RecyClerView - ViewType - Header,Main,Footer 에 따른 ViewHolder 사용
* 아이템 클릭시 WebView 제공
* Dialog를 상속받는 Custom Dialog 구현
* SpannableStringBuilder를 사용하여 텍스트 처리

### 네이버 API 설정

`RequestSearch/local.properties`에 본인의 네이버 API 인증 값을 추가하고 Gradle을 동기화하세요. 기존 `sdk.dir` 설정은 그대로 두면 됩니다.

```properties
NAVER_CLIENT_ID=
NAVER_CLIENT_SECRET=
```

`local.properties`는 Git에서 제외됩니다. 인증 값은 빌드된 APK에 포함되므로 배포용 앱에서는 서버를 통해 네이버 API를 호출하세요.

