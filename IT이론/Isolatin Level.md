Isolation Level

1. Read Uncommited (Level 0)
commit 되지 않은 데이터도 읽을 수 있다
Dirty Read, Unrepeatable Read, Phantom Read 발생가능

2. Read Committed (Level 1)
commit된 데이터만 읽을 수 있다.
Unrepeatable Read, Phantom Read 발생 가능

3. Repeatable Read  (Level 2)
Phantom Read 발생가능

4. Seriazable  (Level 3)
가장 강력한 레벨


* Dirty Read
커밋되지 않은 데이터 읽는 경우
* Unrepeatable Read
특정 데이터를 select 할 경우 데이터가 다름
* Phantom Read
특정 범위 데이터를 읽을 경우 데이터가 다름
