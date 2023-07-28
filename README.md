# TIPS


———————————읽기 전에——————————————
📌📌 : 자주 쓰는 팁(중요도 1순위)
⚠⚠ : 정렬 안된 팁(중요도 2순위)
- [ ]  : off시 미해결 on시 해결
//(주석) : 일지 및 그때 느낌
—————————————————————————————-

⚠⚠ 엑셀파일 다운로드 만드는법  
※※ 쿼리,다오,서비스 까지만 만들어주면 된다. (callService때문에)
개요 : grid에 있는 조회한 리스트 들을 뽑을려고 한다. 여기선 페이지수도 상관없고 그냥조회된 모든 값들을 엑셀로 넘겨주려고 한다.
excelUtils.js에 있는 fn.excelDownloadCallServiceFunc를 이용하여 차례대로 function에 있는 값들을 지정해주면된다. ex) $(grid).excelDownloadCallServiceFunc(callService, keyset, titleset, obj, "test", "test", 60000);  이렇게 말이다.
그러기위해서는 일단 조회하는 것들이 필요하다(조회할때 ajax위에 있는 변수들 var datasplit,startdat,yrow,ip 등등)
이것들을 이용하여 keyset과 titleset으로 html에 있는 key data값들과 s메시지 들을 잡아주고 
obj 즉 파라미터로 넘긴 값들을 이용하여 조회하여 그 값들을 도출해내고 출력해준다.
1. callService를 선언한다 : var callService = "서비스파일명$메소드이름"
2. keyset을 선언한다 : var keyset = $(grid).getKey();
3. titleset을 선언한다 : var titleset = $(grid).getTitle();
4. 검색 메소드 ajax위 변수들을 긁어 온다.
5. param을 선언한다 : (검색 ajax에 있는 넘겨주는 data를 긁어 온다.) var obj = {StartDate: StartDate,
	 			EndDate: EndDate,};
6. 엑셀다운로드함수에 값을 넣어준다 : $(grid).excelDownloadCallServiceFunc(callService, keyset, titleset, obj, "test", "test", 60000);

참고자료 :  excelDownloadCallServiceFunc
excelUtils.js               fn.excelDownloadCallServiceFunc참고하기
ExcelDownloadController.java 846    @excelDownloadCallServiceFunc.file 참고하기
ExcelUtils.java   SXSSFWorkbook이것이 엑셀파일을 다운로드? 하는 거라고 들었다.(워크북)
밑에부턴  excelDownloadCallServiceFunc을 사용하는 예시이다.
adminManager.js   331
listUtils.js    855getTitle과  885getKey를 받아서 excelDownloadCallServiceFunc(블라블라~~~~, 여기에 넣는다!)
