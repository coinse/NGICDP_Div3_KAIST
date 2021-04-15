# 차세대정보컴퓨팅기술개발사업 실적 정리

## 과제 정보

| 항목 | 내용 |
| - | - |
| 사업명              | 원천기술개발사업 > 차세대정보컴퓨팅기술개발사업              |
| 지원기관            | 과학기술정보통신부 > 한국연구재단                            |
| 과제번호            | 2017M3C4A706817923                                           |
| 과제명              | 지능형 자동화를 통한 풀스택 SW 디버깅                        |
| 총괄 연구책임자     | KAIST 김문주 [moonzoo@cs.kaist.ac.kr](mailto:moonzoo@cs.kaist.ac.kr) |
| 세부과제명          | (3세부) 지능형 자동화를 통한 출스택 SW의 다중언어 검증 및 디버깅 |
| 세부과제 연구책임자 | KAIST 유신 [shin.yoo@kaist.ac.kr](mailto:shin.yoo@kaist.ac.kr) |
| 본 실적의 교신저자  | KAIST 유신 [shin.yoo@kaist.ac.kr](mailto:shin.yoo@kaist.ac.kr) |

## ToC
- [1단계 1차년도(2017.07 ~ 2018.05)](#1단계-1차년도-201709--201805)
- [2단계 1차년도(2018.06 ~ 2019.05)](#2단계-1차년도-201806--201905)
- [2단계 2차년도(2019.06 ~ 2020.03)](#2단계-2차년도-201906--202003)
- [2단계 3차년도(2020.04 ~ 2021.03)](#2단계-3차년도-202004--202103)

## 1단계 1차년도 (2017.09 ~ 2018.05)

#### K-1-1. Evaluating Lexical Approximation of Program Dependence (국제학술지: EMSE)

- 다중 언어 분석 효율을 향상시킬 수 있는 언어 모델 기반 분석 기법 3종 개발 (VSM-ORBS, LDA-ORBS, MOBS)
- 최대 80KLOC (guava)로 작성된 C, python, Java 등 3종 이상의 언어를 포함하는 SW를 대상으로 실험 (다중 언어 SW 포함)
- 세계 최고 수준 대비: 최대 316.3% (제안: 13.84 sec/LoC, 세계 최고 수준: 43.78 sec/LoC), 평균 200.2% (제안: 11.21 sec/LoC, 세계 최고 수준: 22.45 sec/LoC) 향상으로 목표 달성
- DOI: https://doi.org/10.1016/j.jss.2019.110459

```
@article{Lee2019aa,
  author = {Lee, Seongmin and Binkley, David and Gold, Nicolas and Islam, Syed and Krinke, Jens and Yoo, Shin},
  journal = {Journal of Systems and Software},
  keywords = {ORBS, Program slicing, Lexical analysis},
  pages = {110459},
  title = {Evaluating lexical approximation of program dependence},
  volume = {160},
  year = {2020}
}
```

#### K-1-2. Genetic Programming for MUSEUM Fault Localisation (보고서)

- 다중언어 결함 위치 식별 세계 최고 수준의 정확도를 가진 Museum에 SBFL 스코어를 추가한 유전 프로그래밍 모델을 이용해 분석한 결함 8개를 모두 정확하게 식별함 (100%)
- PDF: []

#### K-1-3. Muti-Lingual Fault Benchmark (보고서)

- Python과 C 두 개 언어로 이루어진 오픈소스 프로젝트 (TensorFlow, Numpy)로부터 다중언어 결함 10개 조사 발굴
- PDF: 

## 2단계 1차년도 (2018.06 ~ 2019.05)

#### K-2-1. MOAD: Modelling Observation-based Approximation Dependency (국제학회: SCAM)

- 뮤테이션 기반 의존성 예측 모델 3종 개발 (Once Success, Logistic, Bayesian)
- 개발된 모델을 바탕으로 기존 의존성 분석 모델 대비 18%만의 데이터를 사용하여 의존성을 예측 (accuracy: 약 89%), 분석 속도 기준 456% 향상으로 목표 달성
- DOI: https://doi.ieeecomputersociety.org/10.1109/SCAM.2019.00011

```
 @inproceedings{Lee2019pl,
  author = {Lee, Seongmin and Binkley, David and Feldt, Robert and Gold, Nicolas and Yoo, Shin},
  booktitle = {19th IEEE International Working Conference on Source Code Analysis and Manipulation},
  series = {SCAM 2019},
  title = {{MOAD}: Modeling Observation-based Approximate Dependency},
  year = {2019}
}
```



#### K-2-2. Amortising the Cost of Mutation Based Fault Localisation using Statistical Inference (보고서)

- 과거 뮤테이션 데이터를 분석하여 현재 발생한 결함의 위치를 예측하는 랭킹 모델 4종을 개발 (Exact Match, Partial Match, Logistic Regression, MLP). 
- 357개의 오픈소스 결함에 평가함.
- arXiv preprint: https://arxiv.org/abs/1902.09729, PDF: 

## 2단계 2차년도 (2019.06 ~ 2020.03)

#### K-3-1. Search Based Repair of Deep Neural Networks  (보고서)

- 다중언어 환경 구성 요소로 새롭게 등장한 심층신경망 모델에 대해, 기존에 트레이닝된 모델을 시드로 이용해 추가적인 데이터 없이 수정할 수 있는 휴리스틱 2종 개발 (각각 PSO, DE 기반)
- arXiv preprint: https://arxiv.org/abs/1912.12463, PDF: 

#### K-3-2. PyGGI 2.0: Language Independent Genetic Improvement Framework (국제학회: ESEC/FSE)

- Java, Python C에 모두 적용 가능한 자동 결함 수정 프레임워크 PyGGI 2.0 개발, QuixBugs 벤치마크 33개 결함 중 20개 패치 (60%)
- PyGGI 오픈소스 버전을 이용해 영국 UCL 연구진은 최대 70K+ 이상의 다중 언어 소프트웨어 최적화 성공 (https://ieeexplore.ieee.org/abstract/document/9392013)
- DOI: http://doi.acm.org/10.1145/3338906.3341184

```
@inproceedings{An2019aa,
  author = {An, Gabin and Blot, Aymeric and Petke, Justyna and Yoo, Shin},
  booktitle = {Proceedings of the 2019 27th ACM Joint Meeting on European Software Engineering Conference and Symposium on the Foundations of Software Engineering},
  doi = {10.1145/3338906.3341184},
  pages = {1100--1104},
  series = {ESEC/FSE 2019},
  title = {PyGGI 2.0: Language Independent Genetic Improvement Framework},
  url = {http://doi.acm.org/10.1145/3338906.3341184},
  year = {2019}
}
```



## 2단계 3차년도 (2020.04 ~ 2021.03)

#### K-4-1. Human-in-the-Loop Fault Localisation Using Efficient Test Prioritisation of Generated Tests (보고서)

- 결함 위치 식별의 정확도를 높이는 데에 필요한 테스트를 자동 생성 및 선별하는 휴리스틱 3종 개발 (K-4-1)
- arXiv preprint: https://arxiv.org/abs/2104.06641, PDF: 

#### K-4-2. Causal Program Dependence Analysis (보고서 / Under Review)

- 인과 추론 기계학습 기법을 이용, 다중 언어 환경에 적용 가능한 새로운 형태의 의존성 분석 기술 개발 (Causal Program Dependence Analysis): 의존성을 참/거짓이 아닌 특정 입력 집합에 대한 상대적 강도값으로 표현하여 프로그램의 의미적 행위를 좀 더 정확하게 담아낼 수 있음
- 인과적 프로그램 의존성 분석을 이용한 결함 위치 식별 기술 개발: 기존 의존성 기반 결함 위치 식별이 구분할 수 없는 의미적 차이를 구분하여 더 정확한 위치 식별 가능
- arXiv preprint:, PDF:, 





