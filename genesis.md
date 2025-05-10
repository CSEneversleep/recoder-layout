##  필요 역할

- frontend
: basis
벡엔드에게서 사진을 받아서 띄운다!
기깔나는 디자인을 만든다
사진 업로드 기능을 구현한 뒤, 사진 데이터와 사진 메타데이터를 서버에 떤진다

/show
/slide?name=???&date=???
{
    photos: [
        {
            image url:
            lattitude: 
            longitude:
            title:
            description:
            created at:
            peoples: [
                { name: },
                { name: }, ...
            ]
        },
    ]
}
서버가 이미지 목록 보내주면 그거 슬라이드로 보여주기

: map
/map
{
    locations: [
        { 
            folder:
            title: 
            lattitude: 
            longitude:
            redirect_to:
        },
        { 
            folder:
            title: 
            lattitude: 
            longitude:
            redirect_to:
        },
    ]
}
사진에서 위치 정보를 받아온 뒤 지도에 표시한다

/upload/one
/upload/multi
: multi upload (fwd: 김인서)
사진을 한번에 여러개 선택할 시 발동
openai api에 가서 사진 정보 요약을 받는다
그 정보를 기본으로 설정한다
유저는 confirm만 하고 업로그 하게

+
사람이 감지되면, 이름 자동 입력력

- backend
사진 업로드 받으면 처리한다
사진 url을 제공한다
대충 {image url, location, title, description, created at} 정도 있으면 되지 않을까

만약 location 모음집만 요청하면, 요청을 받는다.
