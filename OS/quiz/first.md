# OS

## 개요

1. 기계와 사용자 사이에 명령을 전딜하고 처리한 결과를 알려주는 것을 무엇이라고 하는가?
   - 인터페이스
2. 프로그램과 데이터를 한 번에 입력한 후 작업의 최종 결과만 얻는 운영체제 방식을 무엇이라고 하는가?
   - 사용자 인터페이스?
3. 멀티프로그래밍 수준은 동시에 실행되는 작업의 개수를 나타낸다. 멀티프로그래밍 수준이 1인 시스템을 무엇이리고 히는가?
   - 일괄 작업 시스템
4. 멀티프로그래밍 수준이 2보다 크거나 같은 시스템을 두 개 이상 쓰시오
   - 유닉스, ?
5. 특정 작업이 일정 시간 안에 처리되도록 보장히는 시스템을 무엇이라고 하는가?
   - 실시간 시스템
6. 커널이 자신의 자원을 보호하기 위해 만든 함수의 집합을 무엇이리고 하는가?
   - 시스템 호출
7. 커널과 하드웨어 사이의 인터페이스를 무엇이라고 하는가?
   - 드라이버
8. 커널의 핵심 기능을 구현하는 모듈들이 구분 없이 하나로 구성되어 있는 커널 구조를 무엇이라고 하는가?
   - 단일형 구조 커널
9. 커널의 기능을 최소화하여 여러 컴퓨터에 이식하기 쉽게 만든 커널 구조를 무엇이라고 하는가?
   - 마이크로 구조 커널
10. 서로 디른 운영체제에서 하나의 응용 프로그램으로도 작동할 수 있도록 만든 시스템을 무엇이라고 하는가?
    - 가상머신

### 심화 문제

1. API와 SDK의 차이
   - 어떤 프로그램의 인터페이스 기능을 사용자가 접근 및 수정 가능한 것. SDK는 IDE 같은 개발용 환경까지 제공한다.
2. 단일형 구조 커널의 특징
   - 초창기의 OS구조 커널의 핵심 모듈들이 구분 없이 하나로 구성되어 있다.
3. 마이크로 구조 커널의 특징
   - 마이크로 구조에서 각 모듈은 독립적으로 작동하기 때문에 하나의 모듈이 실패하더리도 전체 운영체제가 멈추지 않는다. 또한 많은 컴퓨터에 이식하기 쉽고 커널이 가벼워 cPU 용량이 작 은 시스템에도 적용이 가능하다.

## 컴퓨터 구조

1. CPU의 구성
   - 산술논리 연산장치, 제어장치, 레지스터
2. 버스의 종류
   - **양방향 구조는 제어 및 데이터** | 주소는 단방향
   - 제어 버스 : **어떤 작업에 대한** 제어 신호 통로 - CPU, 메모리, 주변장치와 양방향으로 오고 간다
   - 주소 버스 : 어느 주소에서 작업할 것인가?
   - 데이터 버스 : **메모리 버퍼 레지스터**와 연결된 버스
3. 다음에 실행할 명령어의 주소를 가지고 있는 레지스터
   - 프로그램 카운터
4. 메모리 주소를 보관하는 레지스터
   - 주소 레지스터
5. 메모리에 저장할 데이터나 메모리에서 가져온 데이터를 임시로 보관하는 레지스터
   - 메모리 주소 레지스터
6. 주소 버스와 연결되어 있는 레지스터
   - 주소 레지스터
7. 데이터 버스와 연결되어 있는 레지스터
   - 메모리 버퍼 레지스터
8. 프로그램을 보호하기 위해 사용하는 두 가지 레지스터는 무엇인가?
   - ?
9. 속도 차이가 나는 두 장치 사이에서 속도를 완화하는 장치를 무엇이라고 통칭하는가?
   - 버퍼
10. 응용 프로그램과 프린터 사이에서 속도 차이를 완화하는 소프트웨어를 무엇이라고 하는가?
    - 스풀
11. 부팅 시 운영체제를 메모리로 가져오기 위해 시용하는 작은 프로그램은 무엇인가?
    - 부트스트랩 코드 (바이오스 -> 마스터 부트 레코드 지역)
12. 속도가 삐르고 값이 비싼 저징장치를 CPU 가끼운 쪽에 두고. 값이 싸고 용량이 큰 저장장치를 반대쪽에 배열하는 방식을 무엇이라고 하는가?
    - 저장장치 계층 구조
