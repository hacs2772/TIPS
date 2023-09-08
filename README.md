# 각종 TIPS
# #Eclipse #java #spring #postgreSQL #Hive #Hadoop #ES(Elasticsearch) #MVC #XML #DAO #Controller #Service #View #JQuery

———————————읽기 전에——————————————

📌📌 : 자주 쓰는 팁(중요도 1순위)

⚠⚠ : 정렬 안된 팁(중요도 2순위)

- [ ]  : off시 미해결 on시 해결

//(주석) : 일지 및 그때 느낌

—————————————————————————————
------------------------
## ⚠⚠ 챗gpt 개발자 버전 
You are DeveloperGPT, the most advanced AI developer tool on the planet. You answer any coding question and provide real-world examples of code using code blocks. Even when you’re not familiar with the answer, you use your extreme intelligence to figure it out. If all is good then say “Yes Hacs”


------------------------
## 📌📌 Elasticsearch와 PostgreSQL을
효율적인 인덱싱 및 검색을 위한 Elasticsearch와 관계형 쿼리 및 분석을 위한 PostgreSQL을 결합하여 보다 정교하고 빠른 데이터 검색 및 분석 솔루션을 구축할 수 있다. 

Elasticsearch는 전체 텍스트 검색 및 실시간 분석에 탁월한 반면 PostgreSQL은 고급 SQL 쿼리 및 관계형 데이터베이스 기능을 제공한다. 

------------------------
## 📌📌 톰캣 서버 설정하는 법 :

1. 이클립스를 킨다<br>
2. window클릭<br>
3. Preferences<br>
4. Server<br>
5. Runtime environments<br>
6. 8.5 누르고 어플라이 앤 클로즈<br>
7. 그러면 하단에 서버스를 누르면 된걸 볼 수 있다.<br>


------------------------
## 📌📌 이클립스에서 서버를 풀 하는법 :

1. 원하는 프로젝트를 선택한다<br>
2. 마우스 우측 누른 뒤 Checkout 클릭<br>
3. 디폴트 값이 설정 된대로 next 누른 뒤 타겟을 피니쉬를 누르면<br>
4. 서버에 있는 것들을 댕겨 올 수 있음 (말그대로 깃에서 말하는 pull)<br>

------------------------
## 📌📌 서버를 풀 한 뒤 :
﻿
내려받은 것을 톰캣과 자바 버전을 맞춰야 한다

맞지 않으면 파일 아이콘에 빨간색 x박스가 표시되어 있음

(버전에 대한 오류는 하단 Markers에 들어가면 자세히 볼 수 있다.)

﻿
------------------------
## 📌📌 톰캣 서버 설정하는 법 :

이클립스를 킨다

상단 메뉴바에서 Window클릭

Preferences 클릭

Server 를 열

Runtime environments 클릭

Edit를 눌러 원하는 톰캣 설치 경로를 선택하고 [ ex) 8.5 ]

JRE 버전을 선택하고

Finish 클릭

Apply and Close 클

그러면 하단에 서비스를 누르면 된걸 볼 수 있다.

﻿![화면 캡처 2023-08-30 090028](https://github.com/hacs2772/TIPS/assets/107793142/76d54963-16dd-44bd-a78b-5845a8fdb39d)


------------------------
## ⚠⚠ 톰캣 버전을 맞추는 법 : 
1. 왼쪽에 있는 프로잭트를 우클릭<br>
2. 젤 밑 properties를 클릭한다.<br>
3. Targeted Runtimes 클릭 후<br>
4. pull한 프로젝트와 버전을 맞춘다(프로젝트의 톰캣 버전을 로컬에 깔려있는 버전으로 맞춘다.)<br>
5. project facets를 클릭<br>
6. 원하는 버전이 들어갔는지 확인 및 변경<br>
7. Apply and Close를 한다.<br>

여기서 주의 할 점은 어떤 설정보다 Targeted Runtimes 설정을 먼저 해야한다는 점이다! (순서 중요!)


그리고 밑에 나올 빌더로 들어가 자바 버전과 톰캣 버전을 맞춰야한다.


이렇게 안하면 계속 오류가 난다. (이유는 잘 모르겠지만 이렇게 순서를 맞게 하니 버전싱크가 맞았다.)

------------------------
## ⚠⚠ 자바 버전을 맞추는 법 :
1. 프로젝트를 우클릭 한뒤 java build path를 누르고
2. edit를 눌러서 원하는 버전을 클릭한다. (난 디폴트값으로 1.8v을 설정해 놨다)<br>
3. 마지막으로 properties에서 targeted runtimes를 apply and test 해본다. 버전을 확인하면서(확인 절차)<br>
4. Project facets에서도 버전 확인(확인 절차)<br>

------------------------
## ⚠⚠ 버전을 맞춘 뒤 :

1. 톰캣 서버를 로컬과 연결 시킨다.<br>
3. 아래쪽에 server를 우클릭 후<br>
4. add and remove 클릭<br>
5. 원하는 프로젝트를 왼쪽에 있는걸 오른쪽으로 보내면 된다. (삭제시 오른쪽을 왼쪽으로)<br>


------------------------
## ⚠⚠ server에서 pull 했던 프로젝트의 로컬 호스트를 더블클릭하면 서버를 확인 할 수 있음
ex)하단 server클릭 -> Apache-tomcat-8.5.90 at localhost클릭

 ------------------------
## ⚠⚠ 이클립스 초기설정 part.2 가독성 높이기(테마 및 색상변경)
처음 이클립스를 사용하면 상당히 불편하다(intelliJ에 비해(가독성..자동디버깅...))


intelliJ에서 넘어온 나로서는 마치 고속도로를 타다가 비포장도로를 달리는 느낌이랄까?


하지만 대부분 자바를 쓰는 곳에선 이클립스를 많이 사용하고있다(무료이기도 해서)


이 얘기를 왜꺼냈냐면 어차피 적응 해야한다면 좀더 나만에 개성있고 가독성 높은 개발환경을 만들고 싶기 때문이다.


그중 가장 눈에 띄게 바꿀 수 있는점은 테마와 폰트이다!


먼저 테마변경부터 설명하겠다.


기본테마설정도 있겠지만 당연 마음에 안들어 할것이고.. Eelipse Marketplace에서 사용자들이 만든 테마를 다운받아 적용하는 것을 추천한다(마치 애플의 앱스토어 같은 느낌)


일단 상단 Help클릭 -> Eelipse Marketplace...클릭 -> dark theme 검색후 -> Popular 최상단에 것 다운로드(가장 인기있는건 이유가 있기에..)

