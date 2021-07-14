# DeepLearning_BeTheLegend

## 2021. 06. 30
### To do List
1. 스탯티즈에서 타자 데이터 수집

스탯티즈(http://www.statiz.co.kr/main.php)

구단 별 타석 수 내림차순 정렬 후 9명 선수를 대상으로
선수정보 - 각타자 - Playlog - 개막부터 6/30 까지 데이터 수집

## 2021. 07. 03
### To-do List
1. 투수 유형
2. 선수 날짜별 데이터 90명 다시 복사 붙여넣기 (선수정보 - 날짜별 수집 > 선수명 기입)
3. 현재까지 모은 데이터 날짜로 묶어야하고
4. 2번에서 모은 데이터로 최근 5, 10경기 타율 뽑아야하고
5. 타율은 2번 데이터에서 활용

## 2021. 07. 05
### To-do List
1. 최근 5일 타율 계산 시, 최근 5일 내에 타수가 있으면 (=타수의 합이 0이 아니면) 그 결과를 반영
2. 최근 5일 / 최근 10일 타율 피쳐를 동시 사용시, 10일 타율에서 5일의 공백이 발생 
최근 5,10경기 타율 및 팀 별 타율 계산 완료

해야할 것: 최근 5일에 대한 타율 및 투수 유형 별 타율, 선발 투수 

※모델 개선 시에는 날짜 별로 가중치를 다르게 줄 수 있을까?

**2021.07.11 수정사항
최근 5일(변경 가능) 경기의 타율 구하기.ipynb 의 결과 테이블의
이름(recent_5days_hitter), 날짜(recent_5days_day)의 복합키로 기본키 가능, 다른 테이블과 조인할때 참고


## 2021. 07. 11
### To-do List
1. 새로운 컬럼 추가: 투수 유형별 타율, 구장별 타율, 상대 팀 타율 수정 및 한 팀 추출
2. EDA  
3. 난관 : 데이터프레임 merge시, 더블헤더 날의 중복된 merge 발생

## 2021. 07. 15
### Done List
append double_header code column > modify recent avg, vs_avg definition
now, we correct merge error : final data's length is 5296

### To-do List
append stadium & pitcher type avg column
learn MLP model 
EDA visulization
