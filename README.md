# 오라클 관리 수업 가이드

<img src="https://github.com/oracleyu01/oracle_admin/blob/main/%EC%98%A4%EB%9D%BC%ED%81%B4-%EA%B4%80%EB%A6%AC-%EC%88%98%EC%97%85-001.png" width="400" height="400">

안녕하세요,  여러분! 🌟



오라클 dba와 오라클 엔지니어를 준비하시는 여러분들을 위해 오라클 관리 스크립트를 정리하였습니다.


## 시작하는 법


아래의 내용을 순서데로 보시면 됩니다.

## 수업 자료 ( ☀️ 2024년 3월 29일 updated)


### 1. **오라클 구조**

- 1.1 **오라클 데이터 베이스 서버 구조를 알아야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/1.1%20%EC%98%A4%EB%9D%BC%ED%81%B4%20%EB%8D%B0%EC%9D%B4%ED%84%B0%20%EB%B2%A0%EC%9D%B4%EC%8A%A4%20%EC%84%9C%EB%B2%84%EC%9D%98%20%EA%B5%AC%EC%A1%B0%EB%A5%BC%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.md)] 
- 1.2 **오라클 데이터베이스 메모리 구조를 알아야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/1.2%20%EC%98%A4%EB%9D%BC%ED%81%B4%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4%20%EB%A9%94%EB%AA%A8%EB%A6%AC%20%EA%B5%AC%EC%A1%B0%EB%A5%BC%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94..txt)]

- 1.3 **공유풀(shared pool)이 왜 필요한지 알아야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/1.3%20%EA%B3%B5%EC%9C%A0%ED%92%80(shared%20pool)%EC%9D%B4%20%EC%99%9C%20%ED%95%84%EC%9A%94%ED%95%9C%EC%A7%80%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94..txt)]

- 1.4 **데이터베이스 버퍼 캐쉬(database buffer cache) 가 왜 필요한지 알아야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4%20%EB%B2%84%ED%8D%BC%20%EC%BA%90%EC%89%AC(database%20buffer%20cache)%20%EA%B0%80%20%EC%99%9C%20%ED%95%84%EC%9A%94%ED%95%9C%EC%A7%80%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 1.5 **리두로그 버퍼(redo log buffer) 가 왜 필요한지 알아야해요.**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/%EB%A6%AC%EB%91%90%EB%A1%9C%EA%B7%B8%20%EB%B2%84%ED%8D%BC(redo%20log%20buffer)%20%EA%B0%80%20%EC%99%9C%20%ED%95%84%EC%9A%94%ED%95%9C%EC%A7%80%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 1.6 **PGA 메모리 영역이 왜 필요한지 알아야해요.**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/edit/main/1.6%20%20PGA%20%EB%A9%94%EB%AA%A8%EB%A6%AC%20%EC%98%81%EC%97%AD.txt)]

- 1.7 **DBWn 프로세서의 역할을 알아야해요.**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/1.7%20DBWn%20%ED%94%84%EB%A1%9C%EC%84%B8%EC%84%9C(%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4%20%EA%B8%B0%EB%A1%9D%EC%9E%90%20%ED%94%84%EB%A1%9C%EC%84%B8%EC%84%9C.txt ) ]

- 1.8 **LGWR (log writer)의 역할을 알아야해요.**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/1.8.%20LGWR%20%EC%9D%98%20%EC%97%AD%ED%99%9C%EC%9D%84%20%EC%95%8C%EC%95%84%EC%95%A0%ED%95%B4%EC%9A%94.txt)]

- 1.9 **CKPT (checkpoint process)의 역할을 알아야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/1.9%20%20CKPT%20%EC%9D%98%20%EC%97%AD%ED%99%9C%EC%9D%84%20%EC%95%8C%EC%95%84%EC%95%BC%20%ED%95%B4%EC%9A%94.txt)]

- 1.10 **SMON(System Monitor process)의 역할을 알아야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/1.10%20SMON%20%EC%9D%98%20%EC%97%AD%ED%99%9C%EC%9D%84%20%EC%95%8C%EC%95%84%EC%95%BC%20%ED%95%B4%EC%9A%94.txt)]

- 1.11 **PMON 프로세서 (Process monitor)의 역할을 알아야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/1.10%20%20PMON%20%ED%94%84%EB%A1%9C%EC%84%B8%EC%84%9C%EC%9D%98%20%EC%97%AD%ED%99%9C%EC%9D%84%20%EC%95%8C%EC%95%84%EC%95%BC%20%ED%95%B4%EC%9A%94.txt)]

