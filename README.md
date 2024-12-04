# 아동·청소년 상담 데이터를 활용한 8가지 학대 및 폭력 유형 분류 연구

> classification-of-9-types-of-violence-using-child-and-adolescent-counseling-data

## 1. 서론

최근 아동학대가 증가하는 추세에 있으며, 그 중 대부분이 가정 내에서 발생하고 있다. 그러나 이러한 학대는 외부에서 인지하기 어려워 즉각적인 대응이 어렵다. 아동들은 학대를 당하고 있어도 이를 인지하지 못하거나 두려움으로 인해 외부에 알리지 못하는 경우가 많다. 따라서 아동과의 자연스러운 대화를 통해 학대 여부를 파악할 수 있는 방법이 필요하다. 본 연구에서는 아동·청소년 상담 데이터를 활용하여 8가지 학대 및 폭력 유형을 분류하는 인공지능 모델을 개발하고자 한다.

## 2. 연구 배경

#### 2.1 아동학대 현황

- **아동학대 신고 증가**: 2023년 아동학대 신고접수 건수는 48,522건으로 전년 대비 5.2% 증가하였다. 이는 최근 5년간 지속적인 증가 추세를 보이는 수치이다.<sup>[1](https://www.mohw.go.kr/board.es?act=view&bid=0027&list_no=1482953&mid=a10503010100&nPage=1)</sup>
- **가정 내 학대 비중**: 학대 발생 장소 중 가정 내 비중이 82.9%로 가장 높다.<sup>[2](https://www.sisayonhapnews.com/news/articleView.html?idxno=43577)</sup> 이는 대부분의 학대가 가정에서 발생하며, 외부에서 인지하기 어렵다는 것을 의미한다.
- **재학대의 심각성**: 전체 아동학대 사례 중 재학대 비율이 15.7%에 달한다. 이는 학대가 반복되고 만성화될 수 있음을 보여주며, 이에 대한 심층적인 연구와 대책이 필요하다.<sup>[1](https://www.mohw.go.kr/board.es?act=view&bid=0027&list_no=1482953&mid=a10503010100&nPage=1)</sup>

#### 2.2 학대 발견의 어려움

가정 내에서 발생하는 학대는 교사나 경찰 등 외부 기관에서 발견하기 어렵다. 아동들은 학대를 당하고 있어도 이를 인지하지 못하거나 두려움으로 인해 외부에 알리지 못한다. 따라서 비침해적이고 자연스러운 방법으로 학대 여부를 파악할 수 있는 접근이 필요하다.

## 3. 연구 목적

본 연구의 목적은 아동과의 자연스러운 대화를 통해 가정 내에서 발생하는 아동학대 여부를 판별하는 인공지능 모델을 개발하는 것이다. 이를 위해 아동·청소년 상담 데이터를 활용하여 8가지 학대 및 폭력 유형을 분류하는 연구를 수행하고자 한다.

## 4. 연구 진행

- 데이터 설명
  - dataset/\*: 원본 데이터셋: [AI 허브 아동·청소년 상담 데이터셋](https://www.aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&dataSetSn=71680)
  - origin_data.csv: dataset을 모은 원본 데이터
  - field.csv: 학대 정도를 3단계로 구분한 데이터셋
  - simple_field.csv: 학대 정도를 구분하지 않고 9가지 학대 유형만을 포함한 데이터셋
  - simple_field.arff: simple_field.csv를 arff 파일로 변환한 데이터셋(Mac 포멧, Windows 호환안됨)
- 코드 설명
  - main.ipynb: 데이터 전처리.
  - smo.ipynb: SVC 모델을 사용한 학대 유형 분류.
  - naive_bayes.ipynb: Naive Bayes 모델을 사용한 학대 유형 분류.
  - naive_bayes_field.ipynb: Naive Bayes 모델을 사용한 학대 정도 분류.
  - kobert.ipynb: KoBERT 모델을 사용한 학대 유형 분류.
  - kobert_field.ipynb: KoBERT 모델을 사용한 학대 정도 분류.

## 5. 기대 효과

#### 5.1 아동학대 조기 발견 및 예방

- **비침해적 학대 징후 파악**: 아동과의 대화를 통해 자연스럽게 학대 징후를 파악할 수 있다.
- **신속한 대응 가능**: 인공지능 모델을 활용하여 학대 여부를 빠르게 판단하고, 필요한 조치를 신속하게 취할 수 있다.

#### 5.2 다양한 분야에서의 활용

- **교육 현장**: 교사들이 학생들과의 상담 시 학대 징후를 파악하는 데 도움을 줄 수 있다.
- **상담 센터 및 복지 기관**: 전문 상담사들의 업무 효율을 높이고, 더 많은 아동들을 지원할 수 있다.
- **정책 수립 지원**: 데이터를 기반으로 한 분석을 통해 정부 및 관련 기관의 정책 수립에 기여할 수 있다.

#### 5.3 아동의 안전과 권익 보호

- **아동 보호 강화**: 학대의 조기 발견으로 피해 아동을 보호하고, 추가적인 피해를 예방할 수 있다.
- **건강한 성장 지원**: 안전한 환경에서 아동이 건강하게 성장할 수 있도록 지원한다.

## 6. 결론

아동학대는 심각한 사회 문제로, 조기 발견과 예방이 중요하다. 본 연구에서는 아동·청소년 상담 데이터를 활용하여 8가지 학대 및 폭력 유형을 분류하는 인공지능 모델을 개발함으로써, 학대의 조기 발견과 개입을 가능하게 하고자 한다. 이를 통해 아동의 안전과 권익을 보호하고, 건강한 사회 구성원으로 성장할 수 있도록 지원하는 데 기여할 것으로 기대된다.

## 참고 자료

1. 보건복지부 보도자료: [https://www.mohw.go.kr/board.es?act=view&bid=0027&list_no=1482953&mid=a10503010100&nPage=1](https://www.mohw.go.kr/board.es?act=view&bid=0027&list_no=1482953&mid=a10503010100&nPage=1)
2. 시사연합뉴스 기사: [https://www.sisayonhapnews.com/news/articleView.html?idxno=43577](https://www.sisayonhapnews.com/news/articleView.html?idxno=43577)
3. AI 허브 아동·청소년 상담 데이터셋: [https://aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=data&dataSetSn=71680](https://aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=data&dataSetSn=71680)
