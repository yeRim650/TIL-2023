### Bean validation
* @RequestBody - Request의 Body에 있는 값(JSON)을 사전에 정의한 Request 객체로 바인딩 @Valid를 통해 validator가 이 객체의 유효성 검사를 진행
* (JpaRepository를 상속시 @Repository없이도 잘 등록된다)
* @Column annotation으로 제약조건을 정의했는데 이 내용은 DB 필드에 적용되는 값으로 유효성 검사와는 상관이없다.
* 필요한 제약조건은 custom annotation을 만들어서 사용 가능
* @PathVariable, @RequestParam 사용시 @Validated를 컨트롤러 클래스에 적용하면 유효성 검사 가능