- 1.12 **ARCn (Archive process)의 역할을 알아야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/1.12%20ARCn%20(Archive%20process)%EC%9D%98%20%EC%97%AD%ED%95%A0%EC%9D%84%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94..txt)]


### 2. **저장 영역 구조**

- 2.1 **데이터 베이스 저장 영역 구조**: [📄   [노트](https://github.com/oracleyu01/oracle_admin/blob/main/2.1%20%EB%8D%B0%EC%9D%B4%ED%84%B0%20%EB%B2%A0%EC%9D%B4%EC%8A%A4%20%EC%A0%80%EC%9E%A5%20%EC%98%81%EC%97%AD%20%EA%B5%AC%EC%A1%B0.txt)]

- 2.2 **논리적 및 물리적 데이터 베이스 구조**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/2.2%20%EB%85%BC%EB%A6%AC%EC%A0%81%20%EB%B0%8F%20%EB%AC%BC%EB%A6%AC%EC%A0%81%20%EB%8D%B0%EC%9D%B4%ED%84%B0%20%EB%B2%A0%EC%9D%B4%EC%8A%A4%20%EA%B5%AC%EC%A1%B0.txt)]


### 3. **startup 단계와 shutdown 옵션**

- 3.1 **startup 의 4가지 단계를 알아야 해요!**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/3.1%20startup%20%EC%9D%98%204%EA%B0%80%EC%A7%80%20%EB%8B%A8%EA%B3%84%EB%A5%BC%20%EC%95%8C%EC%95%84%EC%95%BC%20%ED%95%B4%EC%9A%94.txt)]

- 3.2 **database 종료 모드 4가지를 알고 있어야 해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/3.2%20database%20%EC%A2%85%EB%A3%8C%20%EB%AA%A8%EB%93%9C%204%EA%B0%80%EC%A7%80%EB%A5%BC%20%EC%95%8C%EA%B3%A0%20%EC%9E%88%EC%96%B4%EC%95%BC%20%ED%95%B4%EC%9A%94.txt)]


### 4. **파라미터 파일 관리**

- 4.1 **dba는 초기화 파라미터 관리를 잘 할 줄 알아야 해요.**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/4.1%20dba%EB%8A%94%20%EC%B4%88%EA%B8%B0%ED%99%94%20%ED%8C%8C%EB%9D%BC%EB%AF%B8%ED%84%B0%20%EA%B4%80%EB%A6%AC%EB%A5%BC%20%EC%9E%98%20%ED%95%A0%20%EC%A4%84%20%EC%95%8C%EC%95%84%EC%95%BC%20%ED%95%B4%EC%9A%94.txt)]

- 4.2 **alter system 과 alter session 의 차이는 ?**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/4.2%20alter%20system%20%EA%B3%BC%20alter%20session%20%EC%9D%98%20%EC%B0%A8%EC%9D%B4%EB%8A%94.txt)]


### 5. **테이블 스페이스 관리**

- 5.1 **테이블 스페이스 생성과 관리에 대한 A4지 한장이 머리속에 있어야해요**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/5.1%20%ED%85%8C%EC%9D%B4%EB%B8%94%20%EC%8A%A4%ED%8E%98%EC%9D%B4%EC%8A%A4%20%EC%83%9D%EC%84%B1%EA%B3%BC%20%EA%B4%80%EB%A6%AC%EC%97%90%20%EB%8C%80%ED%95%9C%20A4%EC%A7%80%20%ED%95%9C%EC%9E%A5%EC%9D%B4%20%EB%A8%B8%EB%A6%AC%EC%86%8D%EC%97%90%20%EC%9E%88%EC%96%B4%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 5.2 **데이터를 저장하기 위한 첫걸음 !  테이블 스페이스 생성**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/5.2%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%A5%BC%20%EC%A0%80%EC%9E%A5%ED%95%98%EA%B8%B0%20%EC%9C%84%ED%95%9C%20%EC%B2%AB%EA%B1%B8%EC%9D%8C%20!%20%ED%85%8C%EC%9D%B4%EB%B8%94%20%EC%8A%A4%ED%8E%98%EC%9D%B4%EC%8A%A4%20%EC%83%9D%EC%84%B1.txt)]

