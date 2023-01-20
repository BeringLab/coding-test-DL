# DL Coding test

안녕하세요. 베링랩입니다.  
저희 회사에서는 일종의 코딩테스트로 텍스트 전처리를 과제로 드리고 있습니다.

## 과제

다음과 같은 상황이라고 합시다:

- 기계번역을 데이터셋은 두 언어의 언어쌍으로 되어 있습니다. 두 언어를 영어와 한국어라고 하겠습니다.
- 본 테스트는 "법률"과 "경제", "뉴스" 분야에 특화된 기계번역 엔진을 만들고자 합니다.
- 한국어 문장과 영어 문장은 서로 의미가 맞아야하고, 한 쪽에는 있지만, 다른 한 쪽에는 누락된 문장 등의 요소가 많으면 이는 노이즈가 많은 문장으로 봅니다.
- 노이즈를 최소화하고 기계번역의 품질을 향상시키기 위해서 전처리와 정제는 필수적인 과정입니다.
- 또한 이러한 코드가 여러번 사용이 되기 위해서는 코드의 재사용성도 고려하는 것이 좋습니다. 

본 테스트는 참가자들의 코드 퀄리티, 대용량 데이터를 다루는 능력과 아이디어를 평가하기 위하여 만들어졌습니다.

## 제출

과제를 제출하는 방법은 다음과 같습니다:

1. 데이터 : [aihub-사회과학분야](https://aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=realm&dataSetSn=125)의 말뭉치(train-data만 사용)       를 다운로드합니다.
   [오픈소스 뉴스데이터](https://github.com/jungyeul/korean-parallel-corpora/tree/master/korean-english-news-v1)의 train, dev, test set을 모두 다운로드 합니다.
2. 본 저장소를 clone 하거나 참조할 **private** 저장소를 생성합니다.
   1. 생성한 저장소의 *collaborator*에 `jiwonseo1212`를 추가합니다.
3. 1번에서 다운 받은 말뭉치에서 *aihub* 데이터의 경우는 "법률"분야와 "경제"분야에 해당하는 한-영 페어를 뽑아냅니다. 뉴스데이터는 모두 사용합니다.
4. 3번에서 뽑아낸 페어를 **기계번역을위한 한-영 페어를 만들 목적을 고려하여** 자신의 방식으로 정제/전처리합니다.
5. 최종적으로 정제/전처리된 한국어와 영어 페어를 각각 100라인씩 txt 파일로 만들어 자신의 브랜치에 커밋합니다.(aihub 코퍼스와 뉴스 코퍼스가 섞일 수 있도록 shuffle을 적용해 줍니다.)

## 조건

과제를 수행하면서 다음 조건을 지켜주십시오:

- [ ] 생성하는 저장소는 **private** 저장소로 생성합니다.
  - [ ] 과제를 완료하신 후에 *collaborator*에 `jiwonseo1212`을 추가합니다.
- [ ] 파이썬 버전은 `3.9`를 사용합니다.
  - `3.9.0`, `3.9.1` 등등 `3.9` 버전 내의 파이썬 버전을 사용합니다.
- [ ] 제출하는 파이썬 파일은 `.py` 확장자여야 합니다.
  - [ ] 과제를 진행하면서 사용한 `.ipynb`을 사용하는 것은 허용되지만, 결과 파일은 `.py`여야 합니다.
- [ ] 파이썬을 제외한 쉘 스크립트나 도구를 사용하는 경우 사용법과 관련 파일도 포함해야 합니다.
  - 가능한 제출한 과제를 한번에 실행하는 방법(쉘 스크립트)를 포함하길 바랍니다.
- [ ] 파이썬 의존성을 추가한 경우, `requirements.txt`를 작성해야 합니다.
- [ ] 코드 작동과 관련해서는 docs등의 디렉터리를 추가하여 작성합니다.

## 참고문헌
- https://arxiv.org/pdf/1906.08885.pdf
- https://arxiv.org/pdf/1908.10084.pdf




