---
layout: post
title:  "06.SELECT 구문"
date:   2021-10-25 23:45:27 +0900
categories: sql-level-up 
---
검색 : 데이터베이스를 이용할떄 핵심 처리 (==질의, 추출)
검색을 위해 사용하는 SQL구문을 SELECT 구문이라고 함.

1.SELECT 구와 FROM 구
    FROM을 반드시 입력해야 하는 것은 아니다 (SELECT 1 과 같이 상수를 선택하는 경우, 오라클은 예외)
    SELECT 구문에는 데이터를 어떤 방법으로 선택할지 일절 쓰여있지 않다(=절차지향)
    불명한 데이터를 공란으로 표시한다(NULL)
    
2.WHERE 구
    특정조건에 맞는 일부 레코드만 선택하고 싶을때 사용(=필터조건)
    WHERE는 '어디?'라는 의문사가 아닌 '~라는 경우'를 나타내는 관계부사
    
###WHERE 구의 다양한 조건 지정
다양한 연산자(=,<>,>=,>,<=,<)

###WHERE 구는 거대한 벤다이어그램
AND...OR...
###IN으로 OR조건을 간단하게 작성
WHERE ... IN ('A','B','C')
###NULL-아무것도 아니라는 것은 무엇일까?
IS NULL, IS NOT NULL (NULL은 데이터값이 아니므로 연산자를 쓸 수 없다)

3.GROUP BY 구
홀케이크를 '칼'을 이용해 나누어 먹는다 == 테이블을 'GROUP BY'를 사용해 다룬다
SQL의 대표적인 집계 함수 (COUNT,SUM,AVG,MAX,MIN)
'GROUP BY ()' -> 키를 지정하지 않는다(생략과 동일, 지원하지 않는 DBMS가 많음)

4.HAVING 구
HAVING 구를 사용하면 선택한 결과 집합에 또다시 조건을 지정
(WHERE가 '레코드'에 조건을 지정한다면, HAVING 구는 '집합'에 조건을 지정하는 기능)

5.ORDER BY 구
ORDER BY를 지정하지 않으면 엉터리로 지정한다
DESC -> Descending Order
ASC -> Ascending Order

6.뷰와 서브쿼리
뷰는 데이터를 보유하지 않고 SELECT구문을 저장만 함
###익명 VIEW
뷰는 SELECT 구문이 중첩되어 있는 구조
FROM 구에 직접 지정하는 SELECT 구문을 서브쿼리(subquery)라고 부름
###서브쿼리를 사용한 편리한 조건 지정
IN 내부에서 서브쿼리 사용
(내부적으로는 서브쿼리를 전개해서 실행)
