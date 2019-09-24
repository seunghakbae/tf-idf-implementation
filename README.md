# tf_idf

# TF- IDF(Term Frequency - Inverted Document Frequency)란?

TF-IDF란 1세대 정보검색 기술로 page rank가 등장하기 전 사용되었던 기술이다. 아주 간단한 정보검색을 하는 방식은 각 document에 어떤 word가 있는 지 큰 테이블에 저장하는 방식이였다. 하지만, 이런 경우 table에서 모든 document를 하나씩 검색해서 찾아야 했고, 또 각 테이블마다 모든 단어의 존재 유무 및 개수를 저장해놓고 있어야 했다. 

## Inverted Table
이렇게 되면, 단어의 수가 몇 만, 십만, 백만 개가 되고 document또한 비슷한 개수가 되면, 이 정보를 모두 가지고 있는 table을 만든다는 건 상상이 되지 않는다. 이럴 때 등장한 것이 INVERTED TABLE이다.

Inverted Table은 기준이 문서가 아니라 단어이다. 그래서, 각 단어를 기준으로 그 단어가 속한 document의 index를 linked list로 구현한 것이 inverted Table이다. 

## TF-IDF
하지만, inverted table은 그 단어가 속한 document만 보여줄 뿐, 그 단어와 document가 얼마나 연관성이 있는 지 보여주진 못한다. 그래서, 이 연관성을 보여주기 위해서 나온 것이 tf-idf이다.