- 5.3 **테이블 스페이스를 삭제할 때는 이 옵션을 알아야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/5.3%20%ED%85%8C%EC%9D%B4%EB%B8%94%20%EC%8A%A4%ED%8E%98%EC%9D%B4%EC%8A%A4%EB%A5%BC%20%EC%82%AD%EC%A0%9C%ED%95%A0%20%EB%95%8C%EB%8A%94%20%EC%9D%B4%20%EC%98%B5%EC%85%98%EC%9D%84%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 5.4 **default tablespace 가 뭔지 알고 있어야합니다.**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/5.4%20default%20tablespace%20%EA%B0%80%20%EB%AD%94%EC%A7%80%20%EC%95%8C%EA%B3%A0%20%EC%9E%88%EC%96%B4%EC%95%BC%ED%95%A9%EB%8B%88%EB%8B%A4.txt)]

- 5.5 **테이블 스페이스에 공간이 꽉차면 공간을 추가할 줄 알아야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/5.5%20%ED%85%8C%EC%9D%B4%EB%B8%94%20%EC%8A%A4%ED%8E%98%EC%9D%B4%EC%8A%A4%EC%97%90%20%EA%B3%B5%EA%B0%84%EC%9D%B4%20%EA%BD%89%EC%B0%A8%EB%A9%B4%20%EA%B3%B5%EA%B0%84%EC%9D%84%20%EC%B6%94%EA%B0%80%ED%95%A0%20%EC%A4%84%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 5.6 **과도한 정렬 작업을 위해서는 Temporary tablespace 를 잘 이해하고 있어야합니다.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/5.6%20%EA%B3%BC%EB%8F%84%ED%95%9C%20%EC%A0%95%EB%A0%AC%20%EC%9E%91%EC%97%85%EC%9D%84%20%EC%9C%84%ED%95%B4%EC%84%9C%EB%8A%94%20Temporary%20tablespace%20%EB%A5%BC%20%EC%9E%98%20%EC%9D%B4%ED%95%B4%ED%95%98%EA%B3%A0%20%EC%9E%88%EC%96%B4%EC%95%BC%ED%95%A9%EB%8B%88%EB%8B%A4.txt)]

- 5.7 **과도한 DML 작업이 성공적으로 수행되려면 undo tablespace 를 잘 이해하고 있어야해요**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/5.7%20%EA%B3%BC%EB%8F%84%ED%95%9C%20DML%20%EC%9E%91%EC%97%85%EC%9D%B4%20%EC%84%B1%EA%B3%B5%EC%A0%81%EC%9C%BC%EB%A1%9C%20%EC%88%98%ED%96%89%EB%90%98%EB%A0%A4%EB%A9%B4%20undo%20tablespace%20%EB%A5%BC%20%EC%9E%98%20%EC%9D%B4%ED%95%B4%ED%95%98%EA%B3%A0%20%EC%9E%88%EC%96%B4%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 5.8 **만약 data file 이름을 변경하거나 다른 위치로 이동하고 싶다면?**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/5.8%20%EB%A7%8C%EC%95%BD%20data%20file%20%EC%9D%B4%EB%A6%84%EC%9D%84%20%EB%B3%80%EA%B2%BD%ED%95%98%EA%B1%B0%EB%82%98%20%EB%8B%A4%EB%A5%B8%20%EC%9C%84%EC%B9%98%EB%A1%9C%20%EC%9D%B4%EB%8F%99%ED%95%98%EA%B3%A0%20%EC%8B%B6%EB%8B%A4%EB%A9%B4.txt)]

- 5.9 **테이블 스페이스의 세그먼트 관리 방법을 알아야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/5.9%20%ED%85%8C%EC%9D%B4%EB%B8%94%20%EC%8A%A4%ED%8E%98%EC%9D%B4%EC%8A%A4%EC%9D%98%20%EC%84%B8%EA%B7%B8%EB%A8%BC%ED%8A%B8%20%EA%B4%80%EB%A6%AC%20%EB%B0%A9%EB%B2%95%EC%9D%84%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 5.10 **OMF(Oracle Managed File) 이 뭔지 알아야해요 !**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/5.10%20OMF(Oracle%20Managed%20File)%20%EC%9D%B4%20%EB%AD%94%EC%A7%80%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 5.11 **테이블 스페이스 생성시 extent 관리 방법을 알아야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/5.11%20%ED%85%8C%EC%9D%B4%EB%B8%94%20%EC%8A%A4%ED%8E%98%EC%9D%B4%EC%8A%A4%20%EC%83%9D%EC%84%B1%EC%8B%9C%20extent%20%EA%B4%80%EB%A6%AC%20%EB%B0%A9%EB%B2%95%EC%9D%84%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94..txt)]

