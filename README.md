#공부하는 곳
비글본 블랙을 이용한 리눅스 CE

발생한 문제 on Beaglebone Black

* 자식 프로세스 생성 후 자식 프로세스의 실행문이 마칠때까지 부모 프로세스는 기다리지 않는다.
-------- 터미널 출력시 유저 입력문과 섞여서 나온다.

* alarm, select, poll 등 함수가 프로세스의 블록에 관여하는 함수들 -> 프로세스를 멈추지 않는다.
-------- 폴링 상태로 대기하지 않고 리턴되어 버린다.
