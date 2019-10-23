# Code Review Class

## 구성원 간에 Coding Guideline 합의를 도출하고 문서로 남긴다
* 하이퍼텍스트로 각 항목을 링크할 수 있게 하라
* 링크를 언급하 간략히 리뷰 가능
* https://mtlynch.io/human-code-reviews-1/

## 코드 리뷰는 코드에 대한 리뷰이지 코드 작성자에 대한 리뷰가 아니다
* https://www.processimpact.com/articles/humanizing_reviews.pdf

## 무엇을 리뷰할까?
### Code Invariant에 기반한 함수/클래스별 체크 사항
* thread-safe or not
* may block (schedule) or not
* run in bounded time or not
* throws exception or not
* stateless or not (has side effect which is hard to spot)

### 커밋 로그도 리뷰의 대상이다
* 리누스 토발즈의 가이드: https://github.com/torvalds/subsurface-for-dirk/blob/a48494d2fbed58c751e9b7e8fbff88582f9b2d02/README#L88
* 커밋 로그는 충분히 길게: https://github.com/torvalds/linux/commit/1b7e816fc80e668f0ccc8542cec20b9259abace1#diff-b3cd915d758008bd19d0f2428fbb354a


### 코드 구조/맥락의 파악이 힘들다면 그것도 리뷰다
* clean code의 룰에 부합하는지 
