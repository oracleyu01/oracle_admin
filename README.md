# 오라클 관리 수업 가이드

안녕하세요,  여러분! 🌟

오라클 dba와 오라클 엔지니어를 준비하시는 여러분들을 위해 오라클 관리 스크립트를 정리하였습니다.

## 시작하는 법

아래의 내용을 순서데로 보시면 됩니다.

## 수업 자료 

- **제목**: 노트
|--------|-------------------------------------------------------------|--------------------|

### **1.오라클 구조**

- **오라클 데이터 베이스 서버 구조를 알아야해요.**: 📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/%EC%98%A4%EB%9D%BC%ED%81%B4%20%EB%8D%B0%EC%9D%B4%ED%84%B0%20%EB%B2%A0%EC%9D%B4%EC%8A%A4%20%EC%84%9C%EB%B2%84%EC%9D%98%20%EA%B5%AC%EC%A1%B0%EB%A5%BC%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)
- **오라클 데이터베이스 메모리 구조를 알아야해요.**: 📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/%EC%98%A4%EB%9D%BC%ED%81%B4%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4%20%EB%A9%94%EB%AA%A8%EB%A6%AC%20%EA%B5%AC%EC%A1%B0%EB%A5%BC%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94..txt)
- **공유풀(shared pool)이 왜 필요한지 알아야해요.**: 📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/%EA%B3%B5%EC%9C%A0%ED%92%80(shared%20pool)%EC%9D%B4%20%EC%99%9C%20%ED%95%84%EC%9A%94%ED%95%9C%EC%A7%80%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94..txt)
- **데이터베이스 버퍼 캐쉬(database buffer cache) 가 왜 필요한지 알아야해요.**: 📄 [노트](https://github.com/oracleyu01/oracle_admin/blob/main/%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4%20%EB%B2%84%ED%8D%BC%20%EC%BA%90%EC%89%AC(database%20buffer%20cache)%20%EA%B0%80%20%EC%99%9C%20%ED%95%84%EC%9A%94%ED%95%9C%EC%A7%80%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)
- **리두로그 버퍼(redo log buffer) 가 왜 필요한지 알아야해요.**: 📄  [노트](https://github.com/oracleyu01/oracle_admin/blob/main/%EB%A6%AC%EB%91%90%EB%A1%9C%EA%B7%B8%20%EB%B2%84%ED%8D%BC(redo%20log%20buffer)%20%EA%B0%80%20%EC%99%9C%20%ED%95%84%EC%9A%94%ED%95%9C%EC%A7%80%20%EC%95%8C%EC%95%84%EC%95%BC%ED%95%B4%EC%9A%94.txt)
- **PGA 메모리 영역이 왜 필요한지 알아야해요.**: 📄  [노트]()
- **DBWn 프로세서의 역할을 알아야해요.**: 📄 [노트]()
- **LGWR (log writer)의 역할을 알아야해요.**: 📄  [노트]()
- **CKPT (checkpoint process)의 역할을 알아야해요.**: 📄 [노트]()
- **SMON(System Monitor process)의 역할을 알아야해요.**: 📄 [노트]()
- **PMON 프로세서 (Process monitor)의 역할을 알아야해요.**: 📄 [노트]()
- **ARCn (Archive process)의 역할을 알아야해요.**: 📄 [노트]()

### **2.저장 영역 구조**

- **데이터 베이스 저장 영역 구조**: 📄   [노트]()
- **논리적 및 물리적 데이터 베이스 구조**: 📄  [노트]()

### **3.startup 단계와 shutdown 옵션**

- **startup 의 4가지 단계를 알아야 해요!**: 📄 [노트]()
- **database 종료 모드 4가지를 알고 있어야 해요.**: 📄 [노트]()

### **4.파라미터 파일 관리**

- **dba는 초기화 파라미터 관리를 잘 할 줄 알아야 해요.**: 📄  [노트]()
- **alter system 과 alter session 의 차이는 ?**: 📄 [노트]()

### **5.테이블 스페이스 관리**

- **테이블 스페이스 생성과 관리에 대한 A4지 한장이 머리속에 있어야해요**: 📄 [노트]()
- **데이터를 저장하기 위한 첫걸음 !  테이블 스페이스 생성**: 📄 [노트]()
- **테이블 스페이스를 삭제할 때는 이 옵션을 알아야해요.**: 📄 [노트]()
- **default tablespace 가 뭔지 알고 있어야합니다.**: 📄  [노트]()
- **테이블 스페이스에 공간이 꽉차면 공간을 추가할 줄 알아야해요.**: 📄 [노트]()
- **과도한 정렬 작업을 위해서는 Temporary tablespace 를 잘 이해하고 있어야합니다.**: 📄 [노트]()
- **과도한 DML 작업이 성공적으로 수행되려면 undo tablespace 를 잘 이해하고 있어야해요**: 📄 [노트]()
- **만약 data file 이름을 변경하거나 다른 위치로 이동하고 싶다면?**: 📄  [노트]()
- **테이블 스페이스의 세그먼트 관리 방법을 알아야해요.**: 📄 [노트]()
- **OMF(Oracle Managed File) 이 뭔지 알아야해요 !**: 📄 [노트]()
- **테이블 스페이스 생성시 extent 관리 방법을 알아야해요.**: 📄 [노트]()
- **bigfile tablespace 가 뭔지 알아야해요**: 📄 [노트]()

### **6.언두 테이블 스페이스 관리**

- **undo data 가 무엇인지 알고 있어야해요.**: 📄   [노트]()
- **undo data 와 redo data 를 서로 다른거예요.**: 📄  [노트]()
- **언두 data 관리는 자동으로 되고 있어요.**: 📄  [노트]()
- **undo_retention 을 1시간으로 변경했다고 해서 그것을 확실히 보장하지는 않아요**: 📄 [노트]()
- **ORA-01555 snap shot too old 에러가 뭔지 알고 있어야 해요**: 📄 [노트]()

### **7.오라클 네트워크 관리**

- **오라클에 접속하려면 4가지 정보를 알아야 해요**: 📄 [노트]()
- **sqldeveloper 나 dbever 로 오라클에 접속하려면 리스너 통해서 접속해야해요.**: 📄  [노트]()
- **오라클 네트워크를 다루는 관리 도구가 4가지가 있습니다.**: 📄 [노트]()
- **listener.ora 파일의 위치가 어디에 있는지 알아야 합니다.**: 📄 [노트]()
- **오라클 서버에 접속하는 방식은 총 4가지가 있습니다.**: 📄  [노트]()
- **오라클에 접속 안될때 확인하는 방법 3가지를 알고 있어야해요.**: 📄 [노트]()

### **8.유져관리**

- **유져 생성시 상세한 옵션들을 dba 는 알고 있어야해요.**: 📄 [노트]()
- **유져를 생성하기 위해서 유져 인증 방법 3가지를 알고 있어야해요.**: 📄  [노트]()
- **오라클 db 를 올렸다 내렸다 할 수 있는 권한 관리가 2가지가 있어요.**: 📄 [노트]()
- **보안을 강화 하기 위해서 유져를 잠그거나 암호를 자주 변경해야해요.**: 📄 [노트]()
- **오라클의 권한의 종류는 크게 2가지가 있어요.**: 📄 [노트]()
- **내가 받은 시스템 권한을 남에게 주려면 with admin option을 알아야해요**: 📄 [노트]()
- **객체권한을 남에게 줄 수 있는 권한까지 같이 주려면 with grant option을 알아야해요**: 📄 [노트]()
- **롤(role)을 사용하게 되면 편하게 권한 부여를 할 수 있습니다.**: 📄 [노트]()

### **9.리소스 메니져**

- **특정 세션이 오라클의 자원을 무한히 사용하지 못하게 해야 해요.**: 📄 [노트]()
- **resource manager 로 cpu 사용을 제한해볼 수 있어야해요.**: 📄 [노트]()
- **리소스 메니져를 이용해서 병렬도를 제한하기**: 📄 [노트]()
- **리소스 메니져를 이용해서 악성 sql 이 수행 안되게 설정하기**: 📄 [노트]()

### **10.데이터 이행**

- **데이터를 이행하는 3가지 방법을 알아야 해요**: 📄 [노트]()
- **서브쿼리를 사용한 insert 문의 속도를 높이는 방법을 알아야해요.**: 📄[노트]()
- **High water mark 위에 데이터를 넣을때 병렬로 작업하면 더 빠르게 데이터를 입력할 수 있어요.**: 📄 [노트]()
- **대용량 csv 파일을 오라클 데이터 베이스로 로드할 때는 SQL*Loader 를 쓰세요.**: 📄[노트]()
- **테이블 생성 스크립트를 추출할 줄 알아야해요**: 📄 [노트]()
- **export / import 이용해서 데이터 이행을 할 줄 알아야해요**: 📄 [노트]()
- **유져 레벨로 export /import 를 할줄 알아야해요.**: 📄[노트]()
- **tablespace level 로 export/import 를 할 줄 알아야해요**: 📄  [노트]()
- **database 를 통채로 export/import 를 할 수 있어요.**: 📄 [노트]()
- **export/import 보다 더 업그레이드 되어진 data pump 를 알아야 해요**: 📄 [노트]()
- **현업에서 가장 많이 쓰는 유져 레벨 pump 를 사용할 수 있어야해요**: 📄 [노트]()
- **한번에 데이터 이관을 끝내는 테이블 스페이스 레벨 펌프 사용법**: 📄 [노트]()
- **고수들이 데이터 이행 하는 방법은 이렇습니다.**: 📄  [노트]()
- **외부 테이블을 생성할 줄 알아야해요.**: 📄  [노트]()
- **pump 를 엔진으로 해서 외부 테이블을 생성할 줄 알아야해요.**: 📄 [노트]()

### **11.DB reorg 작업하기**

- **db reorg 작업하기**: 📄 [노트]()
