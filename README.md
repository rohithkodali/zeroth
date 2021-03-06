# Project: Zeroth
* Kaldi-based Korean ASR open-source project
* 칼디를 이용하여 구축하는 한국어 음성인식
* License: Apache 2.0

Zeroth 프로젝트는 Kaldi open source tool-kit 을 사용해서 한국어 음성인식기를 구현하는 프로젝트 입니다. 
이 프로젝트는 기업이 AI를 고객 서비스에 추가하는 데 도움이되는 [(주)아틀라스가이드](https://www.goodatlas.com)의 AI 플랫폼 개발의 일부로서 개발되었습니다. 
Kaldi official recipe 에 한국어 버전을 소개하는 것을 시작으로, 
많은 사람들의 참여를 통해 누구나 사용할 수 있는 음성인식기를 만들어 나갈 수 있도록 하는 것을 목표로하는 프로젝트입니다.
제로스라는 이름은 0-th, 즉 0 번째를 의미합니다. 이름이 의미하는 것처럼 이 프로젝트를 통해 음성인식기를 
만들기 위해 필요한 모든 과정을 처음부터 끝까지 함께 해보고 토론할 수 있기를 바랍니다.

Contact: Lucas Jo (lucasjo@goodatlas.com)

### Special thanks 

* [Gridspace Inc.](https://www.gridspace.com) 사에서 일하고 계신 Wonkyum Lee 님과의 co-work 를 통해 이 프로젝트를 진행하고 있음을 밝힙니다. 

### Mentioned records
* [Interview](http://blog.naver.com/fastcampus/221181060609) with FastCampus
* [딥러닝-음성인식 CAMP](http://www.fastcampus.co.kr/data_camp_dsr/) @ FastCampus

## 1. Audio Data

* 2018.02.03: 51.6 시간 한국어 학습데이터 (22,263 발화, 105명, 3000 문장)
* License: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)

현재 제로스 프로젝트에는 상기와 같은 음성데이터가 포함되어 있습니다.
공개 음성 DB 구축에 참여할 수 있는 음성 녹음 앱 [모아코인(Android)](https://play.google.com/store/apps/details?id=com.goodatlas.morecoin)을 제공하고 있으며, 
해당 앱을 통해 음성 데이터를 1시간 기부해주시면 해당 시점까지 구축된 공개 음성 DB에 접근하여 다운로드할 수 있는 권한을
AWS temporary credential 형태로 발급해 드립니다. 한번 발급된 credential은 12 시간 동안 유효합니다.
더 자세한 내용은 [AWS-temporary-credential](https://github.com/goodatlas/zeroth/wiki/AWS-temporary-credential) 
페이지를 확인하시기 바랍니다

## 2. Requirements

* 제로스 프로젝트를 실행하는데 필요한 패키지들에 대한 설명은 [Requirements](https://github.com/goodatlas/zeroth/wiki/Requirements)
위키 페이지를 참조하시기 바랍니다.

## 3. Acoustic Model
현재 제로스 프로젝트 음향모델에는 아래와 같은 최신 kaldi recipe 가 적용되어 있습니다.

* TDNN + LSTM 
* Chain model
* Data augmentation of reverberant speech

## 4. Language Model & Lexicon
언어모델과 발음사전을 구현하기 위한 코드가 곧 업데이트 될 예정입니다.
