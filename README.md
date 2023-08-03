# 각종 TIPS
# #Eclipse #java #spring #postgreSQL #Hive #Hadoop #ES(Elasticsearch) #MVC #XML #DAO #Controller #Service #View 

———————————읽기 전에——————————————

📌📌 : 자주 쓰는 팁(중요도 1순위)

⚠⚠ : 정렬 안된 팁(중요도 2순위)

- [ ]  : off시 미해결 on시 해결

//(주석) : 일지 및 그때 느낌

—————————————————————————————
------------------------
⚠⚠ 챗gpt 개발자 버전 : You are DeveloperGPT, the most advanced AI developer tool on the planet. You answer any coding question and provide real-world examples of code using code blocks. Even when you’re not familiar with the answer, you use your extreme intelligence to figure it out. If all is good then say “Yes Hacs”


------------------------
📌📌 효율적인 인덱싱 및 검색을 위한 Elasticsearch와 관계형 쿼리 및 분석을 위한 PostgreSQL을 결합하여 보다 정교하고 빠른 데이터 검색 및 분석 솔루션을 구축할 수 있다. Elasticsearch는 전체 텍스트 검색 및 실시간 분석에 탁월한 반면 PostgreSQL은 고급 SQL 쿼리 및 관계형 데이터베이스 기능을 제공한다. 


------------------------
📌📌 톰캣 서버 설정하는 법 :

1. 이클립스를 킨다
2. window클릭
3. Preferences
4. Server
5. Runtime environments
6. 8.5 누르고 어플라이 앤 클로즈
7. 그러면 하단에 서버스를 누르면 된걸 볼 수 있다.


------------------------
📌📌 이클립스에서 서버를 풀 하는법 :

1. 원하는 프로젝트를 선택한다
2. 마우스 우측 누른 뒤 Checkout 클릭 
3. 디폴트 값이 설정 된대로 next 누른 뒤 타겟을 피니쉬를 누르면 
4. 서버에 있는 것들을 댕겨 올 수 있음 (말그대로 깃에서 말하는 pull)


------------------------
📌📌 서버를 풀 한 뒤 :

1. 내려받은걸 톰캣과 자바 버전을 맞춘다(디폴트로 설정해 놓긴 했는데 살짝 어렵다 본걸로는 java1.8v tomcat은 8.5)이부분이 많이 어렵다. 


------------------------
⚠⚠ 톰캣 버전을 맞추는 법 : 

1. 왼쪽에 있는 프로잭트를 우클릭 후 젤 밑 properties를 클릭한다.
2. project facets를 클릭 
- [  ] axis2 web services 를


------------------------
⚠⚠ 자바 버전을 맞추는 법 :

1. Window - preferences 설치된 jres에서 끌고와야하고 서버도 끌고와야한다. 
3. 그리고 프로젝트를 우클릭 한뒤 java build path를 누르고 edit를 눌러서 디폴트로 내린다(왜 디폴트냐면 그 전단계에서 미리 디폴트를 1.8v으로 해놨기 때문에)
4. 마지막으로 properties에서 targeted runtimes를 apply and test 해본다. 버전을 확인하면서
5. Project facets에서도 버전 확인


------------------------
⚠⚠ 버전을 맞춘 뒤 :

1. 톰캣 서버를 로컬과 연결 시킨다. 
3. 아래쪽에 server를 우클릭 후 
4. add and remove 클릭 
5. 왼쪽에 있는걸 오른쪽으로 보내면 된다. (삭제시 오른쪽을 왼쪽으로)


------------------------
⚠⚠ 코드를 막 짜고 상단의 project에서 clean을 눌러줘야지 자동으로 자바 클래스들이 빠져나온다 (이건 추후 어떤 원리인지 공부 해야겠다.)


------------------------
⚠⚠ server에서 pull 했던 프로젝트의 로컬 호스트를 더블클릭하면 서버를 확인 할 수 있음 // ex)하단 server클릭 -> Apache-tomcat-8.5.90 at localhost클릭