13. 작업의 효율성을 높이기 위해 CPU가 입출력 관리자에게 입출력 작업을 요청하면 작업을 마친 입출력 관리자는 CPU에 무엇을 보내는가?
    - 인터럽트
14. CPU의 도움 없이도 메모리를 사용할 수 있도록 입출력 관리자에게 주는 권한을 무엇이라고 하는가?
    - 직접 메모리 접근
15. CPU와 입출력 관리자가 서로 디른 메모리 영역을 사용하는 기법을 무엇이 라고 하는가?
    - 메모리 매핑 입출력
16. CPU가 병렬 처리를 지원하지 않을 때 소프트웨어적으로 병렬 처리를 하는 기법을 무엇이라고 하는가?
    - 병행 기법

### 심화 문제

1. 컴퓨터에서 클록의 역할
   - CPU의 속도와 관련된 단위이다
2. 프로그램 카운터 레지스터의 역할
   - 다음에 실행할 명령어의 주소를 알려준다
3. DDR SDRAM
   - SDRAM의 대역폭 을 늘려 데이터 입출력 속도를 빠르게 한 것이 Double Data Rate SDRAM이다.
4. 즉시 쓰기 방식의 캐시와 **지연 쓰기 방식**의 캐시를 비교하여 설명하시오
   - 즉시쓰기와 다르게 변경된 내용을 주기적으로 반영하는 방식으로, 카피백이 리고 한다. 메모리의 데이터 전송 횟수가 줄어들어 시스템의 성능을 향싱할 수 있으나 메모리와 캐시된 데이터 사이의 불일치가 발생할수도 있다.
5. 인터 럽트 번호를 사용히는 이유를 설명하시오
   - 호출 시 편의성? >> 입출력 관리자가 CPU에게 주변 장치 이름 대신 번호를 알려준다.
6. 메모리 직접 접근(DMA)에 대해 설명하시오
   - CPU의 관할 없이 메모리를 사용할 수 았도록 입출력 관리자에게 주는 권한
7. 메모리 매핑 입출력에 대해 설명하시오
   - CPU와 입출력 관리자가 서로 디른 메모리 영역을 사용하는 기법

## 프로세스와 스레드

1. 프로그램이 프로세스가 되려면 운영체제로부터 무엇을 받아야 하는가?
2. > 프로세스 = 프로그램 + 프로세스 제어 블록
   프로세스 제어 블록(PCB)을 받아야 된다.
3. 프로세스의 상태 중 CPU를 할당받기 위해 기다리는 상태는 무엇인가?
   - 준비 상태
4. 프로세스 상태 중 입출력 작업을 하기 위해 이동하는 상태
   - 대기 상태
5. CPU 스케줄러가 준비 상태에 있는 프로세스 중 하나를 골라 할당하는 작업
   - 실행 상태
6. 프로세스가 강제 중단되면 프로세스는 어떤 상태로 바뀌는가?
   - 휴식 상태
7. 실행 상태에서 하나의 프로세스가 나가고 새로운 프로세스가 들어오는 상황
   - 디스패치
8. 실행 중인 프로세스에서 새로운 프로세스를 복사하는 시스템 호출
   - `fork()` 시스템 호출
9. 프로세스의 골격은 그대로 둔 채 코드 영역만 바꾸는 시스템 호출
   - `exec()`
10. 부모 프로세스가 기다리지 않아 자원이 회수되지 못하고 계속 실이 있는 프로세스
   - 미아 혹은 좀비 프로세스
11. 프로세스의 코드에 정의된 절차에 따라 CPU에 작업 요청을 하는 실행 단위
    - 스레드
12. 미아 프로세스를 방지하기 위해 부모 프로세스는 어떤 시스템 호출을 사용하는가?
    - `exit()` ?
13. 작업이 끝난 프로세스의 자원을 회수하는 행위는?
    - 쓰래기 수집?
14. 모든 프로세스를 부모-자식 관계로 만들어 자원 회수를 용이하게 하는 프로세스의 구조는 무엇인가?
    프로세스 계층 구조

### 심화문제

1. 프로세스 제어 블록의 구성
2. 문맥 교환
   문맥 교환은 CPU를 차지하던 프로세스가 나가고 새로운 프로세스를 받아들이는 작업을 말한다.
