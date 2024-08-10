## Summary
- To imporove Seq2seq models ( Gradient 소실 문제 )

## Method
- ![image](https://github.com/user-attachments/assets/73e19421-396c-4989-ae54-e7bd9670d6a8)
1. Input to the Encoder
2. Encoder
  1. Self-attention
     - Self-attention is the method the Transformer uses to bake the “understanding” of other relevant words into the one we’re currently processing.    
  3. Feed Forward
4. 



## Misc.
​▷코사인 유사도 (Cosine Similarity)
내적을 통해 세타 값을 찾고, 세타 값이 90도에 가까울 수록 관련이 없음 


- 일반적인 거리 (유클리드 거리)에 의한 분류는, 문서에서 각 단어의 등장횟수만 다르고 분포가 같다면,거리가 많이 떨어지게 되어 다른 종류의 문서로 분류하지만, 각도에 의한 거리로 재면 서로 비슷한 방향의 벡터로서 각도 거리는 가깝게 되어 같은 종류의 문서로 분류할 수 있다.
출처 : 인공지능신문(https://www.aitimes.kr)

​▷내적 유사도 (Dot Product Similarity)
- ​각각의 벡터의 길이가 비슷한 경우라면, 벡터의 내적만으로도 유사도를 쉽게 구할 수 있다. 하지만 아니라면?

▷어텐션 메카니즘의 내적 유사도(Dot Product Similarity of Attention Mechanism)
   - ​Attention은 Keys Values가 준비된 상태에서 Query에 대하여 적절한 Value를 얻는 것이 목적이다.
   - Query와 Key의 비슷한 정도의 score를 Query 벡터와 Key 벡터의 dot product를 이용하여 비슷한 정도를 계산하는데 사용
   출처 : 인공지능신문(https://www.aitimes.kr)


## Reference
- 출처 : 인공지능신문(https://www.aitimes.kr)
- https://jalammar.github.io/illustrated-transformer/




