# korean-profanity-resources

직접 욕설, 비속어, 혐오 표현 관련 모델을 개발하면서 유용하다고 생각된 리소스를 모아둔 저장소입니다.

누구나 쉽게 접근할 수 있는 데이터들로 이루어진 만큼 라이선스를 꼭 지켜주시기 바랍니다.

자연어 처리(NLP) 프로젝트, 특히 텍스트 윤리 검증, 악성 댓글 필터링, 혐오 표현 감지 등의 작업에 유용하게 활용될 수 있습니다.

## 목차

- [데이터셋](#데이터셋)
- [라이브러리](#라이브러리)
- [API](#api)
- [블로그](#블로그)
- [논문](#논문)
- [라이선스](#라이선스-요약)


# 데이터셋

| 데이터셋 이름                                                       | URL                                                                                                                                            | 데이터 건수 | 라이선스                                 | 설명                                                                                                                                                                                                                                                  |
| :---------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------- | :----------: | :--------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 한국어 악성댓글 데이터셋                                            | [korean-malicious-comments-dataset](https://github.com/ZIZUN/korean-malicious-comments-dataset)                                                   |  10,000   |  MIT License                           | 한국어 악성 댓글을 수집한 데이터셋                                                                                                                                                                                                                |
| Curse-detection-data                                              | [Curse-detection-data](https://github.com/2runo/Curse-detection-data)                                                                       |   5,825   |  MIT License                     | 각종 커뮤니티 사이트 댓글의 욕설 여부를 분류한 데이터셋                                                                                                                                                                                                |
| kmhas_korean_hate_speech                                         | [kmhas_korean_hate_speech](https://huggingface.co/datasets/jeanlee/kmhas_korean_hate_speech)                                                     |  78,978   | CC BY-SA 4.0                            | 온라인 뉴스 댓글을 8가지 혐오 표현으로 세분화하여 분류한 데이터셋                                                                                                                                                                              |
| Korean Extremist Website Womad Hate Speech Data                  | [Korean Extremist Website Womad Hate Speech Data](https://www.kaggle.com/datasets/captainnemo9292/korean-extremist-website-womad-hate-speech-data/data) |   2,081   | 확인 필요                                 | 한국 극단주의 웹사이트(워마드) 데이터를 분류한 데이터셋                                                                                                                                                                                                |
| LGBT-targeted HateSpeech Comments Dataset (Korean)                | [LGBT-targeted HateSpeech Comments Dataset (Korean)](https://www.kaggle.com/datasets/junbumlee/lgbt-hatespeech-comments-at-naver-news-korean)       |   8,837   | CC BY-NC-SA 4.0                        | 네이버 뉴스 성소수자 관련 댓글을 분류한 데이터셋                                                                                                                                                                                                |
| korean-hate-chat-data                                            | [korean-hate-chat-data](https://www.kaggle.com/datasets/tanat05/korean-hate-chat-data)                                                             | 5,000,00정

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

# 성능 검증
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
