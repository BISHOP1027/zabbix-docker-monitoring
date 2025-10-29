# Zabbix Docker Monitoring (Email Alert Project)

이 프로젝트는 Docker 기반으로 **Zabbix 모니터링 환경을 직접 구축하고**,  
CPU 사용률 등 시스템 자원 상태를 실시간으로 감시하며 **메일 알림 자동화**를 구현한 미니 프로젝트입니다.

---

## 💡 프로젝트 개요
Zabbix는 서버·네트워크·애플리케이션의 상태를 통합적으로 감시할 수 있는 오픈소스 모니터링 툴입니다.  
본 프로젝트에서는 Zabbix의 핵심 기능을 중심으로 다음 목표를 달성했습니다.

- Docker 환경에서 **Zabbix Server / Web / Agent** 구성  
- **Host 및 템플릿 설정**을 통한 자원 모니터링 자동화  
- **CPU 임계치 감지 트리거** 생성으로 문제 상황 자동 탐지  
- **Gmail SMTP 연동**을 통한 실시간 메일 알림 구현  

이 과정을 통해 시스템 모니터링의 기본 구조(수집 → 감시 → 통보)를 직접 설계하고 검증했습니다.

---

## 🧩 프로젝트 구조
```
zabbix-docker-monitoring/
├─ docker-compose.yml
├─ .env.example
├─ README.md
└─ docs/
  ├─ 01-login.png
  ├─ 02-host-list.png
  ├─ 03-trigger-problem.png
  └─ 04-mail-alert.png
```

---

## 🔍 주요 포인트
| 구분 | 설명 |
|------|------|
| **프로젝트 목표** | 자원 모니터링과 알림 자동화의 전체 흐름 구축 |
| **기술 스택** | Docker, Zabbix, Gmail SMTP |
| **핵심 기능** | 서버 상태 감시, 트리거 기반 장애 감지, 메일 알림 |
| **결과물** | 트리거 발생 시 Gmail로 실시간 알림 도착 확인 |

---

## 🖼️ 스크린샷 구성
| 파일명 | 설명 |
|--------|------|
| 01-login.png | Zabbix 웹 로그인 화면 |
| 02-host-list.png | Host 등록 목록 |
| 03-trigger-problem.png | CPU 트리거 발생 (Problem) |
| 04-mail-alert.png | Gmail 경고 메일 도착 화면 |

---

## 🧭 프로젝트 의의
이 프젝트는 Zabbix를 활용한 서버 자원 모니터링 환경 구축 및 알림 자동화 경험입니다.

Docker 기반으로 Zabbix Server, Web, Agent를 구성하고, 트리거를 통해 CPU 사용률 임계치를 실시간으로 감시하며 Gmail SMTP 연동으로 장애 발생 시 메일 알림이 전송되도록 구현했습니다.

이를 통해 모니터링 시스템의 구성 원리와 알림 흐름을 직접 설계하고 운영한 경험을 쌓았습니다.

---

## 🪶 License
MIT
