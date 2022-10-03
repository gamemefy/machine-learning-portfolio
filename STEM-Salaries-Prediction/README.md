# STEM 직군 연봉 예측 머신러닝 프로젝트  

* `STEM`: Science, Tech, Engineering, Math의 앞글자를 딴 말로, 일반적으로 이공계를 의미

## 프로젝트 가설 설정

* IT 업계에서는 이직이 잦은데 이직 이유 중 연봉이 차지하는 비중이 큼(https://www.apollotechnical.com/career-change-statistics/). 이에 대해 검색을 해보는 경우가 많은데, 실제 연봉 데이터를 기반으로 API 서비스를 개발하여 회사 이름과 직책, 직군 등 조건을 입력함에 따라 신뢰할만한 연봉 예측값을 제공해주는 앱을 만든다면, 간단하더라도 많은 STEM 직군 종사자들이 이용할 것

## 데이터셋
* levels.fyi의 연봉 데이터(참고: https://towardsdatascience.com/a-beginners-guide-to-grabbing-and-analyzing-salary-data-in-python-e8c60eab186e)

  * 특성(features)

    * 설명         
      ---  ------                   --------------  -----         
      0   timestamp :        기록된 시간

      1   company  :         회사    

      2   level  :       직급       

      3   title :          직책   

      4   totalyearlycompensation :  기본급과 상여금 등 각종 수당을 포함한 연봉  

      5   location :     직장 위치       

      6   yearsofexperience:   (연 단위)경험    

      7   yearsatcompany  : 직장 내 근무 기간       
      
      8   tag : 풀스택, 백엔드 등 구체적인 직무 설명     

      9   basesalary  :  기본급      

      10  stockgrantvalue  :  보상으로 주어진 주식(무상) 가치       

      11  bonus :  추가 수당       

      12  gender :  젠더     

      13  otherdetails  :  기타 세부사항   

      14  cityid :  미국내 도시 ID         

      15  dmaid  : 방송 권역 ID  

      16  rowNumber : 행 번호    

      17  Masters_Degree : 1(석사 학위가 최종 학위), 0       

      18  Bachelors_Degree : 1(학사 학위가 최종 학위), 0    

      19  Doctorate_Degree : 1(박사 학위가 최종 학위), 0    

      20  Highschool : 1(고등학교 학위가 최종 학위), 0      

      21  Some_College : 1(전문대 학위가 최종 학위), 0       

      22  Race_Asian : 아시아인       

      23  Race_White : 백인     

      24  Race_Two_Or_More : 두 가지 이상의 인종

      25  Race_Black : 흑인      

      26  Race_Hispanic : 히스패닉     

      27  Race : 인종   

      28  Education : 교육 수준 



## 프로젝트 진행 내용

* EDA

* 전처리
* 특성공학
* 머신러닝 알고리즘 적용
  * 선형 회귀

  * 릿지 회귀
  * xg부스트
  * 랜덤포레스트
* 결과 시각화

## 한계 및 개선점

* API 서비스를 구현하여 배포

* timestamp를 사용하지 않았는데, 이는 '기록된' 시간으로, 실제 급여를 언제 받았는지와 다를 수 있다. 그리고 이는 현재 해당 직무, 직책을 가졌을 때 해당 회사에서 어느 정도의 연봉을 기대할 수 있는지와 차이를 만들 수 있다. 이와 같이, 
