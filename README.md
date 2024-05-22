## REST api 활용한 토큰방식 로그인

- REST api 개요
로그인 방식 <br>
소셜로그인이 일반로그인과 다른 점은 로직상으로는 없다. 소셜툴을 이용했다는 것만 다르다. 즉, 어떤 경로든 jwt 발급이 되는 방식이다. <br>
rest api를 쓰면 url이 바뀐다. http method 방식을 사용한다. <br>
 
- 일반사이트 주소체계 : <br>
게시물 목록 : GET http://localhost:8080/article/list <br>
게시물 등록(폼) : GET http://localhost:8080/article/write <br>
게시물 등록 : POST http://localhost:8080/article/write <br>
게시물 단건 조회 : GET http://localhost:8080/article/1 <br>
게시물 수정(폼) : GET http://localhost:8080/article/1/modify <br>
게시물 수정 : POST http://localhost:8080/article/1/modify <br>
게시물 삭제 : GET http://localhost:8080/article/1/delete <br>

- REST API 주소체계 : <br>
게시물 목록 : GET http://localhost:8080/articles <br>
게시물 등록 : POST http://localhost:8080/articles <br>
게시물 단건 조회 : GET http://localhost:8080/articles/1 <br>
게시물 수정 : PATCH http://localhost:8080/articles/1 <br>
게시물 삭제 : DELETE http://localhost:8080/articles/1 <br>

메소드 종류 : GET, PUT, PATCH, DELETE 등 <br>

<hr>

- 로그인 토큰방식

로그인 시 토큰을 생성한다.
![image](https://github.com/yhwit30/rest_api_2024_05/assets/153142837/7169673a-a488-4274-8b0d-da2d503da8ba)

토큰이 헤더에 잘 생성되었다.
![image](https://github.com/yhwit30/rest_api_2024_05/assets/153142837/9b577713-75f8-46e3-ac4a-c8847d004baa)


