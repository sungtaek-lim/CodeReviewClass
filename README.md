# CodeReviewClass

## 구성원 간에 Coding Guideline 합의를 도출하고 문서로 남긴다
* 하이퍼텍스트로 각 항목을 링크할 수 있게 하라
* 리뷰에서 합의된 항목의 링크를 언급하면 간략한 리뷰 가능
* https://mtlynch.io/human-code-reviews-1/

## 커밋 로그도 리뷰의 대상이다
* 리누스 토발즈의 가이드: https://github.com/torvalds/subsurface-for-dirk/blob/a48494d2fbed58c751e9b7e8fbff88582f9b2d02/README#L88
* 문제를 기술하기 위해 자세히 https://github.com/torvalds/linux/commit/1b7e816fc80e668f0ccc8542cec20b9259abace1#diff-b3cd915d758008bd19d0f2428fbb354a

## Humanizing Code Review
* https://www.processimpact.com/articles/humanizing_reviews.pdf

## Code Invariant에 기반한 함수/클래스별 체크 사항
* thread-safe or not
* may block (schedule) or not
* run in bounded time or not
* throws exception or not
* stateless or not (has side effect which is hard to spot)
