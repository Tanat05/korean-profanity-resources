# korean-profanity-resources

직접 욕설, 비속어, 혐오 표현 관련 모델을 개발하면서 유용하다고 생각된 리소스를 모아둔 저장소입니다.

AI를 이용해 편집된 내용입니다.

누구나 쉽게 접근할 수 있는 데이터들로 이루어진 만큼 라이선스를 꼭 지켜주시기 바랍니다.

자연어 처리(NLP) 프로젝트, 특히 텍스트 윤리 검증, 악성 댓글 필터링, 혐오 표현 감지 등의 작업에 유용하게 활용될 수 있습니다.

## 목차

- [데이터셋](#데이터셋): 욕설, 비속어, 혐오 표현을 기준으로 라벨링 된 데이터
- [라이브러리](#라이브러리): 욕설, 비속어, 혐오 표현을 다루는 라이브러리
- [API](#api): 욕설, 비속어, 혐오 표현 판별 기능을 지원하는 API
- [모델](#모델): 욕설, 비속어, 혐오 표현 판별하는 모델
- [라이선스](#라이선스-요약): 데이터셋, 라이브러리, API에 사용된 라이선스 요약
- [성능 검증](#성능검증): 라이브러리, API를 데이터셋으로 어느정도의 성능이 나오는지 표로 정리(업데이트 예정)


# 데이터셋

| 데이터셋 이름                                                       | URL                                                                                                                                            | 데이터 건수 | 라이선스                                 | 설명                                                                                                                                                                                                                                                  |
| :---------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------- | :----------: | :--------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 한국어 악성댓글 데이터셋                                            | [korean-malicious-comments-dataset](https://github.com/ZIZUN/korean-malicious-comments-dataset)                                                   |  10,000   |  MIT License                           | 한국어 악성 댓글을 수집한 데이터셋                                                                                                                                                                                                                |
| Curse-detection-data                                              | [Curse-detection-data](https://github.com/2runo/Curse-detection-data)                                                                       |   5,825   |  MIT License                     | 각종 커뮤니티 사이트 댓글의 욕설 여부를 분류한 데이터셋                                                                                                                                                                                                |
| kmhas_korean_hate_speech                                         | [kmhas_korean_hate_speech](https://huggingface.co/datasets/jeanlee/kmhas_korean_hate_speech)                                                     |  78,978   | CC BY-SA 4.0                            | 온라인 뉴스 댓글을 8가지 혐오 표현으로 세분화하여 분류한 데이터셋                                                                                                                                                                              |
| Korean Extremist Website Womad Hate Speech Data                  | [Korean Extremist Website Womad Hate Speech Data](https://www.kaggle.com/datasets/captainnemo9292/korean-extremist-website-womad-hate-speech-data/data) |   2,081   | 확인 필요                                 | 한국 극단주의 웹사이트(워마드) 데이터를 분류한 데이터셋                                                                                                                                                                                                |
| LGBT-targeted HateSpeech Comments Dataset (Korean)                | [LGBT-targeted HateSpeech Comments Dataset (Korean)](https://www.kaggle.com/datasets/junbumlee/lgbt-hatespeech-comments-at-naver-news-korean)       |   8,837   | CC BY-NC-SA 4.0                        | 네이버 뉴스 성소수자 관련 댓글을 분류한 데이터셋                                                                                                                                                                                                |
| korean-hate-chat-data                                            | [korean-hate-chat-data](https://www.kaggle.com/datasets/tanat05/korean-hate-chat-data)                                                             | 5,000,000 | CC BY-NC-SA 4.0                         | korcen으로 분류한 korcen-ml의 학습 파일 중 일부                                                                                                                                                                                                 |
| korean-hate-speech                                               | [korean-hate-speech](https://github.com/kocohub/korean-hate-speech)                                                                             |   9,381   | CC BY-SA 4.0                             | 한국 연예 뉴스 수집 플랫폼의 댓글 데이터셋                                                                                                                                                                                                         |
| korean_unsmile_dataset                                           | [korean_unsmile_dataset](https://github.com/smilegate-ai/korean_unsmile_dataset?tab=readme-ov-file)                                                 |  18,742   | CC BY-NC-ND 4.0                        | Smilegate AI에서 공개한 한국어 혐오표현 "☹️ UnSmile" 데이터셋                                                                                                                                                                                      |
| bad_word_list                                                   | [bad_word_list](https://github.com/hlog2e/bad_word_list)                                                                                         |   1,145   | 확인 필요                             | 한국에서 주로 사용되는 패드립, 욕설, 비속어 등의 JSON Array                                                                                                                                                                                         |
| 한국어 혐오표현 분류(탐지) 데이터셋                                | [한국어 혐오표현 분류(탐지) 데이터셋](https://open.selectstar.ai/ko/tunib)                                                                        | 100,000  | CC BY-SA 3.0                               | 윤리적으로 문제가 되는 혐오 발화를 분류하여 문장의 윤리성을 판별하는 한국어 혐오 발화 데이터셋                                                                                                                                                       |
| 텍스트 윤리검증 데이터                                             | [텍스트 윤리검증 데이터](https://aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=realm&dataSetSn=558)                         | 453,340  | 확인 필요                              | 비윤리 검증 데이터 선도사례 제시 및 AI 윤리 연구 자료를 공적 활용에 제공                                                                                                                                                                        |
| APEACH - Korean Hate Speech Evaluation Datasets                  | [APEACH - Korean Hate Speech Evaluation Datasets](https://github.com/jason9693/APEACH)                                                             |   3,844   | CC BY-SA 4.0                             | 혐오 발언 탐지를 위한 최초의 크라우드 생성 한국어 평가 데이터셋                                                                                                                                                                                |
| Naver sentiment movie corpus v1.0                               | [Naver sentiment movie corpus v1.0](https://github.com/e9t/nsmc)                                                                                 | 200,000  | CC0 1.0                              | 한국어로 된 영화 리뷰 데이터셋 (감성 분석에도 사용 가능)                                                                                                                                                                                           |
| K-MHaS                                                          | [K-MHaS](https://github.com/adlnlp/K-MHaS)                                                                                                       | 109,692  | 확인 필요                            | 한국어 패턴을 효과적으로 처리하는 혐오 발언 탐지를 위한 새로운 다중 라벨 데이터셋                                                                                                                                                                     |
| DKTC                                                            | [DKTC](https://github.com/tunib-ai/DKTC)                                                                                                       |       -       | CC BY-NC-SA 4.0                               | 2021 인공지능 그랜드 챌린지 4차대회 음성인지 트랙에 참가하기 위해 자체적으로 제작한 데이터셋 (혐오/악성 표현 포함 여부 불명확)                                                                                                                         |
| KOLD                                                            | [KOLD](https://github.com/boychaboy/KOLD)                                                                                                       |       -       | 확인 필요                             | 한국어 공격 언어(Offensive Language) 데이터셋                                                                                                                                                                                                  |
| 속성기반 감정분석 데이터                                             | [속성기반 감정분석 데이터](https://aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=data&dataSetSn=71603)                         | 250,312  | 확인 필요                              | 상품 리뷰데이터에 포함된 사용자 감정을 태깅한 데이터셋 (긍/부정 감정 분류에 사용 가능, 혐오/악성 표현 포함 여부 불명확)                                                                                                                                    |

# 라이브러리

| 언어        | 라이브러리                                                                                                              | 라이선스                          | 설명                                                                                                                                                  |
| :---------- | :---------------------------------------------------------------------------------------------------------------------- | :------------------------------ | :---------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Python**  | [korcen](https://github.com/Tanat05/korcen)                                                                                 | Apache License 2.0                     | 키워드 기반 비속어 판단 모듈                                                                                                                             |
|             | [korcen-ml](https://github.com/Tanat05/korcen-ml)                                                        | Apache License 2.0               | korcen으로 분류한 데이터를 학습한 딥러닝 기반 비속어 판별 모델 (정확도 향상)                                                                              |
|             | [badword_check](https://github.com/Nam-SW/badword_check)                                                                   | 확인 필요               | 딥러닝 기반 한글 욕설 판별 모델                                                                                                                               |
|             | [CurseDetector](https://github.com/mangto/CurseDetector)                                                                   | 확인 필요                     | 한글 유사도와 한글 발음 유사도를 이용한 욕설/비속어/금지어 필터링                                                                                              |
|             | [badwordDetection2](https://github.com/0-inf/badwordDetection2?tab=readme-ov-file)                                                                   | MIT License                     | 만들다가 실패한 [욕설탐지모듈](https://github.com/0-inf/KoreanBadwordDetection)의 아이디어를 바탕으로 새롭게 만드는 욕설탐지모듈입니다.                                                                                              |
| **Java**    | [BadWordFiltering](https://github.com/VaneProject/bad-word-filtering)                                                        | MIT License                | 비속어 필터링 라이브러리 (상세 알고리즘 확인 필요)                                                                                                         |
|             | [bad-word-filtering](https://github.com/Ghosttrio/bad-word-filtering)                                                      | 확인 필요                     | 비속어 필터링 라이브러리 (상세 알고리즘 확인 필요)                                                                                                         |
| **JavaScript** | [Cenkor](https://github.com/sh9351/cenkor)                                                                                 | Apache License 2.0                     | korcen 데이터셋을 이용한 비속어 검열 라이브러리                                                                                                                |
| **TypeScript** | [korcen.ts](https://github.com/Tanat05/korcen.ts)                                                                           | Apache License 2.0                     | korcen의 TypeScript 포팅 버전 (NPM 모듈)                                                                                                                 |
| **Dart**    | [korean_profanity_filter](https://github.com/Xim-ya/korean_profanity_filter)                                                 | MIT License                     | 정규식 기반 한국어 욕설 필터링 라이브러리                                                                                                                       |
| **Go**      | [korcen-go](https://github.com/fluffy-melli/korcen-go)                                                                       | Apache License 2.0                     | korcen의 Go 언어 포팅 버전                                                                                                                                  |                                                                      |

# API
| API                                                                         | 라이선스                 | 설명                                                                                                                |
| :-------------------------------------------------------------------------- | :----------------------- | :------------------------------------------------------------------------------------------------------------------ |
| [profanity-filter-api](https://github.com/Whale0928/profanity-filter-api)   | GPL-3.0 License          | [KISO 이용자 보호 시스템 API 서비스](https://github.com/Whale0928/profanity-filter-api) 서비스를 API로 제공       |
| [do-not-say-profanity](https://github.com/shinwonse/do-not-say-profanity) | MIT License              | Google Jigsaw의 Perspective API를 활용한 비속어 검사 서비스                           |
| [korcen-api](https://github.com/fluffy-melli/korcen-api) | Apache License 2.0 & MIT License              | [korcen-go](https://github.com/fluffy-melli/korcen-go)기반으로 만든 API                           |

# 모델
| 모델 이름 | GitHub / Hugging Face 링크 | 설명 |
|---|---|---|
| **korcen-ml** | https://github.com/Tanat05/korcen-ml |  **한국어** 비속어 탐지 모델입니다. 채팅 데이터를 학습했으며 일부 모델만 공개하고 최신 모델의 경우 유료로 판매하고 있습니다. |
| **badword_check** | https://github.com/Nam-SW/badword_check |  **한국어** 비속어 탐지 라이브러리입니다. 간단한 API를 제공하여 빠르게 비속어 여부를 판단할 수 있습니다. 내장된 비속어 사전을 기반으로 탐지하며, 사용자가 직접 비속어 사전을 추가할 수도 있습니다. 정확도보다는 속도에 중점을 둔 모델입니다. |
| **EthicalEye** | https://huggingface.co/autopilot-ai/EthicalEye |  **영어**에 특화된 유해 콘텐츠(toxic content) 탐지 모델입니다.  Hate speech, insults, threats, obscene language 등 다양한 유형의 유해 콘텐츠를 탐지합니다.  RoBERTa 모델을 기반으로 하며, 높은 정확도를 자랑합니다.  영어 데이터에 대한 높은 성능을 보이지만, 다국어 지원은 제한적입니다. |
| **multilingual-sentiment-analysis** | https://huggingface.co/tabularisai/multilingual-sentiment-analysis |  다국어 감성 분석 모델입니다.  **비속어 탐지 전용 모델은 아니지만**, 부정적인 감성을 가진 텍스트를 탐지하는 기능을 통해 간접적으로 비속어를 탐지하는 데 활용할 수 있습니다.  XLM-RoBERTa 모델을 기반으로 하며, 영어, 프랑스어, 독일어, 스페인어, 이탈리아어, 포르투갈어, 러시아어, 중국어, 일본어, **한국어** 등 다양한 언어를 지원합니다. |


# 라이선스 요약
## 데이터셋
| 라이선스 유형          | 설명                                                                                                                                 | 상업적 이용 | 수정   | 재배포 | 저작권 및 라이선스 고지 | 동일 라이선스 조건 |
| :-------------------- | :----------------------------------------------------------------------------------------------------------------------------------- | :--------- | :----- | :----- | :------------------- | :--------------- |
| **CC0**              | 저작권자가 저작물에 대한 모든 권리를 포기. 누구나 어떤 목적으로든 자유롭게 이용 가능. 저작자 표시 의무 없음.                               | ⭕       | ⭕   | ⭕   | ❌                 | ❌            |
| **MIT License**      | 매우 허용 범위가 넓은 오픈소스 라이선스. 저작권자와 라이선스 문구 명시하면 상업적 이용, 수정, 재배포 등 모두 가능. 소스코드 공개 의무 없음. | ⭕       | ⭕   | ⭕   | ⭕                   | ❌            |
| **CC BY**            | 저작자 표시. 저작자만 표시하면 영리적 이용, 변경 및 2차 저작물 작성이 모두 가능.                                                     | ⭕       | ⭕   | ⭕   | ⭕                   | ❌            |
| **CC BY-SA**         | 저작자 표시-동일조건변경허락. 저작자를 표시하고, 2차 저작물에 동일한 라이선스를 적용하는 한 자유롭게 이용 가능.                           | ⭕       | ⭕   | ⭕   | ⭕                   | ⭕              |
| **CC BY-ND**         | 저작자 표시-변경 금지. 저작자를 표시해야 하며, 저작물 변경은 불가능.                                                                 | ⭕       | ❌ | ⭕   | ⭕                   | ❌            |
| **CC BY-NC**         | 저작자 표시-비영리. 저작자를 표시해야 하며, 영리적 이용은 불가능.                                                                     | ❌     | ⭕   | ⭕   | ⭕                   | ❌            |
| **CC BY-NC-SA**      | 저작자 표시-비영리-동일조건변경허락. 저작자를 표시하고, 비영리 목적으로만 사용 가능하며, 2차 저작물에 동일한 라이선스를 적용해야 함.   | ❌     | ⭕   | ⭕   | ⭕                   | ⭕              |
| **CC BY-NC-ND**      | 저작자 표시-비영리-변경 금지. 저작자를 표시하고, 비영리 목적으로만 사용 가능하며, 저작물 변경은 불가능.                                   | ❌     | ❌ | ⭕   | ⭕                   | ❌            |
| **확인 필요**          | 라이선스 정보가 명확히 기재되어 있지 않거나, 추가 확인이 필요한 경우. | ❓     | ❓ | ❓ | ❓                 | ❓            |
## 라이브러리/API
| 라이선스 유형          | 설명                                                                                                                                                                                             | 상업적 이용 | 수정   | 재배포 | 저작권 및 라이선스 고지 | 소스 코드 공개 | 동일 라이선스 조건 |
| :-------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :--------- | :----- | :----- | :------------------- | :----------- | :--------------- |
| **MIT License**      | 매우 허용 범위가 넓은 라이선스. 상업적 이용, 수정, 재배포 가능. 저작권 및 라이선스 고지 필요. 소스코드 공개 의무는 없음.                                                                               | ⭕       | ⭕   | ⭕   | ⭕                   | ❌        | ❌            |
| **Apache License 2.0** | 특허권 관련 조항이 포함된 오픈 소스 라이선스. 상업적 이용, 수정, 재배포 가능. 저작권 및 라이선스 고지, 변경 사항 명시 필요. 소스코드 공개 의무는 없음.                                                       | ⭕       | ⭕   | ⭕   | ⭕                   | ❌        | ❌            |
| **GPL-3.0 License**   | 강력한 카피레프트(copyleft) 라이선스. 이 라이선스를 사용한 코드를 포함하는 프로그램은 반드시 동일한 라이선스로 공개해야 함. 상업적 이용 가능. 저작권 및 라이선스 고지, 변경 사항 명시, 소스 코드 공개 필요. | ⭕       | ⭕   | ⭕   | ⭕                   | ⭕          | ⭕              |
| **확인 필요**          | 라이선스 정보가 명확히 기재되어 있지 않거나, 추가 확인이 필요한 경우. | ❓     | ❓ | ❓ | ❓                 | ❓            | ❓            |

# 성능검증
> 데이터와 결과가 일치한 개수 / 전체 데이터 개수
> 
> 현재의 성능은 많이 다를 수 있음
>
> 언젠가 업데이트 예정

|  | [korean-malicious-comments-dataset](https://github.com/ZIZUN/korean-malicious-comments-dataset) | [Curse-detection-data](https://github.com/2runo/Curse-detection-data) | [kmhas_korean_hate_speech](https://huggingface.co/datasets/jeanlee/kmhas_korean_hate_speech) | [Korean Extremist Website Womad Hate Speech Data](https://www.kaggle.com/datasets/captainnemo9292/korean-extremist-website-womad-hate-speech-data/data) | [LGBT-targeted HateSpeech Comments Dataset (Korean)](https://www.kaggle.com/datasets/junbumlee/lgbt-hatespeech-comments-at-naver-news-korean) | [korean-hate-chat-data](https://www.kaggle.com/datasets/tanat05/korean-hate-chat-data) | [korean-hate-speech](https://github.com/kocohub/korean-hate-speech) | [korean_unsmile_dataset](https://github.com/smilegate-ai/korean_unsmile_dataset?tab=readme-ov-file) | 평균 처리 속도 |
|------|------|------|------|------|------|------|------|------|------|
| [korcen](https://github.com/KR-korcen/korcen) | 0.7121 | 0.8415 | 0.6773 | 0.6305 | 0.4479 | 0.9857 |  | 0.5534 | 9ms |
| [korcen-ml](https://github.com/KR-korcen/korcen-ml/blob/main/README.md) | **0.8395** | **0.8432** | **0.8851** | **0.7155** | **0.7020** | **0.9941** |  | **0.7824** | 40ms |
| [badword_check](https://github.com/Nam-SW/badword_check) | 0.5829 | 0.6761 |  | 0.6410 | 0.4738 | 0.7980 |  | 0.4913 | 43ms |
| [CurseDetector](https://github.com/mangto/CurseDetector) |  | 0.5679 |  | 0.5785 |  | 0.6657 |  |  | 267ms |
| [BadWordFiltering](https://github.com/VaneProject/bad-word-filtering) |  |  |  |  |  |  |  |  |  |
| [Cenkor](https://github.com/sh9351/cenkor) |  | 0.8317 |  | 0.6275 |  |  |  |  | **0.2**ms |
| [korcen.ts](https://github.com/Tanat05/korcen.ts) |  |  |  |  |  |  |  |  |  |
| [korean_profanity_filter](https://github.com/Xim-ya/korean_profanity_filter) |  |  |  |  |  |  |  |  |  |