------------------------
⚠⚠ apache-tomcat-8.5.90 at localhost 를 보면 포트 넘버와 포트네임 등 테스트를 하기위한 로컬 포트 들을 볼 수 있다. // 일반적으론 8080


------------------------
⚠⚠ 인터넷 url 창에다가 localhost:8080을 입력하게되면 아까 테스트로 해놓은 로컬호스트에 들어갈 수 있다.



------------------------
⚠⚠ 코드 작성 후 우측 하단 초록 화살표를 누르면 테스트 해볼 수 있고 벌레모양을 누르면 디버깅과 테스트를 동시에 진행 할 수 있다.


 ------------------------
⚠⚠ publishing to tomcat ~ has encountered a problem 오류

실행하려는 프로젝트를 우클릭 한 뒤 refresh를 클릭해주자!! (고로 f5키를 자주 눌러주자)


------------------------
⚠⚠ `console.log("===>", data);` `system.out.println("===>" + data);`

콘솔로그를 수시로 찍어보는 습관을 들이자
그래야지 어디가 잘못되었는지 파악 할 수 있다.(쿼리문에서 콘솔찍는법은 쫌 복잡하다...)


------------------------
⚠⚠ selectbox.js > getValue

상위 콤보박스는 콤보박스가 아니였다.
selectbox.js에서 형식과 꺼내는 방법까지 다 형식을 짜 놓았고
그걸 내가 이용하여 만든 것 뿐이다.
거의 라이브러리인듯하다...


------------------------
⚠⚠ main.jsp > daterangepicker

main.jsp에서 나오는 다른 gitio를 보면
캘린더는 다른 gitio에서 api를 받아와 사용 중 이였다.
어떤식으로 돌아가는지 알고 싶다면 main.jsp에서gitio에 들어가 참고 문헌을 쫌 들여다 봐야 할 듯 하다.


------------------------
⚠⚠ #s:message code > message_ko.properties > audit.auditSearch.action_time=시간

<s:message code='audit.auditSearch.action_time'/> 이거가 '시간' 으로 출력되는 것이다.
message_ko.propertie여기에서 추가 변경 삭제하게된다면 자동으로 바뀌게 되는 것이다!
(참고로 언어작업은 맨 나중에 한번에 한다고 한다 굳이 미리하지말고 하드코딩해놓은다음 나중에 하자)


------------------------
⚠⚠ val, getvalue, getdisplayvalue

일반적인 input box는 val로 값을 받아왔다
하지만 우리가 임의로 만든 select box는 getvalue, getdisplayvalue를 사용해야한다.
js 들어가서 보면 알겠지만 위 두개는 우리가만든 콤보박스에만 활욜할 수 있고 선택한게 getvalue
디폴트값으로 넣어놨던 nowon을 반환해주는게 getdisplayvalue이다. 물론 class nowon은 설정해 줘야한다.
그니까 막쓰지말고 어떤걸로 값을 받아왔는지 생각하고 jquery에서 유동적으로 사용해야한다.


------------------------
⚠⚠ log4j2.xml > (7번째줄) <ThresholdFilter level="DEBUG" (원래는 INFO) 
이걸 사용하게 된다면 
이 로그 파일은 평소 콘솔에 띄워주는 것들을 표현해 주고있다. 
실전땐 콘솔창이 더러워 져서 INFO를 해놓고 사용하지만 나같은 배우는 입장에선 콘솔창에서 자세하게
알려주는것이 좋기에 DEVUG로 돌려놓고 사용한다.


------------------------
⚠⚠ 서비스 > `Map<String, Object> paramMap = p.getRequestParamMap();`

