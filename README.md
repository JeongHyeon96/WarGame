# ESG 팀 Wargame 프로젝트

## 📂 프로젝트 개요
**ESG 팀**은 웹 해킹을 중심으로 한 **Wargame** 플랫폼을 개발하는 팀 프로젝트를 진행 중입니다. 이 프로젝트는 **httpd (Apache)**와 **MariaDB**를 활용한 로컬 웹 환경에서 보안 취약점 문제를 풀며 실력을 쌓을 수 있는 시스템을 구현하고 있습니다.

각 팀원은 웹 해킹과 관련된 **취약점 문제**를 10개씩 작성하고, 이를 통해 **SQL Injection**, **Cross-Site Scripting (XSS)**, **File Inclusion**, **Command Injection** 등 다양한 웹 취약점을 실습할 수 있는 환경을 제공합니다.

## 🖼️ 데모 미리보기

> ESG Wargame 프로젝트 실행 화면

![Wargame Demo](demo.gif)

# Web Wargame 문제 요약

이 프로젝트는 웹 및 시스템 보안 문제를 해결하는 웹 워게임입니다. 각 문제는 다양한 보안 취약점 및 해킹 기법을 기반으로 합니다. 
아래는 본인이 제작한 각 문제의 간략한 요약입니다.

| 파일명     | 주요 기술/컨셉                         | 난이도   | 특징 요약                                                         |
|------------|--------------------------------------|----------|------------------------------------------------------------------|
| 01.php     | 정적 플래그 제출                      | 하       | 콘솔에서 힌트를 얻어 정적 플래그를 추출하는 방식. 취약점이 없는 간단한 입력형 문제.  |
| 02.php     | 정적 플래그 + 소스 코드 힌트            | 하       | 관리자가 실수로 소스 코드에 남긴 취약점을 이용해 FLAG를 추출. 소스 보기로 힌트 획득.  |
| 03.php     | 쿠키 값 변조                          | 하~중    | 쿠키 값을 변조하여 FLAG를 찾는 문제. 브라우저 콘솔을 활용해 변조하는 방식.  |
| 04.php     | XSS 취약점                           | 중       | XSS 취약점을 통해 쿠키를 유출시키는 문제. 공격자가 쉽게 악용할 수 있는 취약점. |
| 05.php     | 세션 기반 관리자 권한 우회            | 중~상    | PHPSESSID 조작을 통해 세션을 탈취하거나 관리자 권한을 얻어 FLAG 확인. 세션 관리 취약점. |
| 06.php     | 버퍼 오버플로우 (BOF) 취약점 활용      | 중~상    | 버퍼 오버플로우를 이용해 관리자 권한을 획득하고 FLAG를 확인. 메모리 취약점. |
| 07.php     | X-HTTP-Method-Override 취약점 활용    | 중~상    | HTTP 요청 헤더의 취약점을 이용해 POST 요청처럼 처리하여 FLAG 제출. HTTP 메소드 우회 취약점. |
| 08.php     | SQL Injection                         | 하       | SQL Injection을 이용해 데이터베이스를 우회하여 FLAG를 추출. 입력값 검증 미흡. |
| 09.php     | Blind SQL Injection                   | 중~상    | Blind SQL Injection을 통해 정보 유출 없이 데이터베이스에서 FLAG를 추출. |
| 10.php     | 권한 상승 (find 명령어 활용)          | 상       | 시스템 환경에서 `find` 명령어를 이용해 숨겨진 파일을 찾고 권한 상승 후 FLAG를 추출. |


이 워게임의 각 문제는 웹 보안 취약점 분석 및 해킹 기법을 실습할 수 있는 좋은 기회를 제공합니다. 각 문제의 난이도는 점차 상승하며, 다양한 보안 취약점을 해결하는 방법을 배울 수 있습니다.