- 5.12 **bigfile tablespace 가 뭔지 알아야해요**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/5.12%20bigfile%20tablespace%20%EA%B0%80%20%EB%AD%94%EC%A7%80%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)]


### 6. **언두 테이블 스페이스 관리**

- 6.1 **undo data 가 무엇인지 알고 있어야해요.**: [📄   [노트](https://github.com/oracleyu01/oracle_admin/blob/main/6.1%20undo%20data%20%EA%B0%80%20%EB%AC%B4%EC%97%87%EC%9D%B8%EC%A7%80%20%EC%95%8C%EA%B3%A0%20%EC%9E%88%EC%96%B4%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 6.2 **undo data 와 redo data 를 서로 다른거예요.**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/6.2%20undo%20data%20%EC%99%80%20redo%20data%20%EB%A5%BC%20%EC%84%9C%EB%A1%9C%20%EB%8B%A4%EB%A5%B8%EA%B1%B0%EC%98%88%EC%9A%94.txt)]

- 6.3 **언두 data 관리는 자동으로 되고 있어요.**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/6.3%20%EC%96%B8%EB%91%90%20data%20%EA%B4%80%EB%A6%AC%EB%8A%94%20%EC%9E%90%EB%8F%99%EC%9C%BC%EB%A1%9C%20%EB%90%98%EA%B3%A0%20%EC%9E%88%EC%96%B4%EC%9A%94..txt)]

- 6.4 **undo_retention 을 1시간으로 변경했다고 해서 그것을 확실히 보장하지는 않아요**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/6.4%20undo_retention%20%EC%9D%84%201%EC%8B%9C%EA%B0%84%EC%9C%BC%EB%A1%9C%20%EB%B3%80%EA%B2%BD%ED%96%88%EB%8B%A4%EA%B3%A0%20%ED%95%B4%EC%84%9C%20%EA%B7%B8%EA%B2%83%EC%9D%84%20%ED%99%95%EC%8B%A4%ED%9E%88%20%EB%B3%B4%EC%9E%A5%ED%95%98%EC%A7%80%EB%8A%94%20%EC%95%8A%EC%95%84%EC%9A%94.txt)]

- 6.5 **ORA-01555 snap shot too old 에러가 뭔지 알고 있어야 해요**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/6.5%20ORA-01555%20snap%20shot%20too%20old%20%EC%97%90%EB%9F%AC%EA%B0%80%20%EB%AD%94%EC%A7%80%20%EC%95%8C%EA%B3%A0%20%EC%9E%88%EC%96%B4%EC%95%BC%20%ED%95%B4%EC%9A%94.txt)]


### 7. **오라클 네트워크 관리**

- 7.1 **오라클에 접속하려면 4가지 정보를 알아야 해요**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/7.1%20%EC%98%A4%EB%9D%BC%ED%81%B4%EC%97%90%20%EC%A0%91%EC%86%8D%ED%95%98%EB%A0%A4%EB%A9%B4%204%EA%B0%80%EC%A7%80%20%EC%A0%95%EB%B3%B4%EB%A5%BC%20%EC%95%8C%EC%95%84%EC%95%BC%20%ED%95%B4%EC%9A%94.txt)]

- 7.2 **sqldeveloper 나 dbever 로 오라클에 접속하려면 리스너 통해서 접속해야해요.**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/7.2%20sqldeveloper%20%EB%82%98%20dbever%20%EB%A1%9C%20%EC%98%A4%EB%9D%BC%ED%81%B4%EC%97%90%20%EC%A0%91%EC%86%8D%ED%95%98%EB%A0%A4%EB%A9%B4%20%EB%A6%AC%EC%8A%A4%EB%84%88%20%ED%86%B5%ED%95%B4%EC%84%9C%20%EC%A0%91%EC%86%8D%ED%95%B4%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 7.3 **오라클 네트워크를 다루는 관리 도구가 4가지가 있습니다.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/7.3%20%EC%98%A4%EB%9D%BC%ED%81%B4%20%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC%EB%A5%BC%20%EB%8B%A4%EB%A3%A8%EB%8A%94%20%EA%B4%80%EB%A6%AC%20%EB%8F%84%EA%B5%AC%EA%B0%80%204%EA%B0%80%EC%A7%80%EA%B0%80%20%EC%9E%88%EC%8A%B5%EB%8B%88%EB%8B%A4.txt)]

