# EFUB-backend
# EFUB 4주차 세미나 과제

###### {프백인턴} {김명지}



### 01. 학사 정보 관리 ERD

[https://app.diagrams.net/#G1diV7tYx7HdIT78aLCRUKs6wp-HoRq-4S]

[![image](https://user-images.githubusercontent.com/88931238/162757102-e9f704df-da58-4b62-8a62-2634d7b7091d.png)
]



### 02. MySQL 실습 코드

##### SWS 테이블 생성 코드

```
SWS 테이블 생성 코드

CREATE TABLE sws (
    sws_id BIGINT NOT NULL AUTO_INCREMENT,
    team_name VARCHAR(45),
    PRIMARY KEY (sws_id)
);

INSERT INTO sws(team_name) VALUES
    ("베이커리"),
    ("라꾸라꾸"),
    ("STEADY"),
    ("이상청");
```

##### JOIN 코드

```
JOIN 코드

Select member.team_number, sws.team_name,  member.name, member.position, member.email FROM member JOIN sws ON member.team_number = sws.sws_id
```


##### JOIN 출력 결과

[![image](https://user-images.githubusercontent.com/88931238/162767135-a50984c8-ef9b-462d-8d19-6e17553539cb.png)
]
