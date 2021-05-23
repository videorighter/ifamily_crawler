# Web-site Crawler
## ifamily collaboration result

본 크롤러는 아이패밀리와 함께하는 "화장품 소비자 분석 시스템 프로젝트"의 일환으로 개발되었으며, 초기 크롤러입니다. <br>
고도화된 최신 크롤러는 내부 정보이므로 공유가 불가합니다.

### 1. Youtube Crawler<br><br>
>1. argument 입력<br>
>2. argument 기준대로 검색<br>
>3. 스크롤 다운 및 Post URL 수집<br>
>4. 해당 URL 접속<br>
>5. 스크롤 다운 및 Post information & Comment 수집<br>
>6. 결과 도출<br>

**How to use**
```
$ python3 youtube_crawler.py --keyword [KEYWORD] --is_db [True|False] --choose_period [lasthour|today|thisweek|thismonth|thisyear] --post_scroll_num [NUMBER] --comment_scroll_num [NUMBER] 
```
>--keyword : 크롤링 할 키워드 입력 (default: 유튜브)<br>
>--is_db : RDBMS 사용 여부 (default: True)<br>
>--choose_period : 유튜브 검색 기준 선택(기간) (default: thisweek)<br>

>>lasthour : 지난 1시간 <br>
>>today : 오늘 <br>
>>thisweek : 이번 주 <br>
>>thismonth : 이번 달 <br>
>>thisyear : 올해 <br>

>--post_scroll_num : post(게시글) 수집 시 스크롤 다운 횟수<br>
>--comment_scroll_num : comment(댓글) 수집 시 스크롤 다운 횟수<br><br>

![image](https://user-images.githubusercontent.com/75473005/119261303-c1fd4900-bc11-11eb-8ad7-d591a5d1c2c4.png)


### 2. Instagram Crawler<br><br>
유료 API 사용<br>
API KEY는 개인 정보이므로 "insert key"로 대체<br>

>1. argument 입력<br>
>2. argument 기준대로 검색<br>
>3. Post short code 수집<br>
>4. Post information 수집<br>
>5. Comment information 수집<br>
>6. 결과 도출 및 RDBMS 저장<br>

**How to use**
```
$ python3 arg_instagram_crawler2.py --keyword [KEYWORD] -n|--post_num [NUMBER]
$ python3 arg_instagram_crawler2.py --keyword [KEYWORD] -d|--post_date [YYYY-MM-DD]
```
>--keyword : 크롤링 할 키워드 입력<br>
>-n | --post_num : 크롤링 할 포스트의 수<br>
>-d | --post_date : 입력한 날짜로부터 게시된 포스트 크롤링<br><br>

### 3. Naver Blog Crawler<br><br>
>1. argument 입력<br>
>2. argument 기준대로 검색<br>
>3. 스크롤 다운 및 Post URL 수집<br>
>4. 해당 URL 접속<br>
>5. 스크롤 다운 및 Post information & Comment 수집<br>
>6. 결과 도출 및 RDBMS 저장<br>

**How to use**
```
$ python3 naver_crawler.py --keyword [KEYWORD] --is_db [True|False] --start_date [YYYY-MM-DD] --end_date [YYYY-MM-DD] --num [NUMBER]
```
>--keyword : 크롤링 할 키워드 입력 (default: 네이버블로그)<br>
>--is_db : RDBMS 사용 여부 (default: True)<br>
>--start_date : 네이버블로그 검색 기간 중 시작 시점 입력 (default: 2021-01-01)<br>
>--end_date : 네이버블로그 검색 기간 중 끝 시점 입력 (default: 2021-06-01)<br><br>

![image](https://user-images.githubusercontent.com/75473005/119261280-a85c0180-bc11-11eb-910a-0dd27127b48b.png)


### 4. Glowpick Crawler<br><br>
>1. argument 입력<br>
>2. argument 기준대로 검색<br>
>3. 스크롤 다운 및 Post URL 수집<br>
>4. 해당 URL 접속<br>
>5. 스크롤 다운 및 Post information & Comment 수집<br>
>6. 결과 도출 및 RDBMS 저장<br>

**How to use**
```
$ python3 glowpick_crawler.py --keyword [KEYWORD] --is_db [True|False]
```
>--keyword : 크롤링 할 키워드 입력 (default: 틴트)<br>
>--is_db : RDBMS 사용 여부 (default: True)<br>

![image](https://user-images.githubusercontent.com/75473005/119261257-8ebaba00-bc11-11eb-8feb-c6d3f662b8f0.png)