- 7.4 **listener.ora 파일의 위치가 어디에 있는지 알아야 합니다.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/7.4%20listener.ora%20%ED%8C%8C%EC%9D%BC%EC%9D%98%20%EC%9C%84%EC%B9%98%EA%B0%80%20%EC%96%B4%EB%94%94%EC%97%90%20%EC%9E%88%EB%8A%94%EC%A7%80%20%EC%95%8C%EC%95%84%EC%95%BC%20%ED%95%A9%EB%8B%88%EB%8B%A4.txt)]

- 7.5 **오라클 서버에 접속하는 방식은 총 4가지가 있습니다.**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/7.5%20%EC%98%A4%EB%9D%BC%ED%81%B4%20%EC%84%9C%EB%B2%84%EC%97%90%20%EC%A0%91%EC%86%8D%ED%95%98%EB%8A%94%20%EB%B0%A9%EC%8B%9D%EC%9D%80%20%EC%B4%9D%204%EA%B0%80%EC%A7%80%EA%B0%80%20%EC%9E%88%EC%8A%B5%EB%8B%88%EB%8B%A4.txt)]

- 7.6 **오라클에 접속 안될때 확인하는 방법 3가지를 알고 있어야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/7.6%20%EC%98%A4%EB%9D%BC%ED%81%B4%EC%97%90%20%EC%A0%91%EC%86%8D%20%EC%95%88%EB%90%A0%EB%95%8C%20%ED%99%95%EC%9D%B8%ED%95%98%EB%8A%94%20%EB%B0%A9%EB%B2%95%203%EA%B0%80%EC%A7%80%EB%A5%BC%20%EC%95%8C%EA%B3%A0%20%EC%9E%88%EC%96%B4%EC%95%BC%ED%95%B4%EC%9A%94.txt)]


### 8. **유져관리**

- 8.1 **유져 생성시 상세한 옵션들을 dba 는 알고 있어야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/8.1%20%EC%9C%A0%EC%A0%B8%20%EC%83%9D%EC%84%B1%EC%8B%9C%20%EC%83%81%EC%84%B8%ED%95%9C%20%EC%98%B5%EC%85%98%EB%93%A4%EC%9D%84%20dba%20%EB%8A%94%20%EC%95%8C%EA%B3%A0%20%EC%9E%88%EC%96%B4%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 8.2 **유져를 생성하기 위해서 유져 인증 방법 3가지를 알고 있어야해요.**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/8.2%20%EC%9C%A0%EC%A0%B8%EB%A5%BC%20%EC%83%9D%EC%84%B1%ED%95%98%EA%B8%B0%20%EC%9C%84%ED%95%B4%EC%84%9C%20%EC%9C%A0%EC%A0%B8%20%EC%9D%B8%EC%A6%9D%20%EB%B0%A9%EB%B2%95%203%EA%B0%80%EC%A7%80%EB%A5%BC%20%EC%95%8C%EA%B3%A0%20%EC%9E%88%EC%96%B4%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 8.3 **오라클 db 를 올렸다 내렸다 할 수 있는 권한 관리가 2가지가 있어요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/8.3%20%EC%98%A4%EB%9D%BC%ED%81%B4%20db%20%EB%A5%BC%20%EC%98%AC%EB%A0%B8%EB%8B%A4%20%EB%82%B4%EB%A0%B8%EB%8B%A4%20%ED%95%A0%20%EC%88%98%20%EC%9E%88%EB%8A%94%20%EA%B6%8C%ED%95%9C%20%EA%B4%80%EB%A6%AC%EA%B0%80%202%EA%B0%80%EC%A7%80%EA%B0%80%20%EC%9E%88%EC%96%B4%EC%9A%94.txt)]

- 8.4 **보안을 강화 하기 위해서 유져를 잠그거나 암호를 자주 변경해야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/8.4%20%EB%B3%B4%EC%95%88%EC%9D%84%20%EA%B0%95%ED%99%94%20%ED%95%98%EA%B8%B0%20%EC%9C%84%ED%95%B4%EC%84%9C%20%EC%9C%A0%EC%A0%B8%EB%A5%BC%20%EC%9E%A0%EA%B7%B8%EA%B1%B0%EB%82%98%20%EC%95%94%ED%98%B8%EB%A5%BC%20%EC%9E%90%EC%A3%BC%20%EB%B3%80%EA%B2%BD%ED%95%B4%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 8.5 **오라클의 권한의 종류는 크게 2가지가 있어요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/8.5%20%EC%98%A4%EB%9D%BC%ED%81%B4%EC%9D%98%20%EA%B6%8C%ED%95%9C%EC%9D%98%20%EC%A2%85%EB%A5%98%EB%8A%94%20%ED%81%AC%EA%B2%8C%202%EA%B0%80%EC%A7%80%EA%B0%80%20%EC%9E%88%EC%96%B4%EC%9A%94.txt)]

