# C# 학습 기록 (산업용 소프트웨어 특화)

**학습 방식**: Claude와 함께 실습 중심 학습
**학습 시작일**: 2026-01-31
**목표**: 공장설비 데이터 수집/처리 소프트웨어 개발
**기간**: 6개월 (현업 투입 목표)

**참고 도서**:
- "C# in Depth" - Jon Skeet
- "Pro C# 10 with .NET 6" - Andrew Troelsen
- "Concurrency in C# Cookbook" - Stephen Cleary

---

## 진도 체크리스트

### Part 1: C# 기초 복습 (1-2주)

- [ ] **개발 환경 설정**
  - 핵심: Visual Studio, .NET SDK, 프로젝트 구조
- [ ] **기본 문법 복습**
  - 핵심: 변수, 자료형, 조건문, 반복문, 메서드
- [ ] **자료구조**
  - 핵심: 배열, List, Dictionary, Queue, Stack
- [ ] **객체지향 기초**
  - 핵심: 클래스, 생성자, 프로퍼티, 접근제한자
- [ ] **예외 처리**
  - 핵심: try/catch/finally, 사용자 정의 예외

### Part 2: 객체지향 심화 (2-3주)

- [ ] **상속과 다형성**
  - 핵심: 상속, virtual/override, abstract, sealed
- [ ] **인터페이스**
  - 핵심: interface, 다중 구현, 의존성 역전
- [ ] **제네릭**
  - 핵심: 제네릭 클래스/메서드, 제약조건, 공변성/반공변성
- [ ] **델리게이트와 이벤트**
  - 핵심: delegate, event, Action, Func, 이벤트 패턴
- [ ] **LINQ 기초**
  - 핵심: 쿼리 문법, 메서드 문법, Where, Select, OrderBy
- [ ] **LINQ 심화**
  - 핵심: GroupBy, Join, Aggregate, 지연 실행

### Part 3: .NET 핵심 (2-3주)

- [ ] **파일 I/O**
  - 핵심: File, StreamReader/Writer, 바이너리 파일
- [ ] **직렬화**
  - 핵심: JSON (System.Text.Json), XML, 바이너리 직렬화
- [ ] **정규표현식**
  - 핵심: Regex, 패턴 매칭, 데이터 파싱
- [ ] **날짜와 시간**
  - 핵심: DateTime, TimeSpan, DateTimeOffset, 시간대
- [ ] **컬렉션 심화**
  - 핵심: IEnumerable, ICollection, Concurrent 컬렉션

### Part 4: 비동기 프로그래밍 (3-4주)

- [ ] **스레드 기초**
  - 핵심: Thread, ThreadPool, 동기화 문제
- [ ] **동기화 기법**
  - 핵심: lock, Monitor, Mutex, Semaphore
- [ ] **Task 기반 비동기**
  - 핵심: Task, Task<T>, async/await, 비동기 패턴
- [ ] **비동기 심화**
  - 핵심: ConfigureAwait, 취소 토큰, 진행률 보고
- [ ] **병렬 프로그래밍**
  - 핵심: Parallel.For, PLINQ, 데이터 병렬처리
- [ ] **동시성 패턴**
  - 핵심: Producer-Consumer, 파이프라인, 채널

### Part 5: 데이터베이스 연동 (2-3주)

- [ ] **ADO.NET 기초**
  - 핵심: SqlConnection, SqlCommand, SqlDataReader
- [ ] **Entity Framework Core 기초**
  - 핵심: DbContext, 엔티티, 마이그레이션
- [ ] **EF Core 쿼리**
  - 핵심: LINQ to Entities, 로딩 전략, 성능 최적화
- [ ] **시계열 DB 연동**
  - 핵심: InfluxDB, TimescaleDB 연동 (센서 데이터용)

### Part 6: 네트워크 프로그래밍 (2-3주)

- [ ] **TCP/UDP 기초**
  - 핵심: TcpClient, TcpListener, UdpClient
- [ ] **HTTP 클라이언트**
  - 핵심: HttpClient, REST API 호출, 인증
- [ ] **WebSocket**
  - 핵심: 실시간 통신, 양방향 데이터 스트림
- [ ] **시리얼 통신**
  - 핵심: SerialPort, RS-232/485, Modbus (설비 연동)

### Part 7: 산업 프로토콜 (3-4주)

- [ ] **OPC UA 개요**
  - 핵심: OPC UA 아키텍처, 정보 모델, 보안
- [ ] **OPC UA 클라이언트**
  - 핵심: 연결, 노드 탐색, 데이터 읽기/쓰기
- [ ] **OPC UA 구독**
  - 핵심: Subscription, MonitoredItem, 실시간 데이터
- [ ] **Modbus TCP**
  - 핵심: Modbus 프로토콜, 레지스터 읽기/쓰기
- [ ] **MQTT**
  - 핵심: IoT 메시징, Publish/Subscribe, QoS

### Part 8: 데스크톱 앱 개발 (3-4주)

- [ ] **WPF 기초**
  - 핵심: XAML, 레이아웃, 컨트롤, 데이터 바인딩
- [ ] **MVVM 패턴**
  - 핵심: Model-View-ViewModel, INotifyPropertyChanged, Command
- [ ] **WPF 차트/시각화**
  - 핵심: LiveCharts, OxyPlot, 실시간 그래프
- [ ] **WPF 심화**
  - 핵심: 스타일, 템플릿, 사용자 정의 컨트롤

### Part 9: 실무 패턴 & 아키텍처 (2-3주)

- [ ] **SOLID 원칙**
  - 핵심: 단일책임, 개방폐쇄, 리스코프, 인터페이스분리, 의존성역전
- [ ] **디자인 패턴**
  - 핵심: Factory, Singleton, Observer, Strategy, Repository
- [ ] **의존성 주입**
  - 핵심: DI 컨테이너, Microsoft.Extensions.DependencyInjection
- [ ] **로깅 & 모니터링**
  - 핵심: Serilog, NLog, 구조화된 로깅

### Part 10: 실무 프로젝트 (4주)

- [ ] **프로젝트 1: 센서 데이터 수집기**
  - 핵심: OPC UA/Modbus 연동, 데이터 저장, 로깅
- [ ] **프로젝트 2: 설비 모니터링 대시보드**
  - 핵심: WPF, 실시간 그래프, 알람 시스템
- [ ] **프로젝트 3: 데이터 전처리 파이프라인**
  - 핵심: 비동기 처리, 배치 처리, Python 연동

---

## 학습 일지

| 날짜 | 주제 | 주요 내용 | 비고 |
|------|------|----------|------|

---

## 진행 현황

- **총 항목**: 45개
- **완료**: 0개
- **진행률**: 0%

---

## 디렉토리 구조

```
study/csharp/
├── README.md              # 진도 체크리스트 (현재 파일)
├── CLAUDE.md              # Claude 학습 지침서
├── notes/                 # 주제별 학습 노트
└── logs/                  # 학습 일지
```
