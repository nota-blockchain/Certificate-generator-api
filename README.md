# Certificate-generator-api



Usage
-----

### Students data file
`students_list.csv` 형식

```
a;홍길동;6월 29일,2019년;한국****진흥원
b;아무개;6월 30일,2019년,한국**진흥원
...


### PDF 생성
$ python app.py <template.svg> <students_list.csv> <base_url>


### File description:

* `template.svg`: 수료증 파일 템플릿
 * `short_name`: 파일 이름
 * `full_name` : 풀네임
 * `graduation_date`: `6월 29일, 2019년` 형태로 날짜 입력 (추후 변경하겠습니다)
 * `organization_complement`: 기관명
 * `qrcode_url`: QRCode url, PNG 투명바탕. (optional)
* `students_list.csv`: 학생 리스트/ 타입은 위에 참고 
* `base_url`: QR코드로 해당 상장을 내보낼때`<base_url>/<short_name>.pdf`. 형태로 제공되는데, 그때 사용할 baseurl
