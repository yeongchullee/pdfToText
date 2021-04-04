# pdfToText
Python code, PDF file to Text file

파이썬프로그램.
PyMuPDF 모듈을 이용하여 영문 PDF 파일에서 문자를 추출하여 영문 텍스트파일로 저장한다음
이 파일을 한 문장 단위로 읽어 네이버 파파고 API를 사용하여 번역한다음 한글 텍스트파일로 저장하는 코드.

네이버 파파고 API 번역 함수
def papagoAPI(id, secret, sentence)

Pdf 파일에서 영어 문자를 추출하나 모든 단어에 개행문자 "\n"이 포함되어 있어서
"\n"을 제거한다음 단어에 "." 마침표가 포함된 단어를 정규표현식으로 찾아서 "\n"을 포함,
하나의 문장을 만들고 영어텍스트 파일로 저장하는 함수
def pdfToText(inputFile)

Papago API 함수 결과값을 받아서 한글파일로 저장하는 함수
def trans(id, secret, inputfile, line=20)

## 20라인까지 번역 결과물
문서 페이지 수 :  13
Text length :  68569

문장 길이 :  954

번역결과 0 : 적층 제조 19 (2018) 114–126 Science Direct 적층 제조 저널 홈 페이지: www.

번역결과 1 : 그밖에 더 나은

번역결과 2 : com/locate/addma 전체 길이 아티클 Luke Scime jack, Jack Beuth Next Manufacturing Center, 기계공학부, Carnegie Mellon University, 5000 Forbes Ave에서 훈련된 컴퓨터 비전 알고리즘 Luke Scime를 사용한 레이저 분말 적층 제조 공정에서의 이상 탐지 및 분류.
번역결과 3 : , Pittsburgh, PA 15213, 미국 기사 기사: 2017년 9월 25일 수정된 형태로 2017년 5월 3일 수령 2017년 11월 16일 수락됨 2017년 11월 16일 온라인으로 사용 가능 키워드: 적층 제조 컴퓨터 비전 기계 학습 현장 모니터링 이상 징후 확산 산업별 LPBF(Laser Powder Bed Fusion) 적층 제조의 급속한 도입에도 불구하고 현재 공정은 대부분 개방 루프 상태로 유지되며 실시간 모니터링 기능이 제한됩니다.
번역결과 4 : 일부 기계는 빌드 중에 파우더베드 시각화를 제공하지만 자동화된 분석 기능이 부족합니다.
번역결과 5 : 본 연구는 LPBF 기계에서 실시간 제어 시스템의 구성요소가 될 가능성이 있는 파우더베드 이미지의 현장 모니터링 및 분석을 위한 접근 방식을 제시한다.
번역결과 6 : 특히, 컴퓨터 비전 알고리즘은 공정의 분말 확산 단계에서 발생하는 이상 징후를 자동으로 감지하고 분류하는 데 사용된다.
번역결과 7 : 이상 탐지 및 분류는 이미지 패치의 적당한 크기의 훈련 데이터베이스에서 작동하는 비지도 기계 학습 알고리듬을 사용하여 구현된다.
번역결과 8 : 최종 알고리듬의 성능을 평가하고 독립 실행형 소프트웨어 패키지로서의 유용성은 여러 사례 연구를 통해 입증된다.
번역결과 9 : © 2017년형 Ethervier B.
번역결과 10 : 브이
번역결과 11 : 모든 권한이 예약되었습니다.
번역결과 12 : 1.
번역결과 13 : 소개 최근 몇 년 동안, 3D 프린팅으로 알려진 적층 제조는 산업으로서 엄청난 성장을 경험해 왔습니다. 이는 특히 그물 모양의 금속 부품을 생산하는 기계와 공정에서 그렇습니다. [1].
번역결과 14 : 적층 제조는 항공 우주 및 의료 애플리케이션[2]에 적합할 뿐만 아니라 원격지에서의 미션 크리티컬 부품 생산에도 적합할 것을 약속합니다 [3].
번역결과 15 : 그러나 이러한 애플리케이션에는 현재 시장에 출시된 시스템으로는 달성하기 어려운 부품 품질 보증 및 프로세스 신뢰성이 필요합니다 [1].
번역결과 16 : 이러한 애플리케이션의 엄격한 요건을 충족시키기 위해서는 현장 프로세스 모니터링 및 폐쇄 루프 제어의 구현이 필요하다는 것은 일반적으로 인정된다[1].
번역결과 17 : LPBF(Laser Powder Bed Fusion) 기계는 금속 분말의 얇은 층(일반적으로 두께 20 µm~60 µm)을 리코이터 블레이드를 사용하여 빌드 플레이트 위에 펴 바르는 방식으로 작동합니다.
번역결과 18 : 분말이 퍼진 후 레이저 빔을 사용하여 3D 부품의 2D 슬라이스에 해당하는 위치에서 분말을 선택적으로 녹입니다.
번역결과 19 : 레이스가 완료되면 빌드 플레이트가 낮아지고 다른 파우더 층이 퍼집니다(이제 기존 파우더 베드 위에 피그).
