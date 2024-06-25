# youtube_restapi
django with restapi

(1) User => users
- email
- password
- nickname
- is_business

(2) Video => videos
- title
- description
- link
- views_count
- thumbnail
- video_file

ex) 파일 (이미지, 동영상) 
=> 장고에 부하가 걸림
=> S3 Bucket(저렴, 속도가 빠름) -> 결과물: 링크

(3) Reaction => reacitons
- User: foreign key
- video: foreign key
- reaction (like, dislike, cancel) => 실제 youtube rest api

(4) Comment => comments
- User: foreign key
- Video: foreign key
- content
- like
- dislike

(5) Subscription => subscriptions
- User: foreign key => subscriber
- User: foreign key => subscribed_to

(6) Common => common
- created_at
- updated_at