- 8.6 **내가 받은 시스템 권한을 남에게 주려면 with admin option을 알아야해요**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/8.6%20%EB%82%B4%EA%B0%80%20%EB%B0%9B%EC%9D%80%20%EC%8B%9C%EC%8A%A4%ED%85%9C%20%EA%B6%8C%ED%95%9C%EC%9D%84%20%EB%82%A8%EC%97%90%EA%B2%8C%20%EC%A3%BC%EB%A0%A4%EB%A9%B4%20with%20admin%20option%EC%9D%84%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 8.7 **객체권한을 남에게 줄 수 있는 권한까지 같이 주려면 with grant option을 알아야해요**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/8.7%20%EA%B0%9D%EC%B2%B4%EA%B6%8C%ED%95%9C%EC%9D%84%20%EB%82%A8%EC%97%90%EA%B2%8C%20%EC%A4%84%20%EC%88%98%20%EC%9E%88%EB%8A%94%20%EA%B6%8C%ED%95%9C%EA%B9%8C%EC%A7%80%20%EA%B0%99%EC%9D%B4%20%EC%A3%BC%EB%A0%A4%EB%A9%B4%20with%20grant%20option%EC%9D%84%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 8.8 **롤(role)을 사용하게 되면 편하게 권한 부여를 할 수 있습니다.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/8.8%20%EB%A1%A4(role)%EC%9D%84%20%EC%82%AC%EC%9A%A9%ED%95%98%EA%B2%8C%20%EB%90%98%EB%A9%B4%20%ED%8E%B8%ED%95%98%EA%B2%8C%20%EA%B6%8C%ED%95%9C%20%EB%B6%80%EC%97%AC%EB%A5%BC%20%ED%95%A0%20%EC%88%98%20%EC%9E%88%EC%8A%B5%EB%8B%88%EB%8B%A4.txt)]


### 9. **리소스 메니져**

- 9.1 **특정 세션이 오라클의 자원을 무한히 사용하지 못하게 해야 해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/9.1%20%ED%8A%B9%EC%A0%95%20%EC%84%B8%EC%85%98%EC%9D%B4%20%EC%98%A4%EB%9D%BC%ED%81%B4%EC%9D%98%20%EC%9E%90%EC%9B%90%EC%9D%84%20%EB%AC%B4%ED%95%9C%ED%9E%88%20%EC%82%AC%EC%9A%A9%ED%95%98%EC%A7%80%20%EB%AA%BB%ED%95%98%EA%B2%8C%20%ED%95%B4%EC%95%BC%20%ED%95%B4%EC%9A%94.txt)]

- 9.2 **resource manager 로 cpu 사용을 제한해볼 수 있어야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/9.2%20resource%20manager%20%EB%A1%9C%20cpu%20%EC%82%AC%EC%9A%A9%EC%9D%84%20%EC%A0%9C%ED%95%9C%ED%95%B4%EB%B3%BC%20%EC%88%98%20%EC%9E%88%EC%96%B4%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 9.3 **리소스 메니져를 이용해서 병렬도를 제한하기**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/9.3%20%EB%A6%AC%EC%86%8C%EC%8A%A4%20%EB%A9%94%EB%8B%88%EC%A0%B8%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%B4%EC%84%9C%20%EB%B3%91%EB%A0%AC%EB%8F%84%EB%A5%BC%20%EC%A0%9C%ED%95%9C%ED%95%98%EA%B8%B0.txt)]

- 9.4 **리소스 메니져를 이용해서 악성 sql 이 수행 안되게 설정하기**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/9.4%20%EB%A6%AC%EC%86%8C%EC%8A%A4%20%EB%A9%94%EB%8B%88%EC%A0%B8%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%B4%EC%84%9C%20%EC%95%85%EC%84%B1%20sql%20%EC%9D%B4%20%EC%88%98%ED%96%89%20%EC%95%88%EB%90%98%EA%B2%8C%20%EC%84%A4%EC%A0%95%ED%95%98%EA%B8%B0.txt)]


### 10. **데이터 이행**

