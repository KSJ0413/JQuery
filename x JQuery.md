```
JQuery
```

* jQuery는 JavaScript Library

* jQuery는 JavaScript Library

* 간결하게 코딩하고
   많은 일을 해주는 JavaScript Library
   
   
   
   #### jQuery 스크립트
   
   * $(function () {  // 페이지 로딩될때
   
    * $("dd:not(:first)").css("display","none"); 
    // 첫번째(first) dd태그를 제외(not)한 나머지 dd태그의 display none으로 한다
    
    * $("+dd", this).slideDown("slow"); 
    // 현재 dd의 뒤(+)에 dd를 천천히 올린다

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script src="https://code.jquery.com/jquery-latest.min.js"></script>
<script>
     $(function () {//로딩
      $("dd:not(:first)").css("display", "none");// 처음 dd태그 제외한 dd태그들을 화면에 없앤다?
      $("dl dt").click(function () {// di안에있는 dt 클릭시 
        if ($("+dd", this).css("display") == "none") {
        // 만약에 dd태그 뒤에 this-->(click(function)) 클릭했을떄 화면에 아무것도 없다면? 
          $(this).siblings("dd").slideUp("slow");//this(클릭)dd의 형제자매(siblings)를 천천히 올린다
          $("+dd", this).slideDown("slow");//this(클릭) 시 dd태그 뒤에 있는 dd를 천천히 내린다
        }
      });
    });
</script>
<style>
    * {
      margin: 0;
      padding: 0;
    }
 
    dl {
      width: 400px;
      margin: 50px auto;
    }
 
    dl dt {
      background: #7CADB6;
      border-bottom: 1px solid #FFFFFF;
      cursor: pointer;
    }
 
    dl dd {
      border: 1px solid #7CADB6;
      border-top: none;
      height: 300px;
    }
</style>
</head>
<body>
    <div id="container">
        <dl>
          <dt> 텍스트1</dt>
          <dd>
            <p> 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트
              텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 </p>
          </dd>
          <dt> 텍스트 2</dt>
          <dd>
            <p> 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트
              텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 </p>
          </dd>
          <dt> 텍스트 3</dt>
          <dd>
            <p> 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트
              텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 텍스트 </p>
          </dd>
        </dl>
      </div>
</body>
</html>
```


