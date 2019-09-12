---
description: >-
  이 문서의 허가되지 않은 무단 복제나 배포 및 출판을 금지합니다. 본 문서의 내용 및 도표 등을 인용하고자 하는 경우 출처를 명시하고
  김종민(kimjmin@gmail.com)에게 사용 내용을 알려주시기 바랍니다.
---

# 6.7 형태소 분석 \(Stemming\)

  우리가 사용하는 언어들은 영어만 보더라도 문법에 따라 명사 뒤에 **~s**, **~ness** 등이 붙거나 동사 뒤에 **~ing**, **~ed** 등이 붙는 등 변화가 많습니다. 검색을 할 때는 보통 이런 문법에 따른 단어의 변형에 상관 없이 검색이 가능해야 하기 때문에 텍스트 데이터를 분석할 때 각각의 텀에 있는 단어들을 기본 형태인 어간을 추출하는 과정을 진행해야 합니다. 이 과정을 보통 **어간 추출** 또는 **형태소 분석** 이라고 하며 영어로는 **stemming** 이라고 합니다. 그리고 형태소 분석을 하는 도구를 형태소 분석기, 영어로는 **stemmer** 라고 합니다.

  Elasticsearch 에서는 다양한 형태소 분석기들을 지원하며 Elastic사에서 공식적으로 지원하지 않는 국가의 언어들도 플러그인 형태로 사용 가능하도록 오픈소스로 배포되는 분석기들이 많이 있습니다. Elasticsearch 에서 사용 가능한 형태소 분석기 중에서 가장 많이 알려진 형태소 분석 알고리즘인 Snowball 과 한글 형태소 분석기인 Nori에 대해 살펴보도록 하겠습니다.
