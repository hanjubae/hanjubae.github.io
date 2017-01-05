---
layout: post
title: 쿠키를 이용한 로그인 아이디 저장(javascript)
date: 2017-01-05
---



## 쿠키를 이용한 로그인 아이디 저장(javascript)

html과 javascript를 통해 쿠키를 이요하여 아이디저장 체크박스 선택시 로그인 아이디 저장


### HTML

````````````````````````````````````````````````````````````````````````````````html
<body>
<div align="center">
 <h1>로그인 창</h1>
 <form name="myForm" method='post'>
 <table style="border: 2px solid black; padding: 5px">
   <tr>
    <th><b>ID</b></th>
    <td><input type="text" name="id" id= "user_id" size="20" required="required"></td>
   </tr>
   <tr>
    <th><b>PW</b></th>
    <td><input type="password" name="pw" id="user_password" size="20" required="required"></td>
   </tr>
   <tr>
    <td colspan="2" align="center"><input type="checkbox" name="idSave"  id="cb_saveId" value="yes">아이디저장</td>
   </tr>
   <tr>
    <td colspan="2" align="center">
    <!-- <input type="submit" size="10" value="로그인"> -->
    <input type="button" onclick="mySubmit(1)" value="로그인" size="10">
    <input type="button" onclick="mySubmit(2)" value="회원가입" size="10">
    </td>
   </tr>
  </table>
  </form>
</div>
</body>
````````````````````````````````````````````````````````````````````````````````


### JAVASCRIPT

````````````````````````````````````````````````````````````````````````````````javascript
<script type="text/javascript">
 
 ///////////////////////////////////////////////
 (function init(){

  // 쿠키값을 가져온다.
  
  var cookie_user_id = getLogin();
  
  if(cookie_user_id != "") {
  
   document.getElementById("user_id").value = cookie_user_id;
   cb_saveId.checked = true;
  }
  
 })()//생성자초럼 호출하지 않아도 바로 실행된다
 // 로그인 버튼 클릭시

 function mySubmit(index) {
  if(index==1){
   if(cb_saveId.checked == true){
    saveLogin(document.getElementById("user_id").value);
   }else{
    saveLogin("");
   }
   document.myForm.action='main.jsp';
  }
  if(index==2){
   document.myForm.action='join.html';
  }
  document.myForm.submit();
 }
 
 function saveLogin(id) {

  if(id != "") {

  // userid 쿠키에 id 값을 7일간 저장

  setSave("userid", id, 7);

  }else{

  // userid 쿠키 삭제

  setSave("userid", id, -1);

  }

 }
 
 function setSave(name, value, expiredays) {

  var today = new Date();

  today.setDate( today.getDate() + expiredays );

  document.cookie = name + "=" + escape( value ) + "; path=/; expires=" + today.toGMTString() + ";"

 }
 
 function getLogin() {

  // userid 쿠키에서 id 값을 가져온다.

  var cook = document.cookie + ";";

  var idx = cook.indexOf("userid", 0);

  var val = "";



  if(idx != -1) {

  cook = cook.substring(idx, cook.length);

  begin = cook.indexOf("=", 0) + 1;

  end = cook.indexOf(";", begin);

  val = unescape(cook.substring(begin, end));

  }

  return val;

 }

</script>
````````````````````````````````````````````````````````````````````````````````