- 10.1 **데이터를 이행하는 3가지 방법을 알아야 해요**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/10.1%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%A5%BC%20%EC%9D%B4%ED%96%89%ED%95%98%EB%8A%94%203%EA%B0%80%EC%A7%80%20%EB%B0%A9%EB%B2%95%EC%9D%84%20%EC%95%8C%EC%95%84%EC%95%BC%20%ED%95%B4%EC%9A%94.txt)]

- 10.2 **서브쿼리를 사용한 insert 문의 속도를 높이는 방법을 알아야해요.**: [📄[노트](https://github.com/oracleyu01/oracle_admin/blob/main/10.2%20%EC%84%9C%EB%B8%8C%EC%BF%BC%EB%A6%AC%EB%A5%BC%20%EC%82%AC%EC%9A%A9%ED%95%9C%20insert%20%EB%AC%B8%EC%9D%98%20%EC%86%8D%EB%8F%84%EB%A5%BC%20%EB%86%92%EC%9D%B4%EB%8A%94%20%EB%B0%A9%EB%B2%95%EC%9D%84%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 10.3 **High water mark 위에 데이터를 넣을때 병렬로 작업하면 더 빠르게 데이터를 입력할 수 있어요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/10.3%20High%20water%20mark%20%EC%9C%84%EC%97%90%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%A5%BC%20%EB%84%A3%EC%9D%84%EB%95%8C%20%EB%B3%91%EB%A0%AC%EB%A1%9C%20%EC%9E%91%EC%97%85%ED%95%98%EB%A9%B4%20%EB%8D%94%20%EB%B9%A0%EB%A5%B4%EA%B2%8C%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%A5%BC%20%EC%9E%85%EB%A0%A5%ED%95%A0%20%EC%88%98%20%EC%9E%88%EC%96%B4%EC%9A%94..txt)]

- 10.4 **대용량 csv 파일을 오라클 데이터 베이스로 로드할 때는 SQL*Loader 를 쓰세요.**: [📄[노트](https://github.com/oracleyu01/oracle_admin/blob/main/10.4%20%EB%8C%80%EC%9A%A9%EB%9F%89%20csv%20%ED%8C%8C%EC%9D%BC%EC%9D%84%20%EC%98%A4%EB%9D%BC%ED%81%B4%20%EB%8D%B0%EC%9D%B4%ED%84%B0%20%EB%B2%A0%EC%9D%B4%EC%8A%A4%EB%A1%9C%20%EB%A1%9C%EB%93%9C%ED%95%A0%20%EB%95%8C%EB%8A%94%20SQL%20Loader%20%EB%A5%BC%20%EC%93%B0%EC%84%B8%EC%9A%94.txt)]

- 10.5 **테이블 생성 스크립트를 추출할 줄 알아야해요**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/10.5%20%ED%85%8C%EC%9D%B4%EB%B8%94%20%EC%83%9D%EC%84%B1%20%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8%EB%A5%BC%20%EC%B6%94%EC%B6%9C%ED%95%A0%20%EC%A4%84%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 10.6 **export / import 이용해서 데이터 이행을 할 줄 알아야해요**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/10.6%20export%20%20import%20%EC%9D%B4%EC%9A%A9%ED%95%B4%EC%84%9C%20%EB%8D%B0%EC%9D%B4%ED%84%B0%20%EC%9D%B4%ED%96%89%EC%9D%84%20%ED%95%A0%20%EC%A4%84%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 10.7 **유져 레벨로 export /import 를 할줄 알아야해요.**: [📄[노트](https://github.com/oracleyu01/oracle_admin/blob/main/10.7%20%EC%9C%A0%EC%A0%B8%20%EB%A0%88%EB%B2%A8%EB%A1%9C%20export%20import%20%EB%A5%BC%20%ED%95%A0%EC%A4%84%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94..txt)]

- 10.8 **tablespace level 로 export/import 를 할 줄 알아야해요**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/10.8%20tablespace%20level%20%EB%A1%9C%20export%20import%20%EB%A5%BC%20%ED%95%A0%20%EC%A4%84%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 10.9 **database 를 통채로 export/import 를 할 수 있어요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/10.9%20database%20%EB%A5%BC%20%ED%86%B5%EC%B1%84%EB%A1%9C%20export%20import%20%EB%A5%BC%20%ED%95%A0%20%EC%88%98%20%EC%9E%88%EC%96%B4%EC%9A%94..txt)]

- 10.10 **export/import 보다 더 업그레이드 되어진 data pump 를 알아야 해요**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/10.10%20export%20import%20%EB%B3%B4%EB%8B%A4%20%EB%8D%94%20%EC%97%85%EA%B7%B8%EB%A0%88%EC%9D%B4%EB%93%9C%20%EB%90%98%EC%96%B4%EC%A7%84%20data%20pump%20%EB%A5%BC%20%EC%95%8C%EC%95%84%EC%95%BC%20%ED%95%B4%EC%9A%94.txt)]

- 10.11 **현업에서 가장 많이 쓰는 유져 레벨 pump 를 사용할 수 있어야해요**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/10.11%20%ED%98%84%EC%97%85%EC%97%90%EC%84%9C%20%EA%B0%80%EC%9E%A5%20%EB%A7%8E%EC%9D%B4%20%EC%93%B0%EB%8A%94%20%EC%9C%A0%EC%A0%B8%20%EB%A0%88%EB%B2%A8%20pump%20%EB%A5%BC%20%EC%82%AC%EC%9A%A9%ED%95%A0%20%EC%88%98%20%EC%9E%88%EC%96%B4%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 10.12 **한번에 데이터 이관을 끝내는 테이블 스페이스 레벨 펌프 사용법**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/10.12%20%ED%95%9C%EB%B2%88%EC%97%90%20%EB%8D%B0%EC%9D%B4%ED%84%B0%20%EC%9D%B4%EA%B4%80%EC%9D%84%20%EB%81%9D%EB%82%B4%EB%8A%94%20%ED%85%8C%EC%9D%B4%EB%B8%94%20%EC%8A%A4%ED%8E%98%EC%9D%B4%EC%8A%A4%20%EB%A0%88%EB%B2%A8%20%ED%8E%8C%ED%94%84%20%EC%82%AC%EC%9A%A9%EB%B2%95.txt)]

