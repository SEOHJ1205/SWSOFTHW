
# 리눅스 프로세스 관리 명령어

리눅스 시스템에서 프로세스를 관리하는데 사용하는 `top`, `ps`, `jobs`, `kill` 명령어를 설명합니다.

![panda](https://cdn-1.webcatalog.io/catalog/write-panda/write-panda-icon-filled-256.png?v=1693685228013)

---

## `top`

`top` 명령어는 시스템의 프로세스를 실시간으로 보여줍니다.

**용도:** 시스템의 CPU와 메모리 사용량을 모니터링하고, 현재 실행 중인 프로세스를 확인할 때 사용합니다.

**사용법:**

bash
top


## `ps`

`ps` 명령어는 현재 실행 중인 프로세스의 목록을 보여줍니다.

**용도:** 현재 실행 중인 프로세스를 확인하고, 특정 프로세스의 상태를 조사할 때 사용합니다.

**사용법:**

bash
ps [옵션]

**예시:**

bash
ps aux

---

## `jobs`

`jobs` 명령어는 현재 쉘 세션에서 실행된 리스트를 보여줍니다.

**용도:** 백그라운드 작업의 상태를 확인할 때 사용합니다.

**사용법:**

bash
jobs [옵션]

**예시:**

bash
jobs -l

---

## `kill`

`kill` 명령어는 프로세스를 종료할 때 사용합니다.

**용도:** 특정 프로세스를 종료하거나 신호를 보낼 때 사용합니다.

**사용법:**

bash
kill [옵션] <PID>

**예시:**

bash
kill -9 1234

**주요 신호:**

| 신호        | 설명                          |
|-------------|-------------------------------|
| `-SIGTERM` (15) | 프로세스를 정상 종료 요청 (기본값)  |
| `-SIGKILL` (9)  | 프로세스를 강제 종료               |
| `-SIGSTOP`      | 프로세스를 일시 중지               |
| `-SIGCONT`      | 일시 중지된 프로세스 재개          |

