## 🗂 폴더/파일 구분
## ✏️ 데이터 전처리

1. 위도, 경도를 찾기 위해 실거래가 데이터 eda
    1. 필요한 컬럼 정리
        1. 분산되어 있는 주소들을 하나로 합쳐준다.
        2. 전용면적의 소수값을 제거해 통일해준다.
        3. 동, 번지, 단지명, 전용면적(㎡), 면적라벨, 거래금액(만원), m2당금액(만원),계약년, 주소를 제외한 컬럼을 삭제한다.
    2. Grouping 및 평균 금액 구하기
        1. 연도, 주소, 아파트명, 전용면적을 기준으로 한다.
        2. agg는 평균으로 한다.
        3. 금액의 경우, 소수점은 int로 처리한다.
    
2. location table 만들기
    1. Naver Map API key 발급받기
    2. Naver Map API를 통하여 위도, 경도 내려받기
    3. json 파일로 만들고 이후에 dataframe으로 만들기
    4. 컬럼명
        1. 도로명
        2. 아파트 이름
        3. 전용 면적
        4. 평균 거래가격
        5. 거래연도
        6. 위도
        7. 경도