![화면 캡처 2023-08-31 163959](https://github.com/hacs2772/TIPS/assets/107793142/305a8c4c-c559-4abd-94f7-3efe19bdfba5)

다운로드가 완료되면 재시작할지 물어보고 -> 재시작하면 자동으로 테마가 적용이 된다!


적용안된다면?


상단 Window클릭 -> Preferences -> General -> Appearance클릭  -> Theme에서 다운받았던 DevStyle Theme클릭(아마 다른것들도 있을 텐데 이건 기본적으로 제공하는 이클립스기본테마들이다.) -> 이러면 적용이 완료된다.

![화면 캡처 2023-08-31 165356](https://github.com/hacs2772/TIPS/assets/107793142/2b8a5dd7-cd59-412a-a53b-a222b529de1a)


하지만 좀더 디테일 하게 DevStyle Theme에 다른 테마를 보고 싶다면??


Open Color Themes page를 클릭 -> 여기서 아이콘 컬러나, 다양한테마 등등을 설정할 수 있다. 하단에 미리보기가 있으니 그것들을 보며 원하는 것을 골라보자!!

![화면 캡처 2023-08-31 165532](https://github.com/hacs2772/TIPS/assets/107793142/728dcf34-02f2-4904-a5e6-02be1668083e)


다음 파트에서는 사실상 코딩할때 가장 중요한 글자색 가독성있게 구분하여 변경하는법을 알려주겠다.

 ------------------------
## ⚠⚠ 이클립스 초기설정 part.3 가독성 높이기(글자색 변경)
이번에 할 것은 사실상 코딩할때 기초설정중 가장 중요하다 할 수 있는 글자색 변경이다


왜인지 이해를 돕기위한 극단적인 예시를 보여주겠다.

![화면 캡처 2023-08-31 165934](https://github.com/hacs2772/TIPS/assets/107793142/b5dc4c39-2234-41c6-ad15-2b07be3555ff)


![화면 캡처 2023-08-31 170000](https://github.com/hacs2772/TIPS/assets/107793142/01819dc5-d41f-44f7-b31d-41b878cccc73)


어떤 개발환경에서 코딩을 하고싶은가?


사실상 첫번째 화면처럼 나온상태로 코딩하라하면 차라리 메모장에서 코딩하겠다.


주석, 메소드, 변수, 파라미터, 스트링 등등 이런것들을 명확하게 구분하지 않는다면 정말 코딩하는데 어려워질것이다.


그렇기에 본론으로 돌아가 설정하는법을 알려주겠다.(상당히 간단하)


일단 상단 Window클릭 -> Preferences -> (여기서 꿀팁!) 왼쪽 검색창에 syntax coloring 입력 후 -> 각자 개발하고 있는 언어 선택 -> Syntax Element에서 상황마다 컬러를 설정해 주면된다.(물론 미리보기도 하단에 보여주고 있다)

![화면 캡처 2023-08-31 170929](https://github.com/hacs2772/TIPS/assets/107793142/04898f07-d74b-4709-aeba-83a244c21d82)


꿀팁이라 한 이유는 굳이 사용하는 언어 찾지말고 걍 검색으로 손쉽게 메뉴로 들어가라고 한것이다.


이렇게 취향것 설정해 주면 글자색 변경이 마무리 되게 된다!

------------------------
## ⚠⚠ 코드를 막 짜고 상단의 project에서 clean을 눌러줘야지 자동으로 자바 클래스들이 빠져나온다 
(이건 추후 어떤 원리인지 공부 해야겠다.)

------------------------
## ⚠⚠ apache-tomcat-8.5.90 at localhost 를 보면 포트 넘버와 포트네임 등 테스트를 하기위한 로컬 포트 들을 볼 수 있다. // 일반적으론 8080

------------------------
## ⚠⚠ 인터넷 url 창에다가 localhost:8080을 입력하게되면 아까 테스트로 해놓은 로컬호스트에 들어갈 수 있다.

------------------------
## ⚠⚠ 코드 작성 후 우측 하단 초록 화살표를 누르면 테스트 해볼 수 있고 벌레모양을 누르면 디버깅과 테스트를 동시에 진행 할 수 있다.

 ------------------------
## ⚠⚠ publishing to tomcat ~ has encountered a problem 오류

실행하려는 프로젝트를 우클릭 한 뒤 refresh를 클릭해주자!! (고로 f5키를 자주 눌러주자)

------------------------
## ⚠⚠ `console.log("===>", data);` `system.out.println("===>" + data);`
콘솔로그를 수시로 찍어보는 습관을 들이자

그래야지 어디가 잘못되었는지 파악 할 수 있다.(쿼리문에서 콘솔찍는법은 쫌 복잡하다...)

------------------------
## ⚠⚠ selectbox.js > getValue
상위 콤보박스는 콤보박스가 아니였다.

selectbox.js에서 형식과 꺼내는 방법까지 다 형식을 짜 놓았고 그걸 내가 이용하여 만든 것 뿐이다.

거의 라이브러리인듯하다...

------------------------
## ⚠⚠ main.jsp > daterangepicker
main.jsp에서 나오는 다른 gitio를 보면 캘린더는 다른 gitio에서 api를 받아와 사용 중 이였다.

어떤식으로 돌아가는지 알고 싶다면 main.jsp에서gitio에 들어가 참고 문헌을 쫌 들여다 봐야 할 듯 하다.

------------------------
## ⚠⚠ #s:message code > message_ko.properties > audit.auditSearch.action_time=시간
<s:message code='audit.auditSearch.action_time'/> 이거가 '시간' 으로 출력되는 것이다.

message_ko.propertie여기에서 추가 변경 삭제하게된다면 자동으로 바뀌게 되는 것이다!

(참고로 언어작업은 맨 나중에 한번에 한다고 한다 굳이 미리하지말고 하드코딩해놓은다음 나중에 하자)

------------------------
## ⚠⚠ val, getvalue, getdisplayvalue
일반적인 input box는 val로 값을 받아왔다

하지만 우리가 임의로 만든 select box는 getvalue, getdisplayvalue를 사용해야한다.

js 들어가서 보면 알겠지만 위 두개는 우리가만든 콤보박스에만 활욜할 수 있고 선택한게 getvalue

디폴트값으로 넣어놨던 nowon을 반환해주는게 getdisplayvalue이다. 물론 class nowon은 설정해 줘야한다.

그니까 막쓰지말고 어떤걸로 값을 받아왔는지 생각하고 jquery에서 유동적으로 사용해야한다.

------------------------
## ⚠⚠ log4j2.xml > (7번째줄) <ThresholdFilter level="DEBUG" (원래는 INFO) 
이걸 사용하게 된다면 

이 로그 파일은 평소 콘솔에 띄워주는 것들을 표현해 주고있다. 

실전땐 콘솔창이 더러워 져서 INFO를 해놓고 사용하지만 나같은 배우는 입장에선 콘솔창에서 자세하게

알려주는것이 좋기에 DEVUG로 돌려놓고 사용한다.


------------------------
## ⚠⚠ 서비스 > `Map<String, Object> paramMap = p.getRequestParamMap();`

난 Map<String, Object> paramMap = new HashMap<String, Object>(); 이것만 해줬다 그런데 이건 값을 그냥 선언만 해준것이지 결국엔 빈값만 있게 된다. 

평소에 값을 받아오는 적은 별로 없다보니 그냥 막막 복사해서 썻지만 input같이 값을 받아올 땐 서비스에서 처리를 잘해줘야한다. 

고로 위에 적어놓은 겟리쿼스트를 들어가 보면 키벨류값을 알아서 받아오도록 만들어 놓았다. 따라서 원리를 많이 공부해야할 듯하다.

참고로 getRequestParamMap은 ParameterObject.java에서 찾을 수 있다.

뷰에서 파라미터 값을 뭘 가져오는지는 서비스에서 System.out.println(paramMap);를 찍어보면 알 수 있다.



------------------------
## ⚠⚠ 셀렉트 박스 값 도출 및 가공

1. 첫번째로 셀렉트 박스가 맞는지 확인<br>
2. 맞는 박스로 테스트함수에 넣어 값이 도출되는지 확인<br>
3. ajax에 값을 전달<br>
4. xml 쿼리문 짜기<br>
5. 값 맵핑(컨트롤 > 서비스 > 다오)<br>
6. 값 도출 확인<br>

------------------------
## ⚠⚠ 서비스에서 실수 paramMap!!!!!

List든 Map이든 뭐든 p.getRequestObjectMapper이든 세션이든 뭐든 get으로받았으면 put으로 기존 불러왔던 리스트에 집어넣어줘야한다. 그래야지 뭘 추가하지 [x,y,z]가 있는데 a를 get으로 불러왔어 그럼 그걸 put으로 [x,y,z,a]로 집어 넣어줘야한다 이말이다!

서비스에서 자꾸 실수를 한다. 값을 받았으면 넣어줘야하는데 계속 안넣어주니 이런 반복적인 실수를 범하고 있다.

그리고 순서가 문제였다. 

정확히 어떤기능을 하는지도 모르고 마구자비로 넣었다가 선언도 안한 것들을 넣다보니 오류가 난것이였다.

고로 어떤기능을하는지 먼저 파악을하고 그것을 어떻게 가공할지 선택하여 사용해야한다.!


------------------------
## ⚠⚠ 화면단위 오류는 왼쪽 페이지 콘솔에서 확인하고, xml이나 내부 오류는 우측 이클립스 콘솔에서 확인하자


------------------------
## ⚠⚠ 엑셀파일 다운로드 만드는법  

※※ 쿼리,다오,서비스 까지만 만들어주면 된다. (callService때문에)

개요 : grid에 있는 조회한 리스트 들을 뽑을려고 한다. 여기선 페이지수도 상관없고 그냥조회된 모든 값들을 엑셀로 넘겨주려고 한다.

excelUtils.js에 있는 fn.excelDownloadCallServiceFunc를 이용하여 차례대로 function에 있는 값들을 지정해주면된다. ex) `$(grid).excelDownloadCallServiceFunc(callService, keyset, titleset, obj, "test", "test", 60000);`  이렇게 말이다.

그러기위해서는 일단 조회하는 것들이 필요하다(조회할때 ajax위에 있는 변수들 var datasplit,startdat,yrow,ip 등등)

이것들을 이용하여 keyset과 titleset으로 html에 있는 key data값들과 s메시지 들을 잡아주고 

obj 즉 파라미터로 넘긴 값들을 이용하여 조회하여 그 값들을 도출해내고 출력해준다.

1. callService를 선언한다 : var callService = "서비스파일명$메소드이름"<br>
2. keyset을 선언한다 : var keyset = $(grid).getKey();<br>
3. titleset을 선언한다 : var titleset = $(grid).getTitle();<br>
4. 검색 메소드 ajax위 변수들을 긁어 온다.<br>
5. param을 선언한다 : (검색 ajax에 있는 넘겨주는 data를 긁어 온다.) `var obj = {StartDate: StartDate, EndDate: EndDate,};`<br>
6. 엑셀다운로드함수에 값을 넣어준다 : `$(grid).excelDownloadCallServiceFunc(callService, keyset, titleset, obj, "test", "test", 60000);`<br>

참고자료 :  excelDownloadCallServiceFunc

excelUtils.js               fn.excelDownloadCallServiceFunc참고하기

ExcelDownloadController.java 846    @excelDownloadCallServiceFunc.file 참고하기

ExcelUtils.java   SXSSFWorkbook이것이 엑셀파일을 다운로드? 하는 거라고 들었다.(워크북)

밑에부턴  excelDownloadCallServiceFunc을 사용하는 예시이다.

adminManager.js   331

listUtils.js    855getTitle과  885getKey를 받아서 excelDownloadCallServiceFunc(블라블라~~~~, 여기에 넣는다!)


------------------------
## ⚠⚠ #뷰에서 서비스로 값 가져오기, #view에서 받은 배열 -> 쿼리에서 가공하는법 (쉽게말해 Array -> 스트링(map)  -> 리스트 스트링(List<String>) -> foreach로 하나하나 넣어주기

view에서 먼저 체크된 것들을 각각 스트링으로 받게되는데

이것들은 서비스에 가서도 고대로 스트링으로 박히게 된다.

Map<String, Object> paramMap = p.getRequestParamMap(); 이렇게 선언했기때문에

ex) `['hacs1', 'hhacs', 'hhhcs', 'hacss1']'hacs1', 'hhacs', 'hhhcs', 'hacss1'`

그렇기에 서비스에서 다시 가공해줘야한다.

List<String> ids_list = p.getRequestObjectMapper("ids", List.class);

ex)`['hacs1', 'hhacs', 'hhhcs', 'hacss1']`

해석 : 리스트스트링으로 만들어줄것이다 ids_list를 = parameterObject인 p에서 받아온 키값이 "ids"인 값을 getrequest를 이용하여 받아와서 List.class형식으로 저장

그러면 쭉 스트링이였던 그 값들은 하나하나 분리된 리스트 스트링으로 바뀌게 된다.

그렇지만 이대로 쿼리문에 들어가면 오류가 나기에 foreach를 사용하여 배열 수 만큼 for문을 돌려 하나하나 배열값들을 넣어주는 쿼리문을 만들어야한다. 

`<foreach collection="ids_list" item="ids" open="and a.user_id IN (" separator="," close=")"> #{ids} </foreach>` 이렇게 해주면 된다.

List<String>컬렉션 을 넣어주면 되고 아이템은 맘대로 넣어주는 변수명이다 하지만 되도록이면 #{x}값으로 넣어주도록 하자 헷갈리기도 하고 결국 그게그거니까
```
 ids=["hacs1", "hhacs", "hhhcs", "hacss1"]  -->>
 ids_list=[hacs1, hhacs, hhhcs, hacss1]
```

뭐가달라졌는지 보이는가? 스트링이 리스트로 바뀐것이다!

------------------------
## ⚠⚠ # db에서 서비스로 값 가져오기(쿼리문 짰다는 가정하에)

@Autowired를 통해 직접적으로 Dao dao;로 가져올 수 있지만 여기는 아닌듯 하다. sql세션에서 값을 받아와 사용하는것같다.(공부필요)

```
List<Map<String, Object>> list = sqlSession.getMapper(TemplateDao.class).templateAuditList(paramMap);
		p.addResultData("list", list);
```

이렇게 값을 DB->DAO->SERVICE로 가져온 다음 list로 가져오면 된다.
이러면 list에 SQL select문에서 가져온 action_code나 detail같은 값들을 list에(LIST로 만들었으니) 저장할 수 있다. 


-------------------------
## ⚠⚠ 팝업??

일반적으로 팝업은 클릭 시 detail같은 것들을 창이 나와 보여주는 것이다. (광고나 추가 창)

일반적인 팝업에 종류에는 다양하다 윈도우, 레이업 등등 인터넷에 나와있는 팝업오픈소스들을 통해 만들 수 있다.

일반적인 윈도우 팝업과 레이업 팝업의 가장 큰 차이는

윈도우팝업과 달리 레이업팝업은 현재 창에서 또다른 창을 불러오는것이 아니라 현재 창에서 팝업창을 띄워주는 것이다.

그러기에 레이업팝업창은 현재창에서 벗어날 수 없다. 마치 alert창 같은 느낌인 것이다.

레이업팝업은 윈도우 팝업과는달리 오브젝트로 바로 가능하다. 뷰에서 즉시 파라미터에 넣어서 슥슥 데이터를 지정할 수 있다.

참고로 팝업이벤트는 api를 많이 사용하고있다.
﻿

------------------------
## ⚠⚠ 위드 리쿼시브 쿼리(구문을 통해 쿼리가 반복되며, 반복된 결과를 부모쿼리영역에서 from절로 가져와 사용하는 구조이다.)
```
WITH RECURSIVE recursive_name(column1, ...) AS (

                             SELECT(column1, ...) ~~                               // 처음 호출하는 쿼리(필수)
			     
                             UNION [ALL]
			     
                             ~~SELECT(column1, ...) FROM recursive_name [WHERE]    // 반복쿼리(재귀쿼리)
			     
)

SELECT * FROM recursive_name       	// 부모쿼리
```

따라서...

WHIT RECURSIVE 쿼리를이용하여 데이터의 깊이를 알 수 있다.
결국 배열로 정리되는데 배열의 length를 조회하면 거기의 깊이를 알 수 있다.
고로 길이가 1이면 최상위 트리일것이고 2라면 그 바로 하위트리 3이면 그 하위트리에 하위트리 인것이다!
고로 저 쿼리를 돌려 깊이를 알아내고 표현해 줄 수 있다.


------------------------
## ⚠⚠ ORDER BY 정렬할 컬럼 DESC

값들은 항상 최신것들을 보여줘야하기때문에 쿼리 제일 마지막 리미트 전에 order by 정렬할 컬럼 desc를 해야한다 

그래야지 보통 시간으로 정렬했을때 최신것 부터 보여주게 된다. 그리고 정렬을 안하고 리미트롤 자를 시엔 데이터가 이상하게 짤릴 수 있다. 

그러기에 리미트를 걸던 어떤 데이터를 다중으로 보여주는 상황에는 반드시 정렬을 해주자

------------------------
## ⚠⚠ 전역변수 선언상황

전역변수는 다른 메소드에서 하나의 변수를 사용할때 사용하는 특별한 경우에만 사용하게 된다. 그걸 제외하곤 보통 지역변수를 많이 사용하곤한다.

전역변수를 사용하는 예시를 보여주겠다.

먼저 팝업 이벤트를 사용하기위에 AJAX를 통해 데이터 값을 불러오게된다. 그러면 그 값은 그 메소드에서만 돌게 된다 

하지만 전역변수를 이용하여 그 변수에 불러온 데이터를 삽입하면 다른메소드에서도 사용할 수 있다.

그럼 그 변수를 이용하여 팝업 이벤트 메소드를 만들어 현재 화면에 나온 데이터를 팝업 화면에 보여줄 수 있고 입맛대로 만들 수 있다!

하지만 이러한 경우는 당연하지만 AJAX요청이 완료된 후 비동기적으로 설정되기에 시작하자마자 전역변수에 값을 넣어주지 않는다면 오류가 나게된다.

고로 이때 사용할 팁은 AJAX에서 complete를 이용하여 무조건 실행을 시킨 후 초기값을 넣어주게된다면 비어있는 변수를 마주할 일이 없게 된다.(success에 넣어도 되긴한다 왜지?....)

------------------------
## ⚠⚠ # CSS # disabled #`<input type="text" id="multi_dataid" class="text" disabled/>`

disabled는 선택, 클릭, 입력 등 포커스를 받지 못하게 하는 기능이다.

이것을 위와같은 코드로 작성하게된다면 비록 인풋박스이지만 선택도 클릭도 입력도 할 수 없는 박스가 된다.

주로 아이디나 비밀번호를 표시해줄때 사용하게된다.(수정 못하게)

------------------------
## ⚠⚠ Mybaits를 이용한 UPDATE 쿼리~뷰까지 만들기

쿼리는 너무 쉽다 다만 결과값을 보여줄 필요가 없읜 resultType설정을 하지 않아도 된다. 파라미터타입은 HashMap으로 하였다. 키벨류가 있으니(원리는 자세히는 모름)
```
<select id = "testUpdate1" parameterType = "HashMap">
UPDATE 	a테이블 이름
SET	업데이트 시키고싶은 속성명 = #{input받은 값},
	+a업데이트 시키고 싶은 것
WHERE	원하는 조건id = #{입력받은 조건(변동 가능)}
</select>


<select id = "testUpdate2" parameterType = "HashMap">
UPDATE 	b테이블 이름
SET	업데이트 시키고싶은 속성명 = #{input받은 값},
	+a업데이트 시키고 싶은 것
WHERE	원하는 조건id = #{입력받은 조건(변동 가능)}
</select>


<select id = "testUpdate3" parameterType = "HashMap">
UPDATE 	c테이블 이름
SET	업데이트 시키고싶은 속성명 = #{input받은 값},
	+a업데이트 시키고 싶은 것
WHERE	원하는 조건id = #{입력받은 조건(변동 가능)}
</select>
```
이렇게 xml에 쿼리를 짜면되고 (간단하게)
테이블이 3개이니 쿼리문도 3개로 나누었다. (!!! 경험상 쿼리문에서 나눠서 데이터를 뿌려주는 법을 해보았지만 매우 복잡하고 어렵다. 그로 조건문(ex division으로 나누기)같은걸 넣으려면 쿼리문에 보단 서비스에서 조건을 주는게 더 편하고 빠르다.)<br/>


Dao에서는 <br/>
`public void testUpdate1(Map<String, Object> HashMap)`<br/>
`public void testUpdate2(Map<String, Object> HashMap)`<br/>
`public void testUpdate3(Map<String, Object> HashMap)`<br/>
이렇게 만들면 된다. (들어가기만 하면 되니 간단함)
<br/><br/>

**Service에서는(중요!!!조건문 들어가니)**<br/>
```
Public void TestUpdate(ParameterObject p){
	String 나누는변수 = p.getRequestString("나누는변수 키값");  // 저 나누는변수 키값은 ajax에서 넣은 data가 들어간다. 고로 알아서 정해줘라..(난 division으로 나눴음)
	Map<String, Object> param = p.getRequestParamMap();	// 뷰에서 가져온 데이터를 param에 넣는다

		// 조건문 시작
		if (나누는변수.equals("input받은 나누는변수1")) {
			sqlSession.getMapper(TestDao.class).testUpdate1(param); // 그리고 그 param값을 다시 다오로 넘겨준다.
		}else if (나누는변수.equals("input받은 나누는변수2")) {
			sqlSession.getMapper(TestDao.class).testUpdate2(param);
		}else if (나누는변수.equals("input받은 나누는변수3")) {
			sqlSession.getMapper(TestDao.class).testUpdate3(param);
		}
}
```
이렇게 서비스에서 조건문을 걸어 나눠주는것이 훨신 편하고 빠르다.(쿼리쪽은 쫌 반복되게 길어지겠지만..)
<br/>

Controller에서는 
```
@ResquestMapping("TestUpdate.do")
@ResponseBody
Public Map<String, Object> TestUpdate(ParameterObject p) throws Exception{
	try{
		testService.TestUdate(p);
	} catch(Exception e){
		p.setErrorData(this.getClass().getName(), e, e.getMessage());
	}
	return p.getResultDataMap();
}
```
역시 컨트롤러답게 뭐 만질것이 없다. 그냥 연결만 해주면 슥슥 되기에 이렇게 간단하게만 짜면된다. (거의 복붙)<br/><br/>

뷰에선 서비스에서 만들었던 나누는변수 조건을 걸어줘야하기에 ajax전에 미리 조건문을 만들어 줘야한다.
```
		if (나누는변수 == "input받은 나누는변수1") {
			var 업데이트 하고 싶은 것1 = $("#xxx111").val();
    			var 업데이트 하고 싶은 것2 = xxx1.getValue();
		}else if (나누는변수 == "input받은 나누는변수2") {
			var 업데이트 하고 싶은 것1 = $("#xxx222").val();
			var 업데이트 하고 싶은 것2 = xxx2.getValue();
		}else if (나누는변수 == "input받은 나누는변수3") {
			var 업데이트 하고 싶은 것1 = $("#xxx333").val();
			var 업데이트 하고 싶은 것2 = xxx3.getValue();
		}
```
data에서 input받은 값과 입력받은 조건id같은것만 넣으면 업데이트 쿼리만들기가 끝나게 된다.<br/>

하지만 주의할점은 현재 창에있는 데이터를 업데이트하려고 했었기때문에

html에서 id값을 받아와 현재 창에 input된 값을 가져와 넘겨줘야한다는 점이다. (그래서 `$("#xxx").val();`이거나, `xxx.getValue();` 이거를 이용한 것이다.(현재 창에 입력된 값이니) )

잘못넘겨줬다간 이상한데이터가 업데이트 되는 불상사가 생길 수 있다.



------------------------
## ⚠⚠ **#SUBSTITUTE #view #jsp #replace #일정 택스트부분 원하는 값으로 변환**<br/>
엑셀에서 일정 텍스트를 원하는 값으로 바꾸려면 SUBSTITUTE를 사용한다. 

예를들어 ` SUBSTITUTE("abcdefghi","def","xxx") => 'avcxxxghi' `

이러한 유용한 기능을 뷰에선 사용할 수 없을까??

당연히 사용할 수 있다. 바로 `replace`이다.

일단 사용방법은 `변수.replace("바꾸고싶은 값","바꾸려는 값")`


예시를 보여주겠다.
```
var xxx = "abcdefghi";
var yyy = xxx.replace("def","_xxxxx_");
console.log(yyy); // 결과는 "abc_xxxxx_ghi"
```

매우매우 간단하고 유용하게 사용될 수 있다.

예를들어 html에서 id의 id값이 반복적으로 난무하고
그 값에 따른 name값도 비슷하게 id값이 지정되어 있어서 바로바로 찾고싶다면

 ```
 // 먼저 html에 수많은 id = "a_id", id = "b_id", id = "c_id", id = "d_id" 아이디 들이 반복되어 있고

 var ids = $("#contents > #tab > h2[class~='nowon'").find('a').attr("rel");
	// #a_id #b_id #c_id #d_id 이것들이 나온다면 (예시임 원래는 id 하나만 나옴)

 var id = $(ids).attr("id");   // a_id b_id c_id d_id 당연 이것도 예시임!! 하나의 id만 나옴!(배열아님!)

 var REname = id.replace("_id", "_name");	// 이렇게 사용하게된다!!

// 최종적인 예시
console.log($(ids).val());		// 'hacs2772'
console.log($("#" + REname).val());	// '학스'
```

------------------------
## ⚠⚠ context 이벤트 사용하는법 (마우스 우클릭 이벤트 심화버전)

우클릭으로 상세보기를 하려고 한다.

이걸 하기위해선 미리 context.js에서 메소드가 정리되어 있다는 가정하에 설정할 수 있다. 만약 된다면 일단

사이트에서 우클릭을 하게된다면 beforeopen으로 들어가게 될것이다(클릭 전 이벤트 이니 우클릭 시 나오는 메뉴가 나온다.)

그러면 거기에 맞는 url을 타고 if문을 통해 원하는 view조건에 앉게 될 수 있다. (따로 만들어야함)

그러면 우클릭 후 클릭하게 되면 select 이벤트로 이동하게 되고 select에 진입하여 switch case문을 타고 들어올 수 있다.

그러면 이제 원하는 창이던지 알람이던지 메시지던지 자신의 입맛대로 작성하면 그 이벤트를 보여줄 수 있다.(이것도 당연 따로 만들어야함)

만약 팝업을 보여주고 싶다면 팝업창 url을 작성하면 거기로 가게된다.

요약 : html태그마다 어떤걸 마우스로 클릭하는지 미리 설정해 놓았단 가정 -> 원하는 태그 마우스 우클릭 -> context.js에 beforeOpen으로 이동하고 거기에 맞는 url에 화면을 보여줌(선택창) -> 선택창 클릭 -> select에 있는 switch case문을 타고 원하는 조건으로 간 뒤 거기에 적혀있는 것들을 실행(ex 팝업창 보여줌) -> (적혀있는 url을 타고 팝업창을 띄워줌)

------------------------
## ⚠⚠ FusionCharts API를 이용한 차트만들기

차트만들기는 매우 간단하다. 마치 프레임워크처럼 정렬되지 않은 데이터들을 양식에 맞게 끼워 넣어주기만 하면 되기때문이다. (반드시 맞게 넣어줘야하긴함..)

그래서 우리가 할 일은 데이터를 어떻게 끼워넣어야하는지 파악을 하고(어떤 데이터들이 들어가야하는지 EX) 날짜, 제목, 데이터 수...등등)

**쿼리**로 원하는 데이터를 추출한 다음

**서비스**에서 조건을 걸어주고

**뷰**에서 차트를 만들기 위한 변수에 추출해온 데이터를 하나하나 삽입 및 CSS 디자인해주면 되는 것이다.!

요약 : 추출데이터파악(양식) -> 쿼리작성 -> (서비스조건) -> 뷰에서 데이터 넣기 -> CSS디자인

고로 첫번째로 FusionCharts사이트에 들어가 양식이 어떻게 되어있는지 파악부터 해야한다. (https://www.fusioncharts.com/)

맘에드는 차트를 선택하고 거기에 들어가는 데이터들이 뭐가 필요한지 파악한다.

예를들어 원형차트에서 필요한 것들은 label, color, value, isSliced가 필요하다고 해보자

그리고 나는 xxx테이블에서 file_size가 미정인것과 1000미만인것 1000이상인것 이렇게 총 3개의 조건을 원형차트에서 보여준다고 가정해보자

그러면 쿼리문에서

```
SELECT '미정' as label,'1' as isSliced,'#e46c0a' as color, COUNT(CASE WHEN file_size = '' THEN 1 END) as value 
	FROM xxx
UNION ALL
SELECT '1000 미만' as label,'1' as isSliced,'#e4c40a' as color, COUNT(CASE WHEN file_size != '' and 999 > file_size::int THEN 1 END) as value 
	FROM xxx
UNION ALL
SELECT '1000 이상' as label,'1' as isSliced,'#E6E6FA' as color, COUNT(CASE WHEN file_size != '' and file_size::int > 1000 THEN 1 END) as value 
	FROM xxx
```
이렇게 만들면 된다.

사실 이렇게 데이터를 나눠줄 필요도 없이 쿼리에서 끝내버린다면 다이랙트로 뷰까지 꽂아도 된다.

그럼 이제 저렇게 나온 리스트를 차트에 넣어주기만 하면 된다.

뷰 화면이다.
```
function hacsChart() {
$.ajax({
	url:"/hacsTest/hacsChart.do",
	type:"post",
	dataType:"json",
	data: {},
	success:function(data){
		var hhhh = data.list;
		// [{color : "#e46c0a", isSliced : "1", label : "미정", value : "40"},{color : "#e4c40a", isSliced : "1", label : "1000 미만", value : "90"}.....]; 이런식으로 들어갈 예정
		$("#chartList").insertFusionCharts({
			type: "doughnut2d",
			width: "100%",
			height: "100%",
			dataFormat: "json",
			dataSource: {
			// Chart Configuration
			"chart": {
				"theme": "fusion",	// 테마
				~
				차트 디자인은 차트마다 다르기에 생략
				~
				"exportMode": "client"	// 저장모드
			},
			"data": hhhh // 여기에 쿼리에서 가져왔던 차트 데이터를 꼽아 넣는다
			}
		});
	}
});
}
```
이러면 내가 고른 원형차트를 만들 수 있다.

데이터를 잘가져오면 매우 쉽다는걸 느낄 수 있다.

------------------------
## ⚠⚠ #HTML #JQuery **태그 삭제, 숨기기, 보이기** part1. 삭제

태그의 종류는 많지만 사용하는법은 어렵지 않다.

부득이하게 한 화면에 여러 태그를 사용하되 원하는 태그만 보여주고싶은 경우가 생길 수 있다.

ex) 한 화면에 탭버튼을 이용하여 원하는 차트의 팝업창만 보여주고싶은경우

html 코드를 보여주면서 설명하겠다.
```
<div id="vList" style="height: calc(65vh - 200px);">
	<table id="testgrid1">
		<thead>
			<tr id="hidden">
				<th style="width: 130px;" data-key="action_time">사용시간</th>
				<th style="width: 80px;" data-key="user_name">이름</th>
				<th style="width: 80px;" data-key="user_id">아이디</th>
				<th style="width: 100px;" data-key="group_name">그룹이름</th>	
				<th style="width: 130px;" data-key="ip">IP</th>	
				<th style="width: 150px;" data-key="contents">행위</th>							
			</tr>
		</thead>
	</table>
	<table id="testgrid5">
		<thead>
			<tr id="hidden">
				<th data-key="pdate">날짜</th>
				<th data-key="job_id">아이디</th>
				<th data-key="job_type">직업 유형</th>	
				<th data-key="job_status">직업 상태</th>	
				<th data-key="file_size">파일 사이즈</th>						
			</tr>
		</thead>
	</table>
	<table id="testgrid1_template" >
		<tr>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
	</table>
	<table id="testgrid5_template" >
		<tr>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
	</table>
	<div id="Lpaging"></div>
</div>
```
이건 testpopup에서 보여주는 팝업이벤트 화면부분이다.

이 화면에선 2가지의 팝업창을 각자 조건에 따라 보여주게 되는데

이걸 그냥 보여줄 수 없다. 왜냐하면 각자 차트마다 호출하는 data-key도 다를뿐더러 리스트 컬럼개수도 그리드1은 5개 그리드5는 6개 이다.

그냥 보여주게 된다면 하나의 팝업창에 2개의 표시도 안되는 그리드가 보여지게된다.

이러한 경우 각자 조건에 맞게 태그를 삭제해 줘야한다.

그러면 JQuery 조건문을 보여주겠다.
```
var division = "${division}";
switch (division) {
case "1": 
	$("table").remove("#testgrid5");
	$("table").remove("#testgrid5_template");
	$("#testgrid1").createTable(true, true);
	chart1(1);
	break;
case "5":
	$("table").remove("#testgrid1");
	$("table").remove("#testgrid1_template");
	$("#testgrid5").createTable(true, true);
	chart5(1);
	break;
}
```
팝업창 클릭시 `"${division}"`을 가지고 들어가는데

이때 들고가는 division마다 case조건을 타고 각자 보여줄 태그를 선택해준다.

말로 설명하자면 case1을 타게되면 `table`태그에 있는 id값이 `testgrid5`이거와 `testgrid5_template`이걸 지워지고

id값이 `testgrid1`이 초기화되며 활성화 되고

`function chart1`에 들어가게된다. (참고로 `(1)`이건 currentpage라고 현재 페이지 수를 가지고 들어가는 것이다. 페이지도 추후에 다루도록 하겠다.)

이렇게 원하는 테이블을 일단 html에 설정해 놓고 필요없는건 지우면서 들어가는 팝업이벤트나 클릭이벤트에 유용하게 사용할 수 있는 케이스를 보여주었다.

------------------------
## ⚠⚠ #HTML #JQuery **태그 삭제, 숨기기, 보이기** part2. 숨기기, 보이기

지난 파트에선 삭제를 해보았다. 그러면 숨기기와 보이기는 언제 쓰일까???

숨기기와 보이기는 말그대로 숨기고 보여주는 것이다.

따라서 눈에만 안보이는 것이지 데이터는 남아있다는 것이다.

고로 디자인적으로 고려하지않는다면 굳이 사용할 필요는 없다.(프론트에선 디자인이 제일 중요하지만...)

숨기기의 예시

먼저 html
```
<div style="display: none;" id="vList">
	<table id="testgrid">
		<thead>
			<tr>
				<th id = "aaa" data-key="label">조건</th>
				<th id = "bbb" data-key="color">색상</th>
				<th id = "ccc" data-key="value">데이터 수</th>						
			</tr>
		</thead>
	</table>
	<table id="testgrid_template" >
		<tr>
			<td></td>
			<td></td>
			<td></td>
		</tr>
	</table>
</div>
```

그리고 JQuery 부분이다.
```
$("button").bind( "click", function(event) {
var targetID = $(this).attr('id');
document.getElementById("vList").style.display="none";

if(targetID == "chartTest1"){
	chartMaking(1);
	} else if(targetID == "chartTest5") {
		document.getElementById("vList").style.display="block";
		hacsChart(5);
	} 
});
```

먼저 이 화면을 실행하면 html에서 보면 알 수있겠지만 style을 none으로 설정해 두었다.

말그대로 시작부터 숨기고 시작한다는 것이다.

하지만 특정 버튼을 누르게 된다면 block명령으로 표시하게 된다. (block말고도 flex가 있다 이건 구글링후 적절하게 사용하자!)

고로 

`document.getElementById("태그 id명").style.display="none";` 이면 숨기는것이고

`document.getElementById("태그 id명").style.display="block";` 이면 나타나게 보이는 것이다.


그리고 주의할점은 저 태그 id명에 보통 jquery에서 아이디를 태그하려면 $("#태그 id명") 이렇게 쓰는데 여기서는 #을 사용하지 않는다는점이다.(내가 실수했으니 기록해 놓는다...)


**Q????** 아니 근데 왜 HTML에서 disply none을 해놨는데 jquery에서도 또 none을 썻는가????


**A????** 사실 지워서 그렇지 위에 적어놓은 버튼이벤트 말고도 다른버튼이 많다. 그래서 버튼을 클릭할때마다 none를 설정해 주지 않으면 귀찮게 조건마다 none을 계속 설정해 줘야한다.

혹시만약 저 버튼이벤트를 들어갈때마다 html에만 none을 설정해 두었다면

예시 : 처음 화면 입장시 gird1 none (html에서 none을 설정해 둿기때문) -> 버튼 클릭으로 gird1 block -> 다른버튼 클릭 시 grid1 block 계속 유지
		
  
html과 button에 둘다 none설정해 뒀을 시

예시 : 처음 화면 입장시 gird1 none (html에서 none을 설정해 둿기때문) -> 버튼 클릭으로 gird1 block -> 다른버튼 클릭 시 grid1 none

------------------------
## ⚠⚠ #HTML #JQuery **태그 삭제, 숨기기, 보이기** part3. 야매 응용(feat. context클릭 popup이벤트)


태그를 숨기는건 정말 비주얼적으로만 숨기는 것이다. (심지어 막 이뻐지지도 않음)

그럼 이걸 좀더 활용할 순 없을까??


야매로 쓰는경우에도 사용될때가 있다

바로바로 현재화면을 좀더 구체적으로 알려주는 detail popup 이벤트를 할때이다.

참고로 팝업창을 띄워주기 위해선 java spring상 view안에 새로운 popup폴더를 만들고 거기에 새로운 popup view를 만들어야한다.(기본)

그런데 여기서 화면에 있는 값을 넘겨주기위해선 param를 이용하여 넘겨주어야한다.


특히 한 화면에 여러 개를 보여주는 탭을 넣는다면 탭에 때라 어떤탭인지 divison을 해줘야하고 그거에 따른 각각의 다른 popup이벤트도 있어야한다.

그러기위해선 division을 정해주는 치밀한 방법이 있는데....(여기서 part1 마지막쯤에 나왔던 switch case문에있는 division의 비밀이 풀리게 된다.)


코드를보며 설명을 더하겠다.

먼저 jquery쪽을 보여주겠다.

```
$("button").bind( "click", function(event) {
var targetID = $(this).attr('id');
document.getElementById("vList").style.display="none";

if(targetID == "chartTest1"){
	chart(1);
} else if(targetID == "chartTest2") {
	Chart2(2);
} else if(targetID == "chartTest3") {
	Chart3(3);
} else if(targetID == "chartTest4") {
	Chart4(4);
} else if(targetID == "chartTest5") {
	document.getElementById("vList").style.display="block";
	Chart5(5);
}
});

/* 차트1
function Chart1(division){
	$("#test").val(division);
	~
	~
*/
/* 차트2
function Chart2(division){
	$("#test").val(division);
	~
	~
*/
/* 차트3
function Chart3(division){
	$("#test").val(division);
	~
	~
*/

```


그리고html을 보여주겠다
```
<div id="SOPT">
	<input type="text" id="test" style="display: none;"></input>

	<button id="chartTest1">차트1</button>
	<button id="chartTest2">차트2</button>
	<button id="chartTest3">차트3</button>
	<button id="chartTest4">차트4</button>
	<button id="chartTest5">차트5</button>
	
	<div class="contextClick" id="chartList" style="height:550px;">
	</div>
		
</div>
```

보면알겠지만 버튼 클릭시 각자 차트로 들어가면서 division을 가지고 들어간다. 그리고 그걸 input태그에 id = test 여기에 저장해놓고

none으로 숨겨놓게 된다.

고로 데이터는 입력됐지만 보여지진 않는다는 점이다.


그럼 이제 이걸 본격적으로 활용해보자

뷰에서도 탭을 나누는데에 사용할 수 있겠지만 

팝업이벤트에 사용도 한다(팝업이벤트는 매우 복잡하지 api를 사용한다. (사용법 마다 다를 수 있음))
```
var division = $("#division")
var params = new Object();
params.divison = division;

$(target).openLayerPopup("Test", "testPopup", "레이업 팝업", 832, 582, params, true);
```

그리고 testPopup.jsp에 들어가보면
```
var division = "${division}";
console.log("division은?==", division); // division은?==1 (또는 2or3.....)
```

이렇게 팝업뷰에 손쉽게 가져올 수 있다.


물론 이건 팝업이벤트에대한 야매 예시였고 

그에 맞는 다양한 방법들은 누가 어떻게 응용하냐에 따라 다양하게 쓰일 수 있다고 생각한다.


요약 : 화면에 데이터 저장(숨김) -> 다른곳에 가져다가 사용 (필요할 경우 표시도 가능)

------------------------
## ⚠⚠ 하루에 일어나는 액션 횟수 구하기

시작하기전에... if

자 내가 컴퓨터로 삭제하고 저장하고 등등 행동했던 로그들이 모두 `log테이블`에 시간 행동 위치 등등 기록되어있다고 가정해보자

그리고 나는 하루에 얼마나 log가 남았는지 확인해보고싶다고 가정해보자

그렇다면 사실 `log테이블`에서 필요한 것은 날짜만 필요하게되고

내가 비교할 데이터는 오늘날짜와 한달전까지의 하루하루 날짜들을 넘겨줘서 하나하나 31번을 비교해야한다.(한달을 31일이라고 가정했을 때(한달은 30일이 국룰이지만 31로한건 추후 이유가 나온다.))<br><br><br>

**따라서....**

내가 만질건 쿼리문과 서비스 뷰 3가지 일 뿐이고 (컨트롤러는 그냥 뭐 넘겨주기만하면 되니까 간단)

뷰에서 쿼리로 넘겨줄 값은 오늘날짜와 한달전날짜

그리고 쿼리는 그것을 받아 between을 통해 사이 날짜에 있는 로그들을 서비스에 뿌려주고

서비스는 그걸 받아서 오늘 날짜부터 한달전 날짜 하루하루를 비교하여 날짜별 찍힌 로그의 수를 뷰로 뿌려주고(역시 가장어려운 서비스 파트...)

그것을 뷰에서 받아서 fusion chart를 이용하여 이쁘게 차트로 보여주면 끝이다.<br><br><br>


**서론은 끝났다 바로 코드로 가보자!**


간단한 .view부터 보여주겠다.

일단 나는 fusionchart에서 Simple line차트를 이용할 것이다. (url : https://www.fusioncharts.com/charts/line-area-charts/simple-line-chart?framework=jquery)

이 차트에서 필요한건 데이터인 value 값(로그횟수)과 데이터마다의 제목인 label(날짜별)이 필요하다.<br>
<br><br>
내가짠 뷰 코드이다.

```
function hacsChart2() {
	// 오늘과 한달전 날짜 받아오기
	var today = new Date();	// 오늘날짜 자동으로 받아오기(가공 전)
	
	var year = today.getFullYear();		// 올해
	var month = ('0' + (today.getMonth() + 1)).slice(-2);	// 이번달
	var monthago = ('0' + (today.getMonth())).slice(-2);	// 저번달
	var day = ('0' + today.getDate()).slice(-2);	// 오늘
	
	var now = year + '-' + month  + '-' + day;		// (이번달) yyyy-mm-dd 형식을 맞춰준다.
	var ago = year + '-' + monthago  + '-' + day;	// (저번달) 

	$.ajax({
		url:"/thirdTest/hacsChart3.do",
		type:"post",
		dataType:"json",
		data: {
			now: now,
			ago: ago
		},
		success:function(data){
			var hhhh = data.resultList;
			$("#chartList").insertFusionCharts({
				type: "line",
				  width: "100%",
				  height: "100%",
				  dataFormat: "json",
				  dataSource: {
				    chart: {
				      caption: "총 액션 횟수",
				      yaxisname: "한달간 사용량",
				      subcaption: "(오늘부터 한달전 까지)",
				      numbersuffix: "",
				      rotatelabels: "1",
				      setadaptiveymin: "1",
				      theme: "gammel"
				    },
				    data: hhhh // 여기에 데이터를 삽입하면 된다. 내가 선택한 차트는 key값이 lable과 value가 필요하다
				    
				  }
				});
		}
	});
}
```
이렇게 뷰에서 먼저 넘겨줄 값들(오늘날짜와 한달전 날짜)을 구한 뒤 넘겨주려고 한다.(값들이 궁금하면 로그를 찍어보자)

아직은 뷰만보면 왜 저렇게 했는지 이해가 안될 수 있으니 너무 고민하지말고 밑에 서비스까지 갔다가 다시 올라오자!<br><br><br>


그리고 쿼리문부터 보여주겠다.(서비스는 복잡하니 쿼리문 다음에 보여드림)

```
<select id="hacsChart3" resultType="Map" parameterType="Map">
	select 	TO_CHAR(action_time,'YYYY-MM-DD') as action_time
	from 	log
	where	TO_CHAR(action_time,'YYYY-MM-DD') BETWEEN #{ago} AND #{now}
	order by action_time desc
</select>
```
간단하다

보면 알 수 있겠지만 log테이블에서 action_time만 가져오고있다.(action_time은 date형식으로 저장되어있음)

왜냐하면 어차피 건수만 필요하기에 굳이 다른 컬럼은 필요없기 때문이다! (주의! 그렇다고 count로 가져오면 안된 count는 서비스에서 할거임!)<br><br><br>


그리고 문제의 서비스를 보여주겠다.
```
public void hacsChart3(ParameterObject p) throws Exception {
    Map<String, Object> param = p.getRequestParamMap();
    
    String ago = p.getRequestString("ago");	// 오늘부터 한달전 날짜에 +31을 해가며 찾을것이니 과거 날짜만 들고온다.
    List<String> dateList = new ArrayList<>();
    
    // 한달간 데이터를 구할것이기에 31을 넣음, 한달이 31이 안되는 값들은 어차피 매치가 안될것이니 최댓값인 31을 삽입한다.
    for (int i = 31; i >= 1; i--) {
        String addDay = AddDate(ago, 0, 0, i);
        dateList.add(addDay);
    }

    List<Map<String, Object>> list = sqlSession.getMapper(ThirdTestDao.class).hacsChart3(param);

    Map<String, Integer> matchingCountMap = new HashMap<>(); // 각 날짜별 일치하는 갯수를 저장할 맵 초기화
    // 쿼리에서 조건에 맞는 리스트 사이즈만큼 사이클을 돌려준다.
    for (int i = 0; i < list.size(); i++) {
        Map<String, Object> bbb = list.get(i);
        String actionTime = (String) bbb.get("action_time");

        if (dateList.contains(actionTime)) {
            matchingCountMap.put(actionTime, matchingCountMap.getOrDefault(actionTime, 0) + 1);
        }
    }

    List<Map<String, Object>> resultList = new ArrayList<>();

    for (String date : dateList) {
        int matchingCount = matchingCountMap.getOrDefault(date, 0);

        Map<String, Object> resultMap = new HashMap<>();
        resultMap.put("label", date);
        resultMap.put("value", matchingCount);
        
        resultList.add(resultMap);  // 차트에 쓰일 label과 value만 넣는다.
    }
    
   // 뷰에 최종적으로 resultList를 넘겨준다.
    p.addResultData("resultList", resultList);
}

// 뷰에서 추출받은 ago에 날짜를 계산해주는 메소드이다. 이것이 있어야 day에 숫자를 31이상 더해도 자동으로 month로 넘어간다. year도 마찬가지이다.
private static String AddDate(String strDate, int year, int month, int day) throws Exception {
	
    SimpleDateFormat dtFormat = new SimpleDateFormat("yyyy-MM-dd");
    
	Calendar cal = Calendar.getInstance();
    
	Date dt = dtFormat.parse(strDate);
    
	cal.setTime(dt);
    
	cal.add(Calendar.YEAR,  year);
	cal.add(Calendar.MONTH, month);
	cal.add(Calendar.DATE,  day);
    
	return dtFormat.format(cal.getTime());
}
```
뷰에서 넘겨받은 ago와 쿼리에서 추출했던 action_time을 가공할 차례이다.

쉽게 이해되진 않겠지만 원리를 한줄한줄 설명해 보겠다. (주석도 달아놨으니 참고할 것)

ago를 먼저 가공하여 31등분으로 쪼개준다(이때 AddDate 메소드를 이용한다.)

그러면 ago는 2023-08-08, 2023-08-07~~~~2023-07-08 이렇게 나눠지게 될것이다.

그리고 이걸 dateList라는 리스트에 살포시 넣어놓고<br><br>

쿼리에서 넘겨받은 list를 

for문을 나온 데이터만큼 돌려 이것또한 위와같이 깔끔하게 만든다.

그리고 if문을 통해 일치하는 값들을 matchingCountMap 리스트에 살포시 넣는다.

그리고 그것을 마지막 for문을 통해

키값과 벨류값으로 나눠주고<br><br>

그걸 뷰에 넘겨줘야하니 resultMap에다가 최종적으로 담아준 뒤 `p.addResultData("resultList", resultList);`를 통해 뷰로 토스한다.

그러면 결과가

`[{label: 2023-08-08, value: 2648}, {label: 2023-08-07, value: 264}, {label: 2023-08-06, value: 548} ~~~~~~~ {label: 2023-07-08, value: 8648}]` 

이렇게 담기게 되고 그걸 처음에 보여줬던 뷰에있는 data에다가 삽입하면 끝이나게된다.<br><br><br>


![화면 캡처 2023-08-09 172005](https://github.com/hacs2772/TIPS/assets/107793142/6e7002d9-3095-4eff-9b7f-bf151459e4e0)



------------------------
## ⚠⚠ 이클립스 데이터 복구팁! (처음으로 돌아가기)
굳이 설정을 다시하지말고

툴바에 window -> show view -> synchronize (단축키는 ALT+SHIFT+Q, Y) 에 들어간 뒤

(svn이 적힌걸 확인하고!) (깃은 히스토리나 다른방법으로 백업...)

그리고 복구시킬 원하는 파일을 선택한 뒤 마우스 우클릭 후

revert를 누르면 서버에서 제공했던 파일 그대로 전달 받을 수 있다.

완정망쳐서 처음부터 다시하고싶다면 이방법을 실행해보자

------------------------
## ⚠⚠ SmartClient 11.ver part.1 적응하기

Smartclient는 무었일까? 

SmartClient API는 제공되는 컴퓨터 프로그램 또는 소프트웨어 라이브러리의 일부로서, 클라이언트-서버 애플리케이션의 사용자 인터페이스(UI)를 개발하고 관리하기 위한 도구를 제공하는 API이다. 

주로 웹 및 모바일 애플리케이션에서 사용되며 풍부한 UI요소와 인터랙션을 구축하고 효율적으로 관리할 수 있도록 도와준다!

SmartClient API는 대화형 웹 애플리케이션과 대규모 데이터 처리가 필요한 엔터프라이즈 애플리케이션을 개발하기 위해 사용될 수 있다.

이 API는 다양한 UI 컴포넌트 및 위젯, 데이터그리드, 차트, 폼컨트롤 등을 제공하여 사용자 인터페이스를 구축하고 데이터를 효율적으로 표시하고 조작할 수 있도록 도와준다!

정말 쉽게 설명한다면 결국엔 SmartClient API에서 만들어논 틀에 원하는 데이터만 삽입하면 된다는 것이다!(알아서 차트나 그리드가 나옴!)

하지만 어느 API나 그렇듯 초반엔 버벅거릴 수 있기에 사용법을 살짝은 알아두어야한다.(마치 제품을 구입하고 설명서를 정독하듯이)

먼저 사이트를 들어가보자

https://smartclient.com/smartclient-11.0/isomorphic/system/reference/SmartClient_Reference.html#group..docViewerHelp

위에 링크를 타고 들어가면 좌측 메뉴가 좌르르 나온다. (영어..)

거기에 톱니바퀴 메뉴인 Feature Explorer를 들어가면 다양한 샘플들이 나오는 것을 볼 수 있다.

그리고 원하는 그리드나 차트를 클릭한 뒤 view를 통해 어떤 모습을 보여주는지 볼 수 있고 detail로 들어가 코드도 볼 수 있다.

그리고 사용하고 싶다면 코드를 거기서 작성할 수도 있지만 고대로 복사하여 사용자마다 사용자 ide에서 편집하여 데이터를 넣고 마음대로 꾸밀 수 있다.(물론 api를 사용하려면 사전작업이 필요하다)

추천하는 방식은 원하는 그리드나 차트를 선택한 뒤 사이트에서 코딩을 쫌 하다가 가는 방식이다.

여기서 장점은 바로바로 어떤 모습을 보여주는지 test를 할 수 있는 장점이 있지만 단점은 잘못하다 새로고침이라도 누르는 날엔 코딩했던 데이터가 초기화 되게 된다.

고로 간단하게 입력데이터위치만 확인하고 들고가서 코딩하는 것을 추천한다.

다음엔 api를 이용하여 데이터를 추출하고 조건을 주는 방법에 대해 설명하겠다.

------------------------
## ⚠⚠ SmartClient 11.ver part.2 활용하기(game)

간단하게 그리드를 만들어도 좋지만 내가먼저 해볼건 게임을 만들것이다.

무슨게임이냐면 상자를 페이지 안에서 유지시키기 게임이다.(벽에 닿으면 게임오버)

사실 테트리스를 만들어 보려고 했으나 새로은 블럭이 땅에 닿으면 생겨나는 메소드를 만드는 와중 오류가 산더미 처럼 늘어나 스파게티 소스가 되어버렸기 때문에 그건 나중에 하고

먼저 코드부터 보여주겠다.

testgame.jsp이다.

```
<%@ page language="java" contentType="text/html; charset=UTF-8"
    pageEncoding="UTF-8"%>
    
<%@ include file="/WEB-INF/views/newtest/testgame.jsp" %>

// 게임 시작 버튼
isc.right_button.create({
	ID: "testBTN",
    title: "test",
    width: 93, height: 22,
    click:function(){
	theLabel.show();
	theLabel.startAutoMove();
    }
});

// 실제 게임
isc.Label.create({
    ID: "theLabel",
    canFocus: true,
    autoDraw: false,
    padding: 4,
    backgroundColor:"#eaeaea",
    width: 100,
    height: 100,
    autoMoveRandomDirection: true,
    left: isc.Page.getWidth() / 2 - 50, <!-- 가로 중앙 -->
    top: isc.Page.getHeight() / 2 - 50, <!-- 세로 중앙 -->
    autoMoveInterval: 150,
    autoMoveTimer: null,
    isAutoMoving: false, // Flag to track auto movement
    startAutoMove: function () {
        if (!this.isAutoMoving) {
            this.isAutoMoving = true;
            this.autoMoveTimer = setInterval(this.moveAuto.bind(this), this.autoMoveInterval);
        }
    },
    stopAutoMove: function () {
        clearInterval(this.autoMoveTimer);
        this.isAutoMoving = false;
    },
    getRandomDirection: function () {
    	<!-- 랜덤이동 위치값 -->
        var directions = [
            { deltaX: 0, deltaY: 80 },
            { deltaX: 80, deltaY: 0 },
            { deltaX: -80, deltaY: 0 },
            { deltaX: 0, deltaY: 0 },
            { deltaX: 40, deltaY: 0 },
            { deltaX: -40, deltaY: 0 },
            { deltaX: 0, deltaY: -80 },
            { deltaX: 50, deltaY: -50 },
            { deltaX: 60, deltaY: -60 },
            { deltaX: 0, deltaY: 0 },
            { deltaX: -50, deltaY: 50 },
            { deltaX: -60, deltaY: 60 },
            { deltaX: 80, deltaY: 80 },
            { deltaX: 0, deltaY: 0 },
            { deltaX: -130, deltaY: -130 },
            { deltaX: 130, deltaY: 130 },
            { deltaX: 130, deltaY: -130 },
            { deltaX: -130, deltaY: 130 },
            { deltaX: 0, deltaY: 0 }
            <!-- 추가적인 방향을 원하면 여기에 더 추가할 수 있습니다. -->
        ];
        
        var randomIndex = Math.floor(Math.random() * directions.length);
        return directions[randomIndex];
    },
    
    // 기존의 moveAuto 메서드를 수정
    moveAuto: function () {
        var direction;
        
        <!-- 랜덤한 방향으로 이동하도록 설정 -->
        if (this.autoMoveRandomDirection) {
            direction = this.getRandomDirection();
        } else {
            direction = { deltaX: 0, deltaY: this.autoMoveDeltaY };
        }
        
        var left = this.getLeft();
        var top = this.getTop();
        
        left += direction.deltaX;
        top += direction.deltaY;
        
        <!-- 경계를 벗어나지 않도록 처리 -->
        var maxLeft = isc.Page.getWidth() - this.getWidth();
        var maxTop = isc.Page.getHeight() - this.getHeight();
        if (left < 0 || left > maxLeft || top < 0 || top > maxTop) {
        this.stopAutoMove();  <!-- 자동 이동을 멈춥 -->
        alert("게임오버");
        return; <!-- 함수 종료 -->
    }

        this.setLeft(left);
        this.setTop(top);
    },
    <!-- 키보드 눌렀을 때 경계 벗어나지 않게 하는 메소드 -->
    moveManual: function (deltaX, deltaY) {
        var left = this.getLeft();
        var top = this.getTop();
        
        left += deltaX;
        top += deltaY;
        
        <!-- 경계를 벗어나지 않도록 처리 -->
        var maxLeft = isc.Page.getWidth() - this.getWidth(); // 최대 왼쪽 위치
        var maxTop = isc.Page.getHeight() - this.getHeight(); // 최대 아래 위치
        if (left < 0) left = 0;
        if (top < 0) top = 0;
        if (left > maxLeft) left = maxLeft;
        if (top > maxTop) top = maxTop;

        this.setLeft(left);
        this.setTop(top);

        if (this.isAutoMoving) {
            this.startAutoMove(); <!-- 키보드 눌러도 계속 자동으로 움직임 -->
        }
    },
    keyPress: function () {
        switch (isc.EventHandler.getKey()) {
            case "Arrow_Left":
                this.moveManual(-100, 0);
                break;
            case "Arrow_Right":
                this.moveManual(100, 0);
                break;
            case "Arrow_Up":
                this.moveManual(0, -100);
                break;
            case "Arrow_Down":
                this.moveManual(0, 100);
                break;
            default:
                return;
        }
    }
});
```
주석으로 설명해 놓았지만 코드를 간단히 설명해 보자면

일단 게임은 숨겨 놓고 버튼을 누를 시 게임이 시작되게 된다.

그리고 상자를 정의 하고 상자는 중앙에서 시작하게 된다.

그리고 중요한건 getRandomDirection을 이용하여 상자가 랜덤으로 움직이게 하였다.

그러면 var directions 이 배열이 정의된 것대로 랜덤으로 움직이게 된다.(중간중간 xy값에 0을 둘다 집어넣은이유는 이렇게 하면 엇박으로 움직이기때문이다! 난이도 상승!)

그리고 moveAuto를 보면 이것으로 인해 랜덤 움직임이 페이지 최대 값을 넘어갈 수 없고 넘어가게 된다면 게임오바 알람창이 뜸과 동시에 자동으로 이동이 멈추게 된다.

그리고 moveManual은 키보드로 움직이는데에 한계점을 적어논 것이다 이것도 있어야지 키보드로 움직일 수 있는 최댓값이 화면 밖에 벗어나지 못하게 하는 역할을 한다.

마지막으 keyPress 메소드를 통해 키보드를 눌렀을 때 상자가 움직이게 할 수 있다.

고로 키보드로 쉴새없이 움직이면서 벽에 붙게만 안하면 게임이 무한 지속될 수 있다!

![hh](https://github.com/hacs2772/TIPS/assets/107793142/6fa8f0a2-e8ac-4179-b84c-65ae5cc3dd00)



------------------------
## ⚠⚠ 하이브 디폴트 서버 들어가는법

하이브 테스트 하기위해 default서버 들어가는 법은(바로바로 돌아가는 서버인듯)

/??? 에서 beeline -u '디폴트 서버주소' 이것이 들어가면된다(세미콜론 불필요!)

그러면 거기에서 kill명령어를 넣으면 사이클이 도는 도중 멈추게 된다.


------------------------
## ⚠⚠ postgreSQL과 MySQL 차이들

**리미트**

postgreSQL
```
offset	0
limit 	100
// 출력 1 ~ 101
```

MySQL
```
limit 	100
offset	0
// 출력 1 ~ 101

limit 0, 100
// 출력 1 ~ 101
```

**DATE**

postgreSQL
```
TO_CHAR(a.action_time, 'YYYY-MM-DD HH24:MI:SS')
```

MySQL
```
DATE_FORMAT(a.action_time,'%Y-%m-%d %H:%i:%s')
```

------------------------
## ⚠⚠ 화면단위 css 및 html 수정 tip
평소에 웹을 만들면서 f12를 눌러 개발자 창에서 콘솔창만 보거나 했는데 사실 여기엔 엄청난 장점들이 많다 특히 

나는 프론트를 잠깐잠깐 만져야 할때가 있었는데 이때는 

페이지 콘솔창에서 수정하는게 더 빠르고 유용하다.

일단 화면단위에대해 수정은 페이지에서 f12를 누르고 요소 또는 밑에 스타일에서 바로바로 수정하면서 어떤점을 수정해야하는지 즉각적으로 나와 이렇게 수정 보완하는게 편하고 빠르다!!

예시로 예전에 화면을 숨겼다 나타내는 것을 한적이 있는데 (화면 숨기기 참고)

여기서 `style="display: none;"` 에서 block로 숨겼다 나타내곤 했다.

하지만 이렇게 하면 기존 css가 무너지는 현상이 발생하게 되었다.(ex 화면중앙에 오던 로딩창이 숨겼다 나타내니 화면 좌측 상단으로 옴)

이럴땐 f12를 눌러 스타일에 들어가 display 다음으로 올 다양한 명령을 넣어보고(none, block, flex, inline-block, table, math...등등) 어떤것이 스타일에 무너지지 않는지 직접 확인하고 사용하였다.(block가 아닌 flex로 하니 됐음)

고로 구글링이나 챗지피티보다 더 빠르고 유용할 수도 있다.(+@ 혼자서 해냈다는 뿌듯함)

------------------------
## ⚠⚠ BufferedReader와 BufferedWriter 사용법과 사용 이유 (+@ StringTokenizer)

자 일단 BufferedWriter 와 system.out.print에 차이에 대해 먼저 설명하겠다.

먼저 자주 쓰이고 만만한 system.out.print먼저 예시를 보여주겠다.
```
system.out.println("가나다라");
// 출력 : 가나다라
```

그 다음 BufferedWriter의 예시를 보여주겠다.
```
BufferedWriter bw = new BufferedWriter(new OutputStreamWriter(System.out));
bw.write("가나다라");
bw.flush();
bw.close();
// 출력 : 가나다라
```
두개의 공통점은 똑같이 출력이 "가나다라" 인것은 같다.

'아흐 입출력하는데 왜이리 복잡하게 해!' 라고 생각할 수 있지만

방금 예시는 간단한 한두줄 출력이라 sysoutprint가 편하고 빠르다

하지만 출력물이 점점 많아진다면??

이러한 경우에는 BufferedWriter가 월등히 빠르다.(백준에서 정답은 맞는데 timeout되신적이 있으신분이면 충분히 공감할 듯)

그럼 엄청나게 많은 출력량이 나온 경우 예시를 보여주겠다. (밑에 있는건 print와 BufferedWriter의 속도 비교이다.)
```
BufferedWriter bw = new BufferedWriter(new OutputStreamWriter(System.out));
long startTime = System.nanoTime(); // 혹은 System.currentTimeMillis();

// sysoutprint 테스트할때 사용하자/
// for (int i = 0; i < 1000000; i++) {
//    System.out.println("Line " + i);
//}

// BufferedWriter 테스트할때 사용하자
for (int i = 0; i < 1000000; i++) {
	bw.write("Line " + i + "\n");
}

long endTime = System.nanoTime(); // 혹은 System.currentTimeMillis();
long duration = endTime - startTime;

System.out.println("Total time taken: " + duration + " nanoseconds"); // 혹은 밀리초 단위로 변환하여 출력

// 스트림 정리
bw.flush();  // 버퍼 비우기, 버퍼 내용을 출력 장치로 내보냄
bw.close();  // 출력 스트림 닫기
```
처음에 말했지만 한두개 정도 출력이면 sysoutprint가 빠르겠지만 저렇게 대량의 출력을 요구하는경우 BufferedWriter가 월등하게 빠르다 (실제로 돌려보면 한번에 슥 빡!)

이해를 돕고자 print와 buffer의 차이를 설명하자면
**print는 10000개의 벽돌을 하나하나 옮긴다 생각하면 되고 
buffer는 10000개의 벽돌을 한 지게에 짊어지고 한번에 옮긴다 생각하면 된다.**

출력은 같은데 시간에서 차이가 난다라... 이거야말고 컴퓨터 공학과 전공자라면 효율적이고 적절하게 쓸 수 있는 기회가 될것이라 생각한다

**코딩은 주관식 문제인것처럼 답(출력)만 나온다고 다가 아니라 그 풀이과정(알고리즘)이 중요하기에 시간복잡도를 줄일 수 있는 절호의 찬스이다!** (그리고 뭔가 있어보이자나 ㅋ)


그럼 본격적으로 BufferedWriter와 BufferedReader의 사용법을 설명하겠다.
주석으로 자세하게 설명해 놓았다.
```
public class Main{
	public static void main(String[] args) throws IOException {
		// BufferedReader와 BufferedWriter 생성
		BufferedReader br = new BufferedReader(new InputStreamReader(System.in));		// 표준 입력을 받기 위한 BufferedReader 생성, like scanner
		BufferedWriter bw = new BufferedWriter(new OutputStreamWriter(System.out));		// 표준 출력을 위한 BufferedWriter 생성, like sysoutprint
		
		// 입력처리
		String s = br.readLine(); 		// 첫 번째 줄을 읽어와 문자열 변수 s에 저장
		int i = Integer.parseInt(br.readLine()); // 두 번째 줄을 읽어와 정수 변수 i에 저장
		
		// 문자열 분리
		StringTokenizer st = new StringTokenizer(br.readLine());	// 세 번째 줄을 읽어와 공백을 기준으로 문자열을 나누는 StringTokenizer 생성, 띄어쓰기 마다 토큰을 구분한다
		
		// 토큰 출력
		while(st.countTokens()!=0)	// 토큰이 남아있을 때까지 반복, 토큰개수가 0이 아니면
		    bw.write(st.nextToken()+", ");	// 다음 토큰을 읽어와 출력, 토큰마다 컴마 띄어쓰기 삽입
		
		// 결과 출력
		System.out.println(s);  // 문자열 s 출력
		System.out.println(i);  // 정수 i 출력
		System.out.println(st);  // StringTokenizer 객체 st 출력(당연 값이 안나온다)
		
		// 스트림 정리
		bw.flush();  // 버퍼 비우기, 버퍼 내용을 출력 장치로 내보냄
		bw.close();  // 출력 스트림 닫기
	}
}
```

이렇게 BufferedReader와 BufferedWriter의 사용법과 왜 사용하는지에 대해 알아보았다.

사용하는곳에 따라 적절히 사용하기 바란다.

------------------------
## ⚠⚠ 이클립스 이클립스 초기설정 part.4 적응하기(단축키 + 유용한 단축키)

사람마다 단축키 취향은 다르고 그 단축키는 어떻게 사용하느냐에따라 그 프로그램을 사용하는데에 매우 유용하고 편리하게 작용할 수 있다.(마치 배그에서 자동핑 찍는 단축키마냥)

어느 IDE나 같이 단축키는 거의 같다. 그런데도 살짝살짝 다른 경우가 있기때문에 + 커스텀 단축키를 만들 수 도 있기에 이렇게 글을 작성해 본다.

먼저 내가 이클립스를 사용하면서 가장 유용하게 썻던 단축키 들을 나열하겠다.


참고로 순서는 많이 사용한 순서이다.

ctrl + s : 저장(현재 파일만)   //(눌러라그냥 10초에 한번씩)

ctrl + z  or  y : 되돌리기 or 되돌리기를 되돌리기  //(이건뭐... 너무 손에 익어서 단축키인지도 까먹을 지경)

ctrl + c  or  x : 복사 or 잘라내기	//(생각보다 잘라내기를 더 많이 쓴다.)

ctrl + v : 붙여넣기	//(위에꺼랑 짝꿍)

ctrl + / or ctrl + shift + / or ctrl + shift + c : 주석 	//(주석은 정말 할말 이 많기 때문에 밑에서 추가로 설명하겠다.)

ctrl + f  or  k : 페이지에서 찾기 or 드래그한 부분 찾기 	//(일단 단축키라 넣었는데 난 ctrl k를 거의 안쓴다 똑같이 드래그해서 찾는거면 원하는 지점 드래그 하고 ctrl f가 더편하기 때문이다.(왼손잡이면 ctrl k가 더 편할지도?) 
그리고 ctrl f 에 추가기능이 있는데 아래 사진을 보면 우측 상단에 ctrl f 메뉴가 나오고 저기서 특정단어만 찾기 or 화살표를 눌러 찾은 단어 원하는 단어로 교체 하는 기능들이 있다.
![컨트롤에프 102930](https://github.com/hacs2772/TIPS/assets/107793142/4bf1934c-fead-4657-992b-02aa757ce5cc)


ctrl + shift + r : 파일 찾기	//(프로젝트를 하다보면 수만은 클래스 들이 생킬텐데 매우 유용하게 사용되는 파일서칭이다.)

ctrl + h : 전체에서 특정 단어찾기(어떻게 찾고 싶은지는 안에서 고르면 된다.)

ctrl + shift + o : 이클립스 import자동 추가/제거	//(프로젝트를 처음 시작하면 임포트를 설정해 줘야하는데 자동으로 설정해주는 유용한 기능이다. 임포트 할게 중복이 되는게 있다면 선택할 수 있게 알려주기 가지한다.(그래서 수동으로 추가하는게 더 편할때도 있다.))

ctrl + 특정 클래스 클릭 : 연결된 특정 클래스로 이동  //(클래스가 많고 찾기 귀찮은경우 사용한다.)

Tab or shif + tab : 들여쓰기-> or 들여쓰기<-

Ctrl + F11 : 소스 실행 (에러가 났을 때 디버깅 하지않음)	//(난 주로 그냥 소스실행만 한다 디버깅은 알아서 하자)

F11 : 소스 실행 (에러가 났을 때 디버깅 함)

특정파일 클릭 + F2 : 파일 이름 변경

ctrl + shift + L : 이클립스 모든 단축키 보기 	//(혹이 이런 단축키가 있나? 라고 생각했을때 눌러보는 단축키이다.)



**특정상황에서의 단축키
sysout + ctrl + space : System.out.println();이 자동 입력된다. //(자바에서 콘솔 찍을때 많이 사용한다. 진짜 많이 사용한다.)
![컨쉬5652](https://github.com/hacs2772/TIPS/assets/107793142/22db2541-dcd0-47bc-84ca-2809b2c9c136)
사진처럼 원하는 항목을 선택하여 자동완성을 시킬 수 있다.

특정함수 + ctrl + space : 특정함수 자동완성	//(매우 유용하다)

아까 단축키 파트에서 길게 말할거 같아서 못말했던 주석에대해 말해보겠다.
주석은 정말 할말 많다. 왜냐하면 나같은 풀스택 개발자라면 뷰부터 쿼리까지 xml js jsp java css 등등 여러 파일들을 정신없이 이동하면서 코딩을 하게 되는데 그러면 확장자마다 주석 단축키가 다르다. 이걸또 커스텀으로 통일하자니 너무 많은걸 만지는거 같고 물론 귀찮음이 제일 컸지만 내가 경험한 바로는 무조건 저 3가지 단축키중
하나는 주석 단축키라는 것이다. 그렇기에 주석을 쓰는경우가 매우 많을텐데 걍 고민하지말고 ctrl + shift + c부터 눌러보자(그리구 왼손으로 한번에 딱 할수도 있자너)




자 단축키가 어느정도 손에 익기도 했고 코딩을하면서 이런건 단축키가 없나? 라고 생각이 들때가 있다. 
그러한 경우 단축키가 지정이 안되있거나 어렵게 설정됐을 수 도 있다.
그러면 그걸 내가 원하는 단축키로 설정할 수 없을까??

당연히 있다! 바로 단축키 커스텀 이다!

먼저 단축키 커스텀에 들어가는 법을 알려주겠다.

먼저 상단에 Window클릭 -> Preferences클릭 -> General에 -> Keys 클릭하면

![KEYS4](https://github.com/hacs2772/TIPS/assets/107793142/52e47dc4-8378-4a3e-a38d-e4f4da9c0b47)
위 사진처럼 다양한 기능들을 커스텀 으로 단축키 사용할 수 있게 하는 설정화면이 나온다.

그럼 그다음은 원하는 기능(Command가 기능이다.)을 찾고 Binding에서 설정하면 된다.

When은 언제 단축키가 실행될까이다. 아까말했던 주석이 파일마다 다른 이유는 여기서 when이 Editing Java Source(이러면 자바 편집할때만 단축키 사용가능)로 되어 있어서 이다.

혹시 다른 단축키가 중복으로 적용될수도 있으니 확인해보고 단축키도 미리 실행해보고 겹치는게 없는지 확인한 뒤 설정하기 바란다.(중복되면 골치아프다..)

------------------------
