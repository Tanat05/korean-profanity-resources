> AI를 이용해 편집된 내용입니다.
# 🤬 korean-profanity-resources

직접 욕설, 비속어, 혐오 표현 관련 모델을 개발하면서 유용하다고 생각된 **한국어가 메인**이거나 **한국어가 포함된 글로벌 리소스**를 모아둔 저장소입니다.

> 한국어가 포함되어있지만 특정 언어에 특화된 리소스는 제외함

자연어 처리(NLP) 프로젝트, 특히 텍스트 윤리 검증, 악성 댓글 필터링, 혐오 표현 감지 등의 작업에 유용하게 활용될 수 있습니다.

누구나 쉽게 접근할 수 있는 데이터들로 이루어진 만큼 **라이선스**를 꼭 지켜주시기 바랍니다.

---

## 📑 목차

- [📊 데이터셋](#-데이터셋): 욕설, 비속어, 혐오 표현을 기준으로 라벨링 된 데이터
- [💻 라이브러리](#-라이브러리): 욕설, 비속어, 혐오 표현을 다루는 라이브러리
- [🌐 API](#-api): 욕설, 비속어, 혐오 표현 판별 기능을 지원하는 API
- [🤖 모델](#-모델): 욕설, 비속어, 혐오 표현 판별하는 모델
- [📜 라이선스 요약](#-라이선스-요약): 데이터셋, 라이브러리, API에 사용된 라이선스 요약
- [🤝 기여하기](#-기여하기): 새로운 리소스 추가 방법
- [🔍 검색어](#-keywords--검색어): 다국어 검색 키워드

---

## 📊 데이터셋

| 데이터셋 이름 | URL | 데이터 건수 | 라이선스 | 설명 |
| :--- | :--- | :---: | :---: | :--- |
| **한국어 악성댓글 데이터셋** | [Link](https://github.com/ZIZUN/korean-malicious-comments-dataset) | 10,000 | MIT | 한국어 악성 댓글을 수집한 데이터셋 |
| **Curse-detection-data** | [Link](https://github.com/2runo/Curse-detection-data) | 5,825 | MIT | 각종 커뮤니티 사이트 댓글의 욕설 여부를 분류한 데이터셋 |
| **kmhas_korean_hate_speech** | [Link](https://huggingface.co/datasets/jeanlee/kmhas_korean_hate_speech) | 78,978 | CC BY-SA 4.0 | 온라인 뉴스 댓글을 8가지 혐오 표현으로 세분화하여 분류 |
| **Womad Hate Speech Data** | [Link](https://www.kaggle.com/datasets/captainnemo9292/korean-extremist-website-womad-hate-speech-data/data) | 2,081 | 확인 필요 | 한국 극단주의 웹사이트(워마드) 데이터를 분류한 데이터셋 |
| **LGBT-targeted HateSpeech** | [Link](https://www.kaggle.com/datasets/junbumlee/lgbt-hatespeech-comments-at-naver-news-korean) | 8,837 | CC BY-NC-SA 4.0 | 네이버 뉴스 성소수자 관련 댓글을 분류한 데이터셋 |
| **korean-hate-chat-data** | [Link](https://www.kaggle.com/datasets/tanat05/korean-hate-chat-data/versions/7) | 14,879,962 | CC BY-NC-SA 4.0 | 온라인 대화 문장 수집 데이터 (korcen 1차 라벨링 + 검수) |
| **korean-hate-speech (BEEP!)** | [Link](https://github.com/kocohub/korean-hate-speech) | 9,381 | CC BY-SA 4.0 | 한국 연예 뉴스 수집 플랫폼의 댓글 데이터셋 |
| **korean_unsmile_dataset** | [Link](https://github.com/smilegate-ai/korean_unsmile_dataset) | 18,742 | CC BY-NC-ND 4.0 | Smilegate AI에서 공개한 한국어 혐오표현 "☹️ UnSmile" |
| **bad_word_list** | [Link](https://github.com/hlog2e/bad_word_list) | 1,143 | 확인 필요 | 한국에서 주로 사용되는 패드립, 욕설, 비속어 등의 JSON Array |
| **한국어 혐오표현 분류 데이터셋** | [Link](https://open.selectstar.ai/ko/tunib) | 100,000 | CC BY-SA 3.0 | 윤리적으로 문제가 되는 혐오 발화를 분류한 데이터셋 |
| **텍스트 윤리검증 데이터** | [Link](https://aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=realm&dataSetSn=558) | 453,340 | AI Hub | 비윤리 검증 데이터 선도사례 및 AI 윤리 연구 자료 |
| **APEACH** | [Link](https://github.com/jason9693/APEACH) | 3,844 | CC BY-SA 4.0 | 혐오 발언 탐지를 위한 최초의 크라우드 생성 한국어 데이터셋 |
| **Naver sentiment movie corpus** | [Link](https://github.com/e9t/nsmc) | 200,000 | CC0 1.0 | 한국어로 된 영화 리뷰 데이터셋 (감성 분석 및 비속어 포함) |
| **K-MHaS** | [Link](https://github.com/adlnlp/K-MHaS) | 109,692 | CC BY-SA 4.0 | 다중 라벨 혐오 발언 탐지를 위한 새로운 데이터셋 |
| **DKTC** | [Link](https://github.com/tunib-ai/DKTC) | 4,450 | CC BY-NC-SA 4.0 | 한국어 위협 대화 데이터셋 (협박, 갈취, 괴롭힘 등) |
| **KOLD** | [Link](https://github.com/boychaboy/KOLD) | 40,429 | 확인 필요 | 한국어 공격 언어(Offensive Language) 데이터셋 (EMNLP 2022) |
| **속성기반 감정분석 데이터** | [Link](https://aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=data&dataSetSn=71603) | 250,312 | AI Hub | 상품 리뷰 데이터에 포함된 사용자 감정 태깅 데이터셋 |
| **LDNOOBW (Korean)** | [Link](https://github.com/LDNOOBW/List-of-Dirty-Naughty-Obscene-and-Otherwise-Bad-Words) | - | CC BY 4.0 | 다양한 언어의 욕설 목록 중 한국어 섹션 포함 |
| **HateScore** | [Link](https://github.com/sgunderscore/hatescore-korean-hate-speech) | 약 11,000 | Apache 2.0 | 위키피디아에서 수집한 혐오 이슈 관련 댓글 데이터 |
| **나무위키 욕설 문서** | [Link](https://namu.wiki/w/%EC%9A%95%EC%84%A4/%ED%95%9C%EA%B5%AD%EC%96%B4) | - | CC BY-NC-SA 2.0 | 나무위키 한국어 욕설 관련 상세 설명 및 목록 |
| **f-word (list)** | [Link](https://github.com/theeluwin/f-word/blob/master/f_word/data/bad_words.json) | 약 400 | MIT | Python f-word 라이브러리에 내장된 비속어 리스트 |
| **korean-bad-words** | [Link](https://github.com/mogong2/korean-bad-words) | 약 100 | Unknown | JSON 형식의 간단한 한국어 비속어 목록 |
| **LoL 필터링 리스트 2020** | [Link](./%EB%A6%AC%EA%B7%B8%EC%98%A4%EB%B8%8C%EB%A0%88%EC%A0%84%EB%93%9C_%ED%95%84%ED%84%B0%EB%A7%81%EB%A6%AC%EC%8A%A4%ED%8A%B8_2020.txt) | 3,272 | 확인 필요 | 리그오브레전드(LoL)에서 사용되는 필터링 리스트 |
| **욕설 리스트 (slang.csv)** | [Link](./slang.csv) | 4,315 | 확인 필요 | 출처가 불분명한 데이터셋|

---

## 💻 라이브러리

| 언어 | 라이브러리 | 라이선스 | 설명 |
| :--- | :--- | :---: | :--- |
| **Python** | [korcen](https://github.com/Tanat05/korcen) | Apache 2.0 | 키워드 기반 비속어 판단 모듈 |
| | [badword_check](https://github.com/Nam-SW/badword_check) | 확인 필요 | 딥러닝 기반 한글 욕설 판별 모델 |
| | [CurseDetector](https://github.com/mangto/CurseDetector) | 확인 필요 | 한글 및 발음 유사도를 이용한 필터링 |
| | [f-word](https://github.com/theeluwin/f-word) | MIT | Python 비속어 필터링 라이브러리 |
| | [badwordDetection2](https://github.com/0-inf/badwordDetection2) | MIT | 새롭게 개발 중인 욕설 탐지 모듈 |
| **Java** | [BadWordFiltering](https://github.com/VaneProject/bad-word-filtering) | MIT | 비속어 필터링 라이브러리 |
| | [bad-word-filtering](https://github.com/Ghosttrio/bad-word-filtering) | 확인 필요 | Java 기반 비속어 필터링 |
| **JavaScript** | [Cenkor](https://github.com/sh9351/cenkor) | Apache 2.0 | korcen 데이터를 이용한 JS 라이브러리 |
| | [korean-badwords-filter](https://github.com/Eunmo/korean-badwords-filter) | MIT | 단순 키워드 매칭 기반 JS 필터 |
| **TypeScript** | [korcen.ts](https://github.com/Tanat05/korcen.ts) | Apache 2.0 | korcen의 TypeScript 포팅 버전 |
| **Dart** | [korean_profanity_filter](https://github.com/Xim-ya/korean_profanity_filter) | MIT | 정규식 기반 한국어 욕설 필터링 |
| **Go** | [korcen-go](https://github.com/fluffy-melli/korcen-go) | Apache 2.0 | korcen의 Go 언어 포팅 버전 |

---

## 🌐 API

| API | 라이선스 | 설명 |
| :--- | :---: | :--- |
| [profanity-filter-api](https://github.com/Whale0928/profanity-filter-api) | GPL-3.0 | KISO 이용자 보호 시스템 API 연동 서비스 |
| [do-not-say-profanity](https://github.com/shinwonse/do-not-say-profanity) | MIT | Google Perspective API 활용 비속어 검사 |
| [korcen-api](https://github.com/fluffy-melli/korcen-api) | Apache 2.0 | korcen-go 기반 REST API 서비스 |

---

## 🤖 모델

| 모델 이름 | 링크 | 설명 |
| :--- | :--- | :--- |
| **korcen-ml** | [GitHub](https://github.com/Tanat05/korcen-ml) | 한국어 비속어 탐지 ML 모델 (채팅 데이터 학습) |
| **badword_check** | [GitHub](https://github.com/Nam-SW/badword_check) | 사전 기반 고속 비속어 판별 모델 |
| **multilingual-sentiment** | [HuggingFace](https://huggingface.co/tabularisai/multilingual-sentiment-analysis) | XLM-RoBERTa 기반 다국어 감성 분석 (한국어 포함) |

---

## 📜 라이선스 요약

### 📊 데이터셋
| 라이선스 | 상업적 이용 | 수정 | 재배포 | 고지 의무 | 동일 라이선스 |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **CC0** | ⭕ | ⭕ | ⭕ | ❌ | ❌ |
| **MIT** | ⭕ | ⭕ | ⭕ | ⭕ | ❌ |
| **CC BY** | ⭕ | ⭕ | ⭕ | ⭕ | ❌ |
| **CC BY-SA** | ⭕ | ⭕ | ⭕ | ⭕ | ⭕ |
| **CC BY-NC-SA** | ❌ | ⭕ | ⭕ | ⭕ | ⭕ |

### 💻 라이브러리 & API
| 라이선스 | 상업적 이용 | 수정 | 재배포 | 소스 공개 | 동일 라이선스 |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **MIT** | ⭕ | ⭕ | ⭕ | ❌ | ❌ |
| **Apache 2.0** | ⭕ | ⭕ | ⭕ | ❌ | ❌ |
| **GPL-3.0** | ⭕ | ⭕ | ⭕ | ⭕ | ⭕ |

---

## 🤝 기여하기

추가하고 싶은 리소스가 있다면 언제든지 PR을 보내주세요!
1. 이 저장소를 포크합니다.
2. `README.md` 또는 데이터 파일을 수정합니다.
3. 변경 사항을 커밋하고 PR을 생성합니다.

---

## Star History

<a href="https://www.star-history.com/?repos=Tanat05%2Fkorean-profanity-resources&type=date&logscale=&legend=bottom-right">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=Tanat05/korean-profanity-resources&type=date&theme=dark&legend=bottom-right" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=Tanat05/korean-profanity-resources&type=date&legend=bottom-right" />
   <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=Tanat05/korean-profanity-resources&type=date&legend=bottom-right" />
 </picture>
</a>

## 🔍 Keywords / 검색어
**Korean:** 한국어 욕설, 비속어 리스트, 혐오 표현 데이터셋, 악성 댓글 필터링, 금지어 목록, 롤 욕설, 비하 발언 리소스, 일베 용어, 메갈 용어, 신조어 필터링
**English:** Korean profanity list, Korean bad words dataset, Korean hate speech detection, offensive language corpus, abusive language dataset, K-slang, Korean filtered words
**Chinese:** 韩国语辱骂词汇, 韩语脏话, 韩国语仇恨言论数据集, 韩国语非法词汇, 韩国网络用语, 韩国语谩骂语, 韩国语过滤词
**Japanese:** 韓国語の悪口, 韓国語不適切用語リスト, ヘ이트スピー치データセット, 韓国語ネットスラング, 放送禁止用語, 韓国語スラング, 悪口辞典

---