- 10.13 **고수들이 데이터 이행 하는 방법은 이렇습니다.**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/10.13%20%EA%B3%A0%EC%88%98%EB%93%A4%EC%9D%B4%20%EB%8D%B0%EC%9D%B4%ED%84%B0%20%EC%9D%B4%ED%96%89%20%ED%95%98%EB%8A%94%20%EB%B0%A9%EB%B2%95%EC%9D%80%20%EC%9D%B4%EB%A0%87%EC%8A%B5%EB%8B%88%EB%8B%A4.txt)]

- 10.14 **외부 테이블을 생성할 줄 알아야해요.**: [📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/10.14%20%EC%99%B8%EB%B6%80%20%ED%85%8C%EC%9D%B4%EB%B8%94%EC%9D%84%20%EC%83%9D%EC%84%B1%ED%95%A0%20%EC%A4%84%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)]

- 10.15 **pump 를 엔진으로 해서 외부 테이블을 생성할 줄 알아야해요.**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/10.15%20pump%20%EB%A5%BC%20%EC%97%94%EC%A7%84%EC%9C%BC%EB%A1%9C%20%ED%95%B4%EC%84%9C%20%EC%99%B8%EB%B6%80%20%ED%85%8C%EC%9D%B4%EB%B8%94%EC%9D%84%20%EC%83%9D%EC%84%B1%ED%95%A0%20%EC%A4%84%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)]


### 11. **DB reorg 작업하기**

- 11.1 **db reorg 작업하기**: [📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/11.1%20db%20reorg%20%EC%9E%91%EC%97%85%ED%95%98%EA%B8%B0.txt)]

&nbsp;  

위의 수업 내용은  [이지업 클래스](https://easyupclass.e-itwill.com/main/index.jsp) 온라인 강의에서 곧 수강하실 수 있게 됩니다.
&nbsp;  




### ⚡ 오라클을 처음부터 배우시는 분들을 위해 SQL과 SQL튜닝 강의를 소개합니다.


- **SQL 강의(국비지원)**:  🖥️ [영상](https://www.e-itwill.com/course/course_view.jsp?id=121&ch=course&cid=&s_style=gallery&scid=&s_field=&s_keyword=)  

- **SQL 강의**:  🖥️ [영상](https://easyupclass.e-itwill.com/course/course_view.jsp?id=22&cid=123&ch=course)  

- **SQL튜닝 강의**:  🖥️ [영상](https://easyupclass.e-itwill.com/course/course_view.jsp?id=69&cid=155)

- **SQL자동화 강의**:  🖥️ [영상](https://easyupclass.e-itwill.com/course/course_view.jsp?id=447&cid=28)  

&nbsp;


---

감사합니다!

[코딩 대한민국](https://codingkorea.example.com)

