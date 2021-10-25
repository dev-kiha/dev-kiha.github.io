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

    
3.GROUP BY 구
4.HAVING 구
5.ORDER BY 구
6.뷰와 서브쿼리
