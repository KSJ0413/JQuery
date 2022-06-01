# Attribute

* $("[속성명]") : 특정 속성을 가진 태그 
(기본이라 예제는 스킵 밑을 봐주세요!!)

* $("태그명[속성명^='값']"): 특정 속성이 지정한 값으로 시작되는 태그

<script type="text/javascript">
    $(function(){
      $("[title^='f']").css("color","red");// --> 타이틀이란 tag에서 f로 시작하는 <li>의 색을 레드로 지정한다.
    });
  </script>
 </head>
<body>
<<<<<<< HEAD

=======
>>>>>>> ff5f80debf8c209be43bf247925e869e21037690
    <ul>
    <li title="first"> 텍스트 텍스트 텍스트 텍스트 텍스트 </li>
    <li title="second"> 텍스트 텍스트 텍스트 텍스트 텍스트 </li>
    <li title="third"> 텍스트 텍스트 텍스트 텍스트 텍스트 </li>
    <li title="fourth"> 텍스트 텍스트 텍스트 텍스트 텍스트 </li>
    </ul>
<<<<<<< HEAD

  * $("태그명[속성명$='값']") : 특정 속성이 지정한 값으로 끝나는 태그

  <body>

<input name="newsletter">
<input name="milkman">
<input name="jobletter">

<script>
$( "input[name$='letter']" ).val( "a letter" );// --> name이 letter로 끝나는 input 태그의  "a letter" 값을 준다.
</script>

</body>

  *  $("태그명[속성명*='값']") :특정 속성이 지정한 값을 포함하고 있는 태그

  <body>

=======
  
  * $("태그명[속성명$='값']") : 특정 속성이 지정한 값으로 끝나는 태그
  
  <body>
 
<input name="newsletter">
<input name="milkman">
<input name="jobletter">
 
<script>
$( "input[name$='letter']" ).val( "a letter" );// --> name이 letter로 끝나는 input 태그의  "a letter" 값을 준다.
</script>
 
</body>
  
  *  $("태그명[속성명*='값']") :특정 속성이 지정한 값을 포함하고 있는 태그
  
  <body>
 
>>>>>>> ff5f80debf8c209be43bf247925e869e21037690
<input name="man-news">
<input name="milkman">
<input name="letterman2">
<input name="newmilk">
<<<<<<< HEAD

<script>
$( "input[name*='man']" ).val( "has man in it!" );//--> name에 man이란 단어가 들어간 input태그의 "has man in it!"값을 준다.
</script>

</body>


  * $("태그명[속성 ~= 값]") : 공백으로 구분된 주어진 단어를 포함하는 값으로 지정된 속성이 있는 요소를 선택

  <body>

=======
 
<script>
$( "input[name*='man']" ).val( "has man in it!" );//--> name에 man이란 단어가 들어간 input태그의 "has man in it!"값을 준다.
</script>
 
</body>
  
  
  * $("태그명[속성 ~= 값]") : 공백으로 구분된 주어진 단어를 포함하는 값으로 지정된 속성이 있는 요소를 선택
  
  <body>
 
>>>>>>> ff5f80debf8c209be43bf247925e869e21037690
<input name="man-news">
<input name="milk man">
<input name="letterman2">
<input name="newmilk">
<<<<<<< HEAD

<script>
$( "input[name~='man']" ).val( "mr. man is in it!" );//-->  name에 (공백man)이와 같이 앞에 공백이 있는 input 태그의 val값을 준다
</script>

</body>


  *  $("태그[속성 |= 값]") : 값이 주어진 문자열과 같거나 해당 문자열로 시작하여 하이픈(-)이 오는 지정된 속성이
    있는 요소를 선택한다.

  <body>

<a href="example.html" hreflang="en">Some text</a>
<a href="example.html" hreflang="en-UK">Some other text</a>
<a href="example.html" hreflang="english">will not be outlined</a>

<script>
jQuery( "a[hreflang |= 'en']" ).css( "border", "3px dotted green" );//--> a태그의 hreflang의 값이 주어진 문자열과 같거나 아이픈(-)이 오는 en 값을 찾아 테두리(border)를 주고 3px짜리 초록색 점을 테두리를 따라 둘러준다.(설명이 길었습니다... 3px 초록 점 테두리)
</script>
</body>
=======
 
<script>
$( "input[name~='man']" ).val( "mr. man is in it!" );//-->  name에 (공백man)이와 같이 앞에 공백이 있는 input 태그의 val값을 준다
</script>
 
</body>
  
  
  *  $("태그[속성 |= 값]") : 값이 주어진 문자열과 같거나 해당 문자열로 시작하여 하이픈(-)이 오는 지정된 속성이
  있는 요소를 선택한다.
  
  <body>
 
<a href="example.html" hreflang="en">Some text</a>
<a href="example.html" hreflang="en-UK">Some other text</a>
<a href="example.html" hreflang="english">will not be outlined</a>
 
<script>
jQuery( "a[hreflang |= 'en']" ).css( "border", "3px dotted green" );//--> a태그의 hreflang의 값이 주어진 문자열과 같거나 아이픈(-)이 오는 en 값을 찾아 테두리(border)를 주고 3px짜리 초록색 점을 테두리를 따라 둘러준다.(설명이 길었습니다... 3px 초록 점 테두리)
</script>
 
</body>
>>>>>>> ff5f80debf8c209be43bf247925e869e21037690