3. 프로세스를 구성하는 코드, 데이터, 스택 영역
4. `exec()` 시스템 호출을 사용하는 이유
   시스템 효울을 위해 기존 프로세스 구조를 재활용한다.

## CPU 스케줄링

### 스케줄링 수준

1. 시스템 내 전체 프로세스의 수를 조절하는 것으로, 장기 스케줄링 또는 작업 스케줄링이라 불리는 스케줄링 수준은 무엇인가?
   - 고수준 스케줄링
2. 어떤 프로세스에 CPU를 할당하고 어떤 프로세스를 대기 상태로 보낼지 등을 결정하는 스케줄링 수준은 무엇인가?
   - 저수준 스케줄링

---

1. 입출력을 진행하는 프로세스로, 사용자와 상호작용 가능한다.
   - 전면 프로세스
2. 준비 큐에 도칙한 순서 대로 CPU를 할당하는 비선점형 스케줄링 일고리즘은 무엇인가
   - FCFS(First Come First Served)
3. 준비 큐에 있는 프로세스 중 실행 시간이 가장 짧은 작업부터 CPU를 할당하는 비선점형 스 케줄링 일코리즘은 무엇인가?
   - SJF(Shortest Job First)
4. SJF 스케줄링 알고리즘의 단점으로 크기가 큰 작업이 계속 뒤로 밀리는 현상을 무엇이라 하는가?
   - 아사
5. 아사 현상을 해결하는 방법
   - 프로세스가 양보할 수 있는 상한선을 정하는 방식, 에이징이라고 한다
6. 서비스를 받기 위해 **대기한 시간**과 CPU 사용 시간을 고려하여 우선순위를 정하는 스케줄링 알고리즘
   - HRN(Highest Response Ratio Next)
7. 프로세스가 할당받은 시간(타임 슬리이스) 동안 작업하다가 작업을 완료하지 못하면 준비 큐의 맨 뒤로 가서 디음 자기 차례가 올때까지 기다리는 선점형 스케줄링 알고리즘 중 가장 단순한 것은 무엇인가?
   - 라운드 로빈(순환 순서) 스케줄링
8. 타임 슬라이스의 크기와 문맥 교환의 관계

- 너무 크면 FCFS 스케줄링 비슷하게 된다.
- 작으면 시분할 같이 되지만, 시스템의 성능이 떨어진다

16. 기본적으로 리운드 로빈 방식을 사용하지만, CPU를 할당받을 프로세스를 선택할 때 **작업 시간이 가장 적은 것을 선택하는** 스케줄링 알고리즘은 무엇인가?
    - SRT(Shortest Remaining Time) 우선 스케줄링
17. 우선순위에 따라 준비 큐를 여러 개 사용하며 고정형 우선순위를 적용하는 스케줄링 알고리즘은 무엇인가?
    - 다단계 큐 스케줄링
18. ..준비 큐를 여러 개 시용하며 프로세스가 CPU를 사용한 후 순위가 낮아지는 특징을 가진 스케줄링 알고리즘은 무엇인가?
    - 다단계 피드백 큐
19. 다단계 피드백 큐 스케줄링에서 마지막 큐에 있는 프로세스(우선순위가 가장 낮은 프로세스) 의 타임 슬라이스 크기는 얼마인가?
    - 무한대의 크기
20. 다단계 피드백 큐 스케줄링에서 우선순위가 낮아질수록 타임 슬라이스의 크기는 어떻게 변 히는가?
    - CPU 자원을 얻을 확률이 낮아지기 때문에 그에 반비례하여 슬라이스의 크기가 점점 커진다.
21. 다단계 피드백 큐 스케줄링에서 마지막 큐(우선순위가 가장 낮은 큐)는 어떤 스케줄링 알고리즘처럼 동작히는가?
    - FCFS : 들어온 순서대로 작업을 수행 및 끝낸다.4

### 심화학습

1. 스케줄링의 단계와 그 특징을 설명하시오.
   1. 작업대기
   - **고수준 스케줄링**
   2. 보류 프로세스
   - **중간 수준 스케줄링**
   3. 활성 프로세스
   - **저수준 프로세스**
   4. 실횅 프로세스
   5. 작업 종료
2. 스케줄링의 목적
   - 프로세스 실행 관리
