## member_search.jsp

```html
<td><input type="text" name="in_custno"></td>
```

input에 type="text"를 하여 회원번호를 입력합니다.
<br><br><br>

![image](https://user-images.githubusercontent.com/104752202/195021238-b3446156-a438-4f83-9263-272f923c5358.png)
<br><br><br>

```html
<input type="button" value="취소" onclick="location.href='index.jsp'">
```

취소 버튼을 누르면 index.jsp로 이동합니다.
<br><br><br>

```html
<input type="submit" value="조회" >
```

조회 버튼을 누르면 form 태그에 action이 호출됩니다.
<br><br><br>


```html
<form name="data1" action="member_search_list.jsp" method="post" onsubmit="return checkValue2()">
```

form 태그에 onsubmit="return checkValue2()"를 추가하여 조회 버튼을 클릭하면 checkValue2() 함수가 호출됩니다.
<br><br><br>

```javascript
<script type="text/javascript">
    function checkValue2() {
        if(!document.data1.in_custno.value) {
            alert("회원번호를 입력하세요.");
            data1.in_custno.focus();
        return false;
    } 		
    return true;
}
</script>
```

조회 버튼을 눌렀을 때 회원번호(in_custno)를 입력하지 않으면 '회원번호를 입력하세요.'라는 메시지가 출력됩니다.
<br><br><br>

## member_search_list.jsp



## sales_list.jsp

## update.jsp

## update_p.jsp

## delete.jsp
