# Flask

## Flask?
Python 기반 마이크로 웹 프레임워크
* 마이크로 = 작지만 있을 건 다 있다! -> 매우 가볍고 작은 프로젝트에서 효율을 내는 특징을 가지고 있음

## 가상환경 (Virtual Environment)
각 프로젝트의 목적에 따른 모듈만 있는 환경을 구축해서 관리할 수 있도록 함
### 파이썬 가상환경 모듈 설치하기
`pip install virtualenv`
### 현재 디렉토리에 새 가상환경 만들기
`virtualenv <가상환경 이름>`
* 통상적으로는 **venv**로 가상환경 이름을 많이 씀
### 가상환경에 진입하기
Mac
* `source venv/bin/activate`
Window
* `./venv/Scripts/activate.bat`
* `call venv/bin/activate`
* `venv\Scripts\activate`

## Flask 설치하기
`pip install flask`

## Flask 시작하기
`flask run`
