# Jeju_project

## 프로젝트 설명
- 언어 : python, google colab
- 인원 : 6명 (팀장 : 본인, 팀원 5명)
- 기간 : 2023.09.06 - 2023.09.26
- 주요내용
  + 제주 관광 공사에 제안서를 만드는 것을 최종 목표로 삼음.
  + ~~현재 독립변수 지정에 대한 회의를 거치는 중으로 확정시 수정 예정.(23.09.08)~~
  + ~~날씨의 영향으로 인한 항공편, 선박편 연착 문제를 다루는 것으로 함. 입도객 통계 일부를 뒷받침함. => 날씨가 독립변수.~~
  + 현재 날씨와 관련지을 항공편 결항 부분과 관광객수에 대한 가설검증이 제대로 이루어지지 못해 이 부분은 fail 요인으로 따로 기록하는 것으로 확정지음.(23.09.12)
  + 성수기/비성수기 부분의 통계를 통해 입도객 통계의 성수기 월별의 통계를 뒷받침함. => 성수기가 독립변수. (이 때, 성수기는 12-1월, 7-8월로 설정잡음. 여름휴가와 크리스마스 연말 등을 성수기로 잡음.)
  + 물가 관련 데이터를 제주 지역으로 한정해 수집하여 물가에 따른(숙박비별, 식비별, 항공/선박비별, 관광/문화지출별) 관광객들의 통계를 수집함. (+ 추후 뒷받침 할 근거로 만족도 조사를 찾아둠.)
 
- 역할
  + ~~주제가 갈아엎어져 역할 재분담 필요. 확정시 수정 예정.(23.09.08)~~
  + 현재 각 파트당 역할을 분담함.
    + 날씨 파트 : Sang-Hyeok-Lee(https://github.com/Sang-Hyeok-Lee), SangMingyu(https://github.com/SangMingyu)
    + 성수기/비성수기 파트 : Ezraelyes(https://github.com/Ezraelyes), HWANHEECHO(https://github.com/HWANHEECHO)
    + 물가 파트 : HaJeong-K(본인), Grace Kim(https://github.com/haeunkim48)
 


## 개발 로그 기록
- ~~데이터 수집 이후 시작할 예정.(23.09.08)~~
- 데이터 전처리 과정은 넘어서야 트러블 슈팅이 진행될 것 같음.(23.09.12)

[2023.09.11]
- 오늘 한 일
  + 날씨 : 18~22년까지의 월별 방문객 데이터와 강수량 데이터 통합.
  + 성수기 : 2022년 여름시즌 사전, 사후조사 데이터 수집.
  + 물가 : 2018~19년 데이터 수집 완료.

- 오늘 못한 일
  + 날씨 : 강수량에 따른 항공기 결항 상황이나 결항에 따른 입도객 차이수 확인.
  + 성수기 : 2022년 여름시즌 사전, 사후조사 데이터 전처리.
  + 물가 : 2020~21년 데이터 수집 및 일부 데이터 전처리 시작.

- 내일 할 일
  + 날씨 : 결항관련 데이터 수집.
  + 성수기 : 2022년 여름시즌 사전, 사후조사 데이터 수집.
  + 물가 : 2020~21년 데이터 수집 및 모든 데이터 전처리 시작.

- **Trounle-shooting**
  + **날씨 부분만 현재 코드가 진행됨.**
  + 모든 목적별 방문객의 합을 변수로 갖는 전체 방문객 컬럼을 만드는 과정에서 합계 수치가 과도하게 크게 나타나 일부 변수 대상 문자열 -> 숫자열 변환 시행
 

[2023.09.12]
- 오늘 한 일
  + 날씨 : 항공기 결항 및 실내 관광지 데이터 탐색, 확인, 입도객 데이터와 대조, 강수량별 전체 관광객 비교 .
  + 성수기 : 2022년 사전/사후조사 데이터 전처리.
  + 물가 : 2018년 프로파일, 항공 경비 관련 일부 전처리/2019년 프로파일, 지출경비 관련 일부 전처리.

- 오늘 못한 일
  + 날씨 : 날씨 데이터 자체가 전체 관광객에 영향을 별로 미치지 못한다는 결론이 도출되어 실패된 케이스로 돌아가버림, 그렇기에 다른 변수 및 내용을 탐색해봄.
  + 성수기 : 데이터 차이 관련하여 해결하지 못함, 전처리 일부 미완.
  + 물가 : 2018년, 2019년 데이터 전처리 일부 딜레이.

- 내일 할 일
  + 날씨 : 쓸만한 새로운 데이터(변수)를 찾거나, 다음 주제인 관광지 탐색파트를 미리 탐색해보기.
  + 성수기 : 월간 보고서와 다른 데이터간의 차이 관련 토의, 다른 년도 월별 입도/방문객 데이터 전처리 등.
  + 물가 : 2018, 19년 데이터 남은 전처리 + 2020,21 년 데이터 전처리 시작.

[2023.09.13]
- 오늘 한 일
  + 날씨 : 제주 인기 관광지 탐색 및 데이터 수집(trip.com, trip advisor 등 제주 추천 관광지 직접 추출), 크롤링 or 텍스트마이닝과 워드클라우드 진행해보기.
  + 성수기 : 2022년 사전/사후조사 데이터 전처리 추가작업, 2020-2022 방문 관광객 월간 보고서 파일 다운로드 후 테이블 데이터 일부 전처리.
  + 물가 : 2018, 2019, 21년 전처리 마무리, 2020년, 2022년 전처리 시작.

- 오늘 못한 일
  + 날씨 : 결과가 정상적으로 출력되지 않음  사실상 실패.
  + 성수기 : 월간 보고서에서 활용할 데이터 토의 및 데이터 전처리.
  + 물가 : 2020년 데이터 전처리 마무리.

- 내일 할 일
  + 날씨 : 데이터수집을 더하거나 크롤링, 텍스트마이닝을 다듬어 전체 데이터 워드클라우드 출력까지 확인해보기.
  + 성수기 : 활용 데이터 확정 및 전처리 마무리.
  + 물가 : 2020년, 2022년 전처리 마무리 + 통계분석 시작.

- **Trounle-shooting**
  + 물가 파트 전처리 과정에서 csv파일을 pandas DF로 읽어오는 것에 실패함 => 인코딩의 문제가 있었음.
  + 해결방법을 찾아 해결했고, 블로그에 상세히 작성함. (https://forky-develop.tistory.com/entry/%EB%8D%B0%EC%9D%B4%ED%84%B0-%EC%A0%84%EC%B2%98%EB%A6%AC-%EA%B3%BC%EC%A0%95%EC%97%90%EC%84%9C-%EB%B0%9C%EC%83%9D%ED%95%9C-csv-%ED%8C%8C%EC%9D%BC-%EC%9D%B8%EC%BD%94%EB%94%A9-%EC%9D%B4%EC%8A%88-%ED%95%B4%EA%B2%B0%EB%B2%95)
  + 인기 관광지 목록을 텍스트 마이닝해서 워드 클라우드를 활용하는데 한글이 깨지는 현상이 일어남 > matplotlib.font_manager 참고해서 해결함.