난 Map<String, Object> paramMap = new HashMap<String, Object>(); 이것만 해줬다 그런데 이건 값을 그냥 선언만 해준것이지 결국엔 빈값만 있게 된다. 
평소에 값을 받아오는 적은 별로 없다보니 그냥 막막 복사해서 썻지만 input같이 값을 받아올 땐 서비스에서 처리를 잘해줘야한다. 
고로 위에 적어놓은 겟리쿼스트를 들어가 보면 키벨류값을 알아서 받아오도록 만들어 놓았다. 따라서 원리를 많이 공부해야할 듯하다.
참고로 getRequestParamMap은 ParameterObject.java에서 찾을 수 있다.
뷰에서 파라미터 값을 뭘 가져오는지는 서비스에서 System.out.println(paramMap);를 찍어보면 알 수 있다.


------------------------
⚠⚠ 셀렉트 박스 값 도출 및 가공

1. 첫번째로 셀렉트 박스가 맞는지 확인
2. 맞는 박스로 테스트함수에 넣어 값이 도출되는지 확인
3. ajax에 값을 전달
4. xml 쿼리문 짜기
5. 값 맵핑(컨트롤 > 서비스 > 다오)
6. 값 도출 확인

------------------------
⚠⚠ 서비스에서 실수 paramMap!!!!!
List든 Map이든 뭐든 p.getRequestObjectMapper이든 세션이든 뭐든 get으로받았으면 put으로 기존 불러왔던 리스트에 집어넣어줘야한다. 그래야지 뭘 추가하지 [x,y,z]가 있는데 a를 get으로 불러왔어 그럼 그걸 put으로 [x,y,z,a]로 집어 넣어줘야한다 이말이다!
서비스에서 자꾸 실수를 한다. 값을 받았으면 넣어줘야하는데 계속 안넣어주니 이런 반복적인 실수를 범하고 있다.
그리고 순서가 문제였다. 
정확히 어떤기능을 하는지도 모르고 마구자비로 넣었다가 선언도 안한 것들을 넣다보니 오류가 난것이였다.
고로 어떤기능을하는지 먼저 파악을하고 그것을 어떻게 가공할지 선택하여 사용해야한다.!


------------------------
⚠⚠ 화면단위 오류는 왼쪽 페이지 콘솔에서 확인하고, xml이나 내부 오류는 우측 이클립스 콘솔에서 확인하자


------------------------
⚠⚠ 엑셀파일 다운로드 만드는법  

※※ 쿼리,다오,서비스 까지만 만들어주면 된다. (callService때문에)
개요 : grid에 있는 조회한 리스트 들을 뽑을려고 한다. 여기선 페이지수도 상관없고 그냥조회된 모든 값들을 엑셀로 넘겨주려고 한다.
excelUtils.js에 있는 fn.excelDownloadCallServiceFunc를 이용하여 차례대로 function에 있는 값들을 지정해주면된다. ex) `$(grid).excelDownloadCallServiceFunc(callService, keyset, titleset, obj, "test", "test", 60000);`  이렇게 말이다.
그러기위해서는 일단 조회하는 것들이 필요하다(조회할때 ajax위에 있는 변수들 var datasplit,startdat,yrow,ip 등등)
이것들을 이용하여 keyset과 titleset으로 html에 있는 key data값들과 s메시지 들을 잡아주고 
obj 즉 파라미터로 넘긴 값들을 이용하여 조회하여 그 값들을 도출해내고 출력해준다.
1. callService를 선언한다 : var callService = "서비스파일명$메소드이름"
2. keyset을 선언한다 : var keyset = $(grid).getKey();
3. titleset을 선언한다 : var titleset = $(grid).getTitle();
4. 검색 메소드 ajax위 변수들을 긁어 온다.
5. param을 선언한다 : (검색 ajax에 있는 넘겨주는 data를 긁어 온다.) `var obj = {StartDate: StartDate, EndDate: EndDate,};`
6. 엑셀다운로드함수에 값을 넣어준다 : `$(grid).excelDownloadCallServiceFunc(callService, keyset, titleset, obj, "test", "test", 60000);`

