| 번호   | 제목                                                          | 스크립트 |
|--------|-------------------------------------------------------------|--------------------|
|  |   **오라클 구조**                                                  |                  |
| 1    | 오라클 데이터 베이스의 구조를 제일 처음 알아야해요                        |                  |
| 2    | 오라클 데이터 베이스 서버 구조 : 개요                                  |                  |
| 3    | 오라클 데이터베이스 메모리 구조                                      |                  |
| 4    | shared pool                                                 |                  |
| 5    | 데이터베이스 버퍼 캐쉬(database buffer cache)                         |                  |
| 6    | 리두로그 버퍼(redo log buffer)                                     |                  |
| 7    | PGA 메모리 영역                                               |                  |
| 8    | DBWn 프로세서                                                |                  |
| 9    | LGWR (log writer)                                           |                  |
| 10   | CKPT (checkpoint process)                                    |                  |
| 11   | SMON(System Monitor process)                                 |                  |
| 12   | PMON 프로세서 (Process monitor)                              |                  |
| 13   | ARCn (Archive process)                                       |                  |
|   | **저장 영역 구조**                                                |                  |
| 14   | 데이터 베이스 저장 영역 구조                                          |                  |
| 15   | 논리적 및 물리적 데이터 베이스 구조                                      |                  |
|    | **startup 단계와 shutdown 옵션**                                |                  |
| 16   | startup 의 4가지 단계를 알아야 해요!                                   |                  |
| 17   | database 종료 모드 4가지를 알고 있어야 해요.                            |                  |
|    | **파라미터 파일 관리**                                            |                  |
| 18   | dba는 초기화 파라미터 관리를 잘 할 줄 알아야 해요.                        |                  |
| 19   | 파라미터 값을 alter system 명령어로 변경하는 것과 alter session 명령어로 변경하는 것의 차이를 알아야 해요. |                  |
|    | **테이블 스페이스 관리**                                          |                  |
| 20   | 테이블 스페이스 생성과 관리에 대한 A4지 한장이 머리속에 있어야해요            |                  |
| 21   | 데이터를 저장하기 위한 첫걸음 !  테이블 스페이스 생성                      |                  |
| 22   | 테이블 스페이스를 삭제할 때는 이 옵션을 알아야해요.                        |                  |
| 23   | default tablespace 가 뭔지 알고 있어야합니다.                       |                  |
| 24   | 테이블 스페이스에 공간이 꽉차면 공간을 추가할 줄 알아야해요.                  |                  |
| 25   | 과도한 정렬 작업을 위해서는 Temporary tablespace 를 잘 이해하고 있어야합니다. |                  |
| 26   | 과도한 DML 작업이 성공적으로 수행되려면 undo tablespace 를 잘 이해하고 있어야해요 |                  |
| 27   | 만약 data file 이름을 변경하거나 다른 위치로 이동하고 싶다면 테이블 스페이스를 offline 시킬 줄 알아야 되요. |                  |
| 28   | 테이블 스페이스의 세그먼트 관리 방법을 알아야해요.                        |                  |
| 29   | OMF(Oracle Managed File) 이 뭔지 알아야해요 !                        |                  |
| 30   | 테이블 스페이스 생성시 extent 관리 방법을 알아야해요.                      |                  |
| 31   | bigfile tablespace 가 뭔지 알아야해요                                 |                  |
|     | **언두 테이블 스페이스 관리**                                      |                  |
| 32   | undo data 가 무엇인지 알고 있어야해요.                                   |                  |
| 33   | undo data 와 redo data 를 서로 다른거예요.                                |                  |
| 34   | 언두 data 관리는 자동으로 되고 있어요.                                  |                  |
| 35   | undo_retention 을 1시간으로 변경했다고 해서 그것을 확실히 보장하지는 않아요 |                  |
| 36   | ORA-01555 snap shot too old 에러가 뭔지 알고 있어야 해요                 |                  |
|    | **오라클 네트워크 관리**                                           |                  |
| 37   | 오라클에 접속하려면 4가지 정보를 알아야 해요                           |                  |
| 38   | sqldeveloper 나 dbever 로 오라클에 접속하려면 리스너 통해서 접속해야해요.    |                  |
| 39   | 오라클 네트워크를 다루는 관리 도구가 4가지가 있습니다.                     |                  |
| 40   | listener.ora 파일의 위치가 어디에 있는지 알아야 합니다.                 |                  |
| 41   | 오라클 서버에 접속하는 방식은 총 4가지가 있습니다.                       |                  |
| 42   | 오라클에 접속 안될때 확인하는 방법 3가지를 알고 있어야해요.                  |                  |
|    | **유져관리**                                                      |                  |
| 43   | 유져 생성시 상세한 옵션들을 dba 는 알고 있어야해요.                         |                  |
| 44   | 유져를 생성하기 위해서 유져 인증 방법 3가지를 알고 있어야해요.                |                  |
| 45   | 오라클 db 를 올렸다 내렸다 할 수 있는 권한 관리가 2가지가 있어요.             |                  |
| 46   | 보안을 강화 하기 위해서 유져를 잠그거나 암호를 자주 변경해야해요.             |                  |
| 47   | 오라클의 권한의 종류는 크게 2가지가 있어요.                              |                  |
| 48   | 내가 받은 시스템 권한을 남에게 주려면 with admin option을 알아야해요         |                  |
| 49   | 객체권한을 남에게 줄 수 있는 권한까지 같이 주려면 with grant option을 알아야해요 |                  |
| 50   | 롤(role)을 사용하게 되면 편하게 권한 부여를 할 수 있습니다.                   |                  |
|  | **리소스 메니져**                                                 |                  |
| 51   | 특정 세션이 오라클의 자원을 무한히 사용하지 못하게 해야 해요.                 |                  |
| 52   | resource manager 로 cpu 사용을 제한해볼 수 있어야해요.                     |                  |
| 53   | 리소스 메니져를 이용해서 병렬도를 제한하기                               |                  |
| 54   | 리소스 메니져를 이용해서 악성 sql 이 수행 안되게 설정하기                    |                  |
|  | **데이터 이행**                                                   |                  |
| 55   | 데이터를 이행하는 3가지 방법을 알아야 해요                             |                  |
| 56   | 서브쿼리를 사용한 insert 문의 속도를 높이는 방법을 알아야해요.              |                  |
| 57   | High water mark 위에 데이터를 넣을때 병렬로 작업하면 더 빠르게 데이터를 입력할 수 있어요. |                  |
| 58   | 대용량 csv 파일을 오라클 데이터 베이스로 로드할 때는 SQL*Loader 를 쓰세요.    |                  |
| 59   | 테이블 생성 스크립트를 추출할 줄 알아야해요                           |                  |
| 60   | export / import 이용해서 데이터 이행을 할 줄 알아야해요                  |                  |
| 61   | 유져 레벨로 export /import 를 할줄 알아야해요.                          |                  |
| 62   | tablespace level 로 export/import 를 할 줄 알아야해요                   |                  |
| 63   | database 를 통채로 export/import 를 할 수 있어요.                      |                  |
| 64   | export/import 보다 더 업그레이드 되어진 data pump 를 알아야 해요          |                  |
| 65   | 현업에서 가장 많이 쓰는 유져 레벨 pump 를 사용할 수 있어야해요          |                  |
| 66   | 한번에 데이터 이관을 끝내는 테이블 스페이스 레벨 펌프 사용법            |                  |
| 67   | 고수들이 데이터 이행 하는 방법은 이렇습니다.                           |                  |
| 68   | 외부 테이블을 생성할 줄 알아야해요.                                 |                  |
| 69   | pump 를 엔진으로 해서 외부 테이블을 생성할 줄 알아야해요.                 |                  |
|  | **DB reorg 작업하기**                                             |                  |
| 70   | db reorg 작업하기             |                  |
