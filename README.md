
# 1. Success Prediction

- Predict success or not with information before project begins
- Features : target_money, grammar_level, has_video, funding_type_count, funding_type_1, funding_type_2, funding_type_3, funding_duration

### ※Estimation of grammar_level

- number of errors / number of tokens
- tested by naver grammar tester (https://github.com/ssut/py-hanspell)
- suppposed grammar level represents ability of creators

## Outline

- Check the insight from previous project (https://github.com/surprisoh/crowdfunding_prediction)
- Distribution test
- Feature selection
- Model Selection (classification)
- Grid Search & Scores
- Optimum model selection
- Result & Insight

# 2. Crowd Funding Recommender system

## Idea
- For new crowd funding projects, there are no such classificable factors with old projects (I suppose category is not a key factor)
- Users are only interested in a project itself (Funding target money, duration, etc are non of their business)
- Doc2vec is a quite logical method to classify documents
- Classifying descriptions of projects by using Doc2vec -> Recommending 10 nearest projects with a project users clicked or supported

## Outline
- Tokenizing description
- Run Doc2vec
- Calculate distance of each project combinations
- Recommend

## Insight
- 새로 개설되는 (user 정보, item 정보가 없는)프로젝트들의 연관성을 파악할 수 있을까에 대한 의문에서 출발한 실험적인 모델입니다.
- 각 유저별 프로젝트 선택 목록, 웹 사이트내 행동 패턴 등과 결합하면 더욱 의미있는 모델이 될 것입니다.


