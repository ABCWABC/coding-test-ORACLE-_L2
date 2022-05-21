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
  13. 오랜 기간 보호한 동물(1)

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
  7. 
