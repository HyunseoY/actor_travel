# 🌈내일배움캠프 B-10조 미니프로젝트 S.A.

### 팀명

### `P4J1`

### 팀소개

| 이름 | 구분 | 역할 |
| --- | --- | --- |
| 신민수 | 팀장 | 댓글창 |
| 송희진 | 팀원 | 리뷰카드  |
| 이소영 | 팀원 | 리뷰카드/api/BGM기능 |
| 양현서 | 팀원 | 작품 슬라이드/api |
| 김진성 | 팀원 | 리뷰카드/api |

## 미니프로젝트 회의

### 주제

- 영화 배우 소개 및 해당 배우의 대표작품 리뷰 작성 서비스

### 프로젝트명

### 📽️출발! 배우여행

### 간단설명

- 영화 배우 소개 [김혜수] 배우로 특정한 페이지
- 리뷰카드 작성시 이미지,작품제목,별점,코멘트 함께 나오도록 생성
- 명언 모달창으로 뜨게 구현
- 대표작품 외의 클라이언트가 다른 작품 및 명대사를 작성하는 댓글창 구현
- 페이지에 2005 갬성의 향수를 불러일으키는 “프리스타일-Y”노래 삽입 (미니홈피)

### 와이어 프레임

페이지1] 배우소개 

![https://blog.kakaocdn.net/dn/bbI6cm/btses4UFYju/N3ZMmyPnSlRMIHcFo2UBk1/img.png](https://blog.kakaocdn.net/dn/bbI6cm/btses4UFYju/N3ZMmyPnSlRMIHcFo2UBk1/img.png)

페이지2] 작품리뷰

![https://blog.kakaocdn.net/dn/sjdxO/btseqc7suA6/QoKxwk6YzUbWpHkwXKKsCK/img.png](https://blog.kakaocdn.net/dn/sjdxO/btseqc7suA6/QoKxwk6YzUbWpHkwXKKsCK/img.png)

## API Table

| Number | Method | URL | Description | Request | Response |
| ------ | ------ | --- | ----------- | ------- | -------- |
| 1 | POST | /api/save_review | 작성된 리뷰 저장 | {"movie": movie, "comment": comment, "star": star, "imageUrl": imageUrl} | return "Success” |
| 2 | GET | /api/get_reviews | 작성된 리뷰 불러오기 | review_data = list(db.reviews.find({}, {"_id": 0})) | return jsonify(review_data) |
