### 문제
```
동물 보호소에 가장 먼저 들어온 동물의 이름을 조회하는 SQL 문을 작성해주세요.
```

### 풀이
```mysql
SELECT NAME
FROM ANIMAL_INS 
ORDER BY DATETIME
LIMIT 1;
```

### 정리
1. `LIMIT`, `OFFSET`
```mysql
LIMIT 10; # 맨 위부터 10개 행 선택

LIMIT 10 OFFSET 3; # 맨 위에서 3번째 행부터(포함) 10개의 행 선택 (단, 1번째 행은 0)

LIMIT 3, 10; # 위의 문장과 같은 역할을 한다. LIMIT offset수, limit수
```
