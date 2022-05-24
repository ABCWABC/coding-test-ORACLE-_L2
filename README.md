# coding-test-ORACLE-_L2

## level 2
  1. 고양이와 개는 몇 마리 있을까
  2. 동명 동물 수 찾기
  3. 입양 시각 구하기(1)
  4. 최솟값 구하기
  5. 동물 수 구하기
  6. 중복 제거하기
  7. 입양 시각 구하기(2) #
  8. 이름이 없는 동물의 아이디
  9. 이름이 있는 동물의 아이디
  10. NULL 처리하기
  11. 없어진 기록 찾기
  12. 있었는데요 없었습니다 @
  13. 오랜 기간 보호한 동물(1) #
  14. 보호소에서 중성화한 동물
  15. 루시와 엘라 찾기
  16. 이름에 el이 들어가는 동물 찾기 #
  17. 중성화 여부 파악하기 #
  18. 오랜 기간 보호한 동물(2)

## 코드
  1. 날짜or시간 포맷 변경 > TO_CHAR(DATETIME, 'HH24')
  2. 중복값 제거 > DISTINCT
  3. 계층형쿼리
      - 0~23까지 숫자 > SELECT LEVEL-1 AS HOUR
                        FROM DUAL
                        CONNECT BY LEVEL BETWEEN 0 AND 24
  4. NULL 인 값 찾기 > WHERE 컬럼명 IS NULL
  5. NULL 값이면 특정값 출력 > NVL(컬럼명, '특정값')
  6. A테이블에 없는 B테이블 값 찾기 > 차집합 연산자 MINUS
  7. 외부조인 > WHERE 테이블명1.컬럼명1(+) = 테이블명2.컬럼명2   또는   테이블명1.컬럼명1 = 테이블명2.컬럼명2(+)
  8. 해당값과 일치하는 조건 > WHERE 컬럼명 IN ('값1', '값2', ...)
  9. 해당값이 들어가는 조건 > WHERE (컬럼명 LIKE '%값1%' OR 컬럼명 LIKE '%값2%')
     - () 안해주면 다른 조건 입력시 틀린값이 조회됨
  9-2. 대소문자 구분없이 해당값이 들어가는 조건 >  WHERE (LOWER(NAME) LIKE '%el%')
     - 미리 컬럼값을 대문자 또는 소문자로 바꾼후 진행
  10. case 문