참고자료 :  excelDownloadCallServiceFunc
excelUtils.js               fn.excelDownloadCallServiceFunc참고하기
ExcelDownloadController.java 846    @excelDownloadCallServiceFunc.file 참고하기
ExcelUtils.java   SXSSFWorkbook이것이 엑셀파일을 다운로드? 하는 거라고 들었다.(워크북)
밑에부턴  excelDownloadCallServiceFunc을 사용하는 예시이다.
adminManager.js   331
listUtils.js    855getTitle과  885getKey를 받아서 excelDownloadCallServiceFunc(블라블라~~~~, 여기에 넣는다!)


------------------------
⚠⚠ #뷰에서 서비스로 값 가져오기, #view에서 받은 배열 -> 쿼리에서 가공하는법 (쉽게말해 Array -> 스트링(map)  -> 리스트 스트링(List<String>) -> foreach로 하나하나 넣어주기

view에서 먼저 체크된 것들을 각각 스트링으로 받게되는데
이것들은 서비스에 가서도 고대로 스트링으로 박히게 된다.
Map<String, Object> paramMap = p.getRequestParamMap(); 이렇게 선언했기때문에
ex)['hacs1', 'hhacs', 'hhhcs', 'hacss1']'hacs1', 'hhacs', 'hhhcs', 'hacss1'
그렇기에 서비스에서 다시 가공해줘야한다.
List<String> ids_list = p.getRequestObjectMapper("ids", List.class);
ex)['hacs1', 'hhacs', 'hhhcs', 'hacss1']
해석 : 리스트스트링으로 만들어줄것이다 ids_list를 = parameterObject인 p에서 받아온 키값이 "ids"인 값을 getrequest를 이용하여 받아와서 List.class형식으로 저장
그러면 쭉 스트링이였던 그 값들은 하나하나 분리된 리스트 스트링으로 바뀌게 된다.
그렇지만 이대로 쿼리문에 들어가면 오류가 나기에 foreach를 사용하여 배열 수 만큼 for문을 돌려 하나하나 배열값들을 넣어주는 쿼리문을 만들어야한다. 
`<foreach collection="ids_list" item="ids" open="and a.user_id IN (" separator="," close=")"> #{ids} </foreach>` 이렇게 해주면 된다.
List<String>컬렉션 을 넣어주면 되고 아이템은 맘대로 넣어주는 변수명이다 하지만 되도록이면 #{x}값으로 넣어주도록 하자 헷갈리기도 하고 결국 그게그거니까
 ids=["hacs1", "hhacs", "hhhcs", "hacss1"]  -->>
 ids_list=[hacs1, hhacs, hhhcs, hacss1]
뭐가달라졌는지 보이는가? 스트링이 리스트로 바뀐것이다!


------------------------
⚠⚠ # db에서 서비스로 값 가져오기(쿼리문 짰다는 가정하에)

@Autowired를 통해 직접적으로 Dao dao;로 가져올 수 있지만 여기는 아닌듯 하다. sql세션에서 값을 받아와 사용하는것같다.(공부필요)

```
List<Map<String, Object>> list = sqlSession.getMapper(TemplateDao.class).templateAuditList(paramMap);
		p.addResultData("list", list);
```

이렇게 값을 DB->DAO->SERVICE로 가져온 다음 list로 가져오면 된다.
이러면 list에 SQL select문에서 가져온 action_code나 detail같은 값들을 list에(LIST로 만들었으니) 저장할 수 있다. 


-------------------------
⚠⚠ 팝업??