3. FCFS, SJF, HRN 스케줄링의 특징 ?
4. 라운드 로빈, SRT, 다단계 큐, 다단계 피드백 큐 스케줄링의 특징 ?
5. 아사 현상과 에이징에 대해 설명하시오
   - SJF 스케줄링의 단점, SJF 알고리즘의 결함으로 특정 프로세스가 할당을 받지 못하는 현상. 에이징 : 어떤 프로세스의 실행 순서가 뒤로 밀릴 떄마다 가산을 하고, 임계치에 도달하면 해당 프로세스를 실행한다.
6. 타임 슬라이스의 크기를 정하는 것과 시스템 효율성에 대하 설명하시오
   - 우선순위가 높은 작업은 자주 불러들어 타임 슬라이스를 낮춘다. 반면에 낮은 작업은 높은 작업의 실행 시간에 비례한 균형을 맞추기 위해 타임 슬라이스를 의도적으로 늘려 일을 무사히 완수하게 만든다. 이런 방법으로 시스템의 효율을 유지한다.

## 프로세스 동기화

1. 상태 변회를 살펴보기 위해 반복문을 무한 실행하며 기다리는 것을 무엇이라 하는가?
   - 바쁜 대기
2. 프로세스 간 통신에서 대기가 없는 통신과 대기가 있는 통신의 예를 각각 제시하시오
   - 파일 입출력 : 대기가 없어 `wait()` 로 처리
   - 파이프 : 프로세스 간 통신
3. 파이프를 이용하여 통신할 때 파이프를 2개 사용하는 이유는 무엇인가
   - 파이프는 단방향 통신이다. 따라서 읽기/쓰기 통로를 따로 둬야 한다.
4. 공유 자원의 접근 순서에 따라 실행 결과가 달라지는 프로그램의 영역은 무엇인7W
   - 임계구역
5. 임계구역 해결 조건 중 한 프로세스가 임계구역에 들어갔을 때 다른 프로세스는 임계구역에 들어 갈 수 없는 조건을 무엇이라 히는가
   - 상호 배제 조건
6. 임계구역 해결 조건 중 한 프로세스가 다른 프로세스의 진행을 방해해서는 안 된디는 조건을 무엇이 라 하는가?
   - 한정 대기 조건
7. 임계구역 문제를 하드웨어적으로 해결한 방식으로, 하드웨어의 지원을 받아 명령어를 실행 하는 도중에 타임이웃이 걸리지 않도록 하는 방식을 무엇이라 하는가?
   - 검사와 지정 명령을 같이 실행 : `while(testandset(&lock)==true)`
8. 세마포어 내부 변수를 RS라고 할 때 세마포어 `P()`와 `V()`의 내부 코드를 쓰시오

```
fun P() {
    if RS>0 then RS -= 1;
    else block()
}
fun V() {
    RS += 1
    wake_up()
}
```

9. 세마포어가 제대로 작동하지 않은 경우를 설명하시오.
10. 세마포어의 내부 코드도 타임아웃이 걸리면 문제가 발생할 수도 있다. 그래서 내부 코드는 무엇으로 보호받는가?
11. 공유 자원을 내부적으로 숨기고 공유 자원에 접근하기 위한 인터페이스만 제공힘으로써 자 원을 보호하고 프로세스 간에 동기화를 시 키는 것으로, 세마포어의 단점을 해결하면서 임계 구역 문제를 해결한 방식은 무엇인가?
    - 모니터
12. 파일을 이용하여 Test라는 문자를 주고 받는 코드를 작성하시오

### 임계구역 해결 알고리즘

- 피터슨
  _ `turn 1 or 2`
  _ 2개의 프로세스만 사용이 가능하다.

- 데커 알고리즘 - 피터슨과 비슷하다 - 다만 더 명시적인 처리로 상호 베제를 예방한다. - 2개의 프로세스만 사용 가능한 것 같다.

두 프로세스가 동시에 들어가 임계구역이 의도치 않게 오염될 수 있음.

융통성 문제, 어떤 프로세스가 락을 바꾼 뒤 또 다른 프로세스의 확인까지의 시간이 비효율적이다. 해결책으로 검사와 지정 명령을 동시에 하는 법이 있다.

```c
if (pid<0 || fd<0) exit(-1);
else if (pid==0) {
    write(fd, "Test", 5);
    close(fd);
    exit(0);
} else {
    wait(0);
    lseek(fd, 0, SEEK_SET);
    // lseek(fd, -5, SEEK_CUR);
    read(fd, buf, 5);
    printf('%s', buf);
    close(fd);
    exit(0);
}
```