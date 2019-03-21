1. String
immutable(불변) -> thread safe
new를 통해 생성된 메모리 공간이 불변. 즉 연산이 발생하면 새롭게 new를 한다 -> 성능적 이슈와 GC 이슈가 있음.

2. StringBuffer
mutable(가변), synchronized 키워드가 가능 -> thread safe
생성된 메모리 공간이 가변. 연산이 빠름. 

3. StringBuilder
mutable(가변) -> single thread에서만 사용
생성된 메모리 공간이 가변. 연산이 빠름. 