팝업이란 클릭 시 detail같은 것들을 창이 나와 보여주는 것이다.
팝업에 종류에는 다양하다 윈도우, 레이업 등등 현재 우리가 직접 만든 팝업양식을 통해 만들 수 있다.
윈도우팝업과 달리 레이업팝업은 현재 창에서 또다른 창을 불러오는것이 아니라 현재 창에서 팝업창을 띄워주는 것이다.
그러기에 레이업팝업창은 현재창에서 벗어날 수 없다. 마치 alert창 같은 느낌인 것이다.
팝업창을 띄우는 법은 $(this).openLayerPopup이 있다. 
참고로 팝업윈도우는 api를 사용하고있다. 그러기에 js파일에 들어가서 어떻게 값을 받아오고 사용하는지 공부해봐야한다.
레이업팝업은 윈도우 팝업과는달리 오브젝트로 바로 가능하다. 뷰에서 즉시 파라미터에 넣어서 슥슥 데이터를 지정할 수 있다.

------------------------
⚠⚠ 위드 리쿼시브 쿼리(구문을 통해 쿼리가 반복되며, 반복된 결과를 부모쿼리영역에서 from절로 가져와 사용하는 구조이다.)
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
⚠⚠ ORDER BY 정렬할 컬럼 DESC

값들은 항상 최신것들을 보여줘야하기때문에 쿼리 제일 마지막 리미트 전에 order by 정렬할 컬럼 desc를 해야한다 

그래야지 보통 시간으로 정렬했을때 최신것 부터 보여주게 된다. 그리고 정렬을 안하고 리미트롤 자를 시엔 데이터가 이상하게 짤릴 수 있다. 

그러기에 리미트를 걸던 어떤 데이터를 다중으로 보여주는 상황에는 반드시 정렬을 해주자

------------------------
⚠⚠ 전역변수 선언상황

전역변수는 다른 메소드에서 하나의 변수를 사용할때 사용하는 특별한 경우에만 사용하게 된다. 그걸 제외하곤 보통 지역변수를 많이 사용하곤한다.

전역변수를 사용하는 예시를 보여주겠다.

먼저 팝업 이벤트를 사용하기위에 AJAX를 통해 데이터 값을 불러오게된다. 그러면 그 값은 그 메소드에서만 돌게 된다 

하지만 전역변수를 이용하여 그 변수에 불러온 데이터를 삽입하면 다른메소드에서도 사용할 수 있다.

그럼 그 변수를 이용하여 팝업 이벤트 메소드를 만들어 현재 화면에 나온 데이터를 팝업 화면에 보여줄 수 있고 입맛대로 만들 수 있다!

하지만 이러한 경우는 당연하지만 AJAX요청이 완료된 후 비동기적으로 설정되기에 시작하자마자 전역변수에 값을 넣어주지 않는다면 오류가 나게된다.

고로 이때 사용할 팁은 AJAX에서 complete를 이용하여 무조건 실행을 시킨 후 초기값을 넣어주게된다면 비어있는 변수를 마주할 일이 없게 된다.(success에 넣어도 되긴한다 왜지?....)

------------------------
⚠⚠ # CSS # disabled #`<input type="text" id="multi_dataid" class="text" disabled/>`

disabled는 선택, 클릭, 입력 등 포커스를 받지 못하게 하는 기능이다.

이것을 위와같은 코드로 작성하게된다면 비록 인풋박스이지만 선택도 클릭도 입력도 할 수 없는 박스가 된다.

주로 아이디나 비밀번호를 표시해줄때 사용하게된다.(수정 못하게)

------------------------
⚠⚠ Mybaits를 이용한 UPDATE 쿼리~뷰까지 만들기

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

⚠⚠ **#SUBSTITUTE #view #jsp #replace #일정 택스트부분 원하는 값으로 변환**<br/>
엑셀에서 일정 텍스트를 원하는 값으로 바꾸려면 SUBSTITUTE를 사용한다. ` SUBSTITUTE("abcdefghi","def","xxx") => 'avcxxxghi' `

이러한 유용한 기능을 뷰에선 사용할 수 없을까??

당연히 사용할 수 있다. 바로 replace이다.

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