## 🛠 기술 스택
- **Frontend**: HTML, CSS, JavaScript
- **Backend**: PHP (또는 팀 협업에 따라 다른 기술을 사용할 수 있음)
- **Web Server**: **httpd (Apache)**
- **Database**: **MariaDB**
- **Version Control**: Git, GitHub
- **Vulnerabilities Focus**: SQL Injection, XSS, Command Injection, File Inclusion 등

## 📝 프로젝트 기능
- **다양한 웹 해킹 취약점 문제**: 각 팀원은 **SQL Injection**, **Cross-Site Scripting (XSS)**, **File Inclusion**, **Command Injection** 등 다양한 웹 해킹 취약점 문제를 작성하고 이를 풀 수 있습니다.
- **문제 풀이 환경**: 사용자는 **httpd (Apache)**와 **MariaDB**를 로컬에서 설정하여 웹 애플리케이션 환경에서 취약점을 해결합니다.
- **정답 확인**: 문제를 풀고 나면 정답을 확인하여, 취약점 해결에 대한 피드백을 받을 수 있습니다.
- **로컬 서버 환경**: **httpd (Apache)**와 **MariaDB**를 활용하여 로컬 서버에서 안전하게 실습할 수 있습니다.

## 👥 팀원 구성
- **팀명**: ESG
- **팀원 수**: 6명
  - 각 팀원은 10개의 웹 해킹 취약점 문제를 작성하여 총 60개의 문제를 제출합니다.

## 🎯 프로젝트 목표
- 웹 해킹 및 보안 취약점 실습을 통해 보안 전문가로서의 역량을 키울 수 있습니다.
- SQL Injection, XSS, File Inclusion, Command Injection 등 다양한 웹 취약점을 학습하고 해결하는 능력을 기를 수 있습니다.
- 팀원들과 협업하여 문제를 해결하고, 보안 취약점에 대한 심도 있는 이해를 바탕으로 실습합니다.

## 📄 프로젝트 구조
```
root/var/www/html
├── problems/                          # Wargame 문제 폴더
│   ├── beomgeun/                      # 범근님의 문제 폴더
│   ├── byeonguk/                      # 병욱님의 문제 폴더
│   ├── memory/                        # 재호님의 문제 폴더
│   ├── seungmin/                      # 승민님의 문제 폴더
│   ├── timemachine/                   # 길형님의 문제 폴더
│   └── junghyun/                      # 정현(나)의 문제 폴더
├── flags.php                          # 각 문제의 정답 PHP 파일
├── img/                               # 메인페이지 및 문제 이미지 폴더
├── index.php                          # 홈페이지 php 파일
├── main.php                           # 홈페이지에서 Start누르면 문제목록들이 나오는 php 파일
├── js/                              # js 폴더
│   ├── main.js                      # 메인 페이지 js 파일
│   ├── jumpscare.js                 
│   ├── memory02.js                  
│   ├── script.js                    
│   ├── terminal05.js                
│   └── terminal06.js                
└── style/                           # CSS 스타일 디렉토리

```
## 🚀 실행 방법
1. **웹 서버 환경 설정**:
    - **httpd (Apache)**와 **MariaDB**를 로컬 환경에 설치합니다.
    - 데이터베이스 설정 및 웹 서버 설정을 완료한 후 프로젝트를 실행할 준비를 합니다.

2. **로컬 서버 실행**:
    - Apache 웹 서버를 실행하여, 프로젝트를 로컬 서버에서 확인할 수 있습니다.
    - `sudo systemctl start httpd` 명령어로 웹 서버를 시작합니다.
    - MariaDB는 `sudo systemctl start mariadb`로 시작합니다.

3. **프로젝트 실행**:
    - PHP 파일을 `httpd` 서버에서 제공하도록 설정합니다.
    - 웹 브라우저에서 `http://localhost`로 접속하여 프로젝트를 실행할 수 있습니다.

---

**ESG 팀 Wargame 프로젝트**는 웹 해킹을 통해 보안 취약점 문제를 해결하는 과정에서 실력을 키울 수 있는 플랫폼을 제공합니다. 각종 웹 해킹 기법을 익히고, 취약점 해결 능력을 향상시킬 수 있습니다.
