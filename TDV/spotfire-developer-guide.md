# TDV 특정 함수 Push-Down 하기

## 1. Query Plan 확인
Query Plan을 통해 특정 DataSource에서 PushDown 이 안되는 함수 명 확인 하기

## 2. capabilities 편집 하기

### 2.1. 특정 Data Source의 Capabilities 폴더 이동
``` bash
cd {TIBCO_HOME}/apps/dlm/cis_ds_{DataSource}/conf 
```
예) Hive2 DataSource 폴더 : {TIBCO_HOME}/apps/dlm/cis_ds_hive2/conf 

### 2.2. 특정 Data Source의 Capabilities 파일 수정
``` bash
vi {DataSource}.capabilities 
```
예) vi hive2.capabilities

### 2.3. 특정 Data Source의 Capabilities 파일 수정
``` bash
vi {DataSource}.capabilities 
```
예) vi hive2.capabilities

함수 추가

TDV인식 함수(파라미터 타입1, ...) : 원천 DataSource Native함수 명 (파라미터 번호)
아래 CEILING 함수를 Hive의 CEILING 함수로 맵핑하여 Push-Down
``` bash
CEILING(~number): CEILING($1)
```

## 3. TDV 재시작

## 4. Query Plan 재확인

## 5. Custom Function 등록 후 해당 함수를 Capabilities 파일로 Native 함수 맵핑 가능


