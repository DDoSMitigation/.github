# 한국정보기술연구원(KITRI) 화이트햇 스쿨 2기

## 프로젝트 개요
저사양 환경에서 패킷을 모니터링하여 악성 패킷을 분류하고 차단하는 것을 목표로 하며, 누구나 무료로 안전한 인프라를 구성하는 것을 프로젝트 목표로 하고 있습니다.

## 멘토 및 주요 인원

### 멘토
- **박건호** (테이텀 시큐리티)

### 프로젝트 리더 (PL)
- **곽송이** (테이텀 시큐리티)

### 프로젝트 매니저 (PM)
- **함준형** (배재대학교) [LinkedIn](https://www.linkedin.com/in/%EC%A4%80%ED%98%95-%ED%95%A8-669898284/)

### 팀원
- **강성원** (배재대학교)
- **최홍석** (전북대학교)
- **임정훈** (조선대학교)
- **지도환** (한밭대학교)
- **김도현** (강릉원주대학교)
- **라민우** (건국대학교)

## 네트워크 정보
- **네트워크:** AS216362 (함준형)
- **업스트림:** AS20473 (The Constant Company, LLC), AS199524 (G-Core Labs S.A.)
- **애니캐스트 네트워크:** AS199524 (G-Core Labs S.A.)

[홈페이지](https://ddosmitigation.github.io/)

## 일정

### 4월
- **25일:** 레퍼런스 서치
- **29일:** 온라인 미팅
- **30일:** 팀원 회의

### 5월
- **3일:** 논문 리뷰 중간 점검
- **6일:** 온라인 미팅
- **10일:** 팀원 회의
- **13일:** 격주 보고서 초안 작성, 온라인 미팅, 팀원 회의
- **14일:** 격주 보고서 초안 검토 및 피드백
- **15일:** 격주 보고서 피드백 반영, 논문 초안 피드백
- **16일:** 격주 보고서 마무리
- **17일:** 격주 보고서 제출 (도환, 도현)
- **18일:** 논문 리뷰
  - 강성원: "BGP Anycast Tuner Intuitive Route Management for Anycast Services"
  - 최홍석: "Routing Around Congestion Defeating DDoS Attacks and Adverse Network Conditions via Reactive BGP Routing"
  - 지도환: "DDoS Mitigation AMeasurement-Based Approach & Understanding the Behaviors of BGP-based DDoS Protection Services"
- **19일:** 논문 리뷰
  - 함준형: "Anycast Agility Network Playbooks to Fight DDoS"
  - 라민우: "Fast packet processing with ebpf and xdp: Concepts, code, challenges, and applications"
  - 임정훈: "Extended Berkeley Packet Filter: An Application Perspective"
  - 김도현: "An eBPF-XDP hardware-based network slicing architecture for future 6G front to back haul networks"
- **25일:** 온라인 중간 발표
- **26일:** 회식
- **31일:** 격주 보고서 제출 (홍석, 정훈)

### 6월
- **14일:** 격주 보고서 제출 (성원, 준형)
- **28일:** 격주 보고서 제출 (민우)

### 7월
- **6일:** 오프라인 최종 발표

## 해야 할 일

### 전체 인원
- 논문 요약 및 번역본 GitHub 업로드 (5월 9일 완료)

### 개별 할 일
- **도환, 도현:** 격주 보고서 초안 작성 (완료)
- **준형, 민우:** XDP 보안 코드 개발 (완료)
- **홍석:** DDoS 공격 종류 및 각 공격 유형별 대응 방안 조사 (5월 11일 완료)
- **성원, 정훈, 준형:** 논문 초안 작성 (완료)

### 논문 요약 및 번역 완료
- **준형:** "Anycast Agility Network Playbooks to Fight DDoS"
- **성원:** "BGP Anycast Tuner Intuitive Route Management for Anycast Services"
- **홍석:** "Routing Around Congestion Defeating DDoS Attacks and Adverse Network Conditions via Reactive BGP Routing"
- **도환:** "DDoS Mitigation AMeasurement-Based Approach & Understanding the Behaviors of BGP-based DDoS Protection Services"
- **민우:** "Fast packet processing with ebpf and xdp: Concepts, code, challenges, and applications"
- **정훈:** "Extended Berkeley Packet Filter: An Application Perspective"
- **도현:** "An eBPF-XDP hardware-based network slicing architecture for future 6G front to back haul networks"

## 오픈소스 가이드라인 작성 (05월 13일 기준)
- **Zeek:** 완료
- **Arkime:** 완료
- **BCC:** 완료
- **Suricata:** 70%
- **BGP Tool:** 완료
- **XDP Firewall:** 완료
- **GPT-2:** 완료
- **BGP Anycast Tuner:** 90%
- **nDPI:** 진행중
- **Security Onion:** 진행중

## 논문 핵심
- **핵심:** 대용량 패킷을 BGP를 이용한 Anycast 구축으로 패킷을 분산시킴. BGP Flowspec, eBPF/XDP를 이용해 악성 패킷을 분류 및 필터링하여 대용량 패킷부터 세밀한 패킷까지 정교하게 필터링 하는 방법 제시. DPI를 통해 악성 행위 판단.
- **추가:** AI를 이용해 악성 패킷과 정상 패킷을 구분. 로그에 쌓이는 패킷 데이터를 기반으로 AI가 점점 정교한 패킷 분류 알고리즘을 생성.
- **추가:** 웹과 연동하여 실시간으로 모니터링 기능 제공.

## 테스트 IP
141.11.245.2
