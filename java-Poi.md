### apache poi
* 엑셀 파일 읽어 DB 저장하기
1. 이미 있는 엑셀 파일을 사용해서 workbook 인스턴스를 생성한다.

2. 해당 workbook에서 원하는 sheet를 가져온다.

3. sheet내에서 읽고자 하는 행 번호를 지정한다.

4. row에 있는 모든 cell을 순회하면서 읽는다.

5. 3과 4의 과정을 sheet 내의 모든 행을 읽을 때까지 반복한다.

- List<Map<String, String>> excelContent - ex Map<"cell의 이름","cell의 값">
- vo.setData(excelContent)
- Mydatis insert 파라미터 data.key값
* 참고
  * [[Spring] Excel 파일 업로드/ import / 엑셀업로드 / 첨부파일 / 엑셀 값 읽기 / Java](https://daydreamer-92.tistory.com/42)
  * [[java] poi 활용하여 excel upload 후 db insert / excel upload and DB insert](https://take-it-into-account.tistory.com/175)
  * [[2020.01.30] Excel upload 후 db저장](https://eugene-kim.tistory.com/46)
  * [[Java] 대용량 Insert 상세 설명 (Batch, Dynamic sql)](https://chobopark.tistory.com/306)
