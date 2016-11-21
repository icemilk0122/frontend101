這份文件是由Wes Chuang所維護，主要內容是紀錄前端教學時所用到的一些範例

<h2>Lesson 0:</h2>
1. 編輯器安裝: [Atom](https://atom.io/)
2. 版本管理及網頁空間: [github](https://pages.github.com/)

<h2>Lesson 1:</h2>
1. 網頁基本架構與[CSS基礎](http://zh-tw.learnlayout.com/)
2. 簡單的navbar, content, footer架構範例
3. [Bootstrap](http://getbootstrap.com/) ([中文版](https://kkbruce.tw/bs3)) + RWD - [教學](http://www.w3schools.com/bootstrap/default.asp)
[表單練習](https://docs.google.com/forms/d/e/1FAIpQLSfKvag9jDCytky9ZAXuVP4TJItfY0MTuF6XffwoltLc8vN41w/viewform?usp=send_form)
4. 補充fixed navbar和sticky footer範例

<h2>Lesson 2:</h2>
1. 表單製作
   ```
   TextBox    (最基本的)

Html定義
<input type="text" name="text1" value="text" test="測試用" /> 

取值
$('input[name="text1"]').val();
取自訂屬性
$('input[name="text1"]').attr("test");
設定值
$('input[name="text1"]').val("text123");
設定自訂屬性
$('input[name="text1"]').attr("test","測試用123");

Checkbox

Html定義
<label>
<input type="checkbox" name="check1" value="a" test="b" />Check
</label>

取值
$('input[name="check1"]').val()
取自訂屬性
$('input[name="check1"]').attr("test")
取得是否被勾選
$('input[name="check1"]').prop("checked");
設定值
$('input[name="check1"]').val("text123");
設定自訂屬性
$('input[name="check1"]').attr("test","測試用123");
設定勾選
$('input[name="check1"]').prop("checked",true);

RadioButton

Html定義
<label><input type="radio" name="radio1" value="0" text="test1" checked />測試</label>
<label><input type="radio" name="radio1" value="1" text="test2" />實作</label>

取得現在選取的值
$('input[name="radio1"]:checked').val()
取現在選取的自訂屬性
$('input[name="radio1"]:checked').attr("text")
設定測試為勾選狀態
$('input[name="radio1"][value="0"]').prop("checked",true);
取得此欄位是否為勾選狀態
$('input[name="radio1"][value="0"]').is(':checked')

Dropdownlist

Html定義
<select name="select1">
    <option value="val1" Text="text1" test="test1" >1</option>
    <option value="val2" Text="text2" test="test2" SELECTED>2</option>

</select>

取得現在選取的值
$('select[name="select1"]').val()
取得現在選取的自訂屬性 (兩種都可以)
$('option:selected', 'select[name="select1"]').attr('test');
$( 'select[name="select1"] :selected').attr('test');
設定現在選取的值 (兩種效果一樣)
$('select[name="select1"]').val("val1");
$('select[name="select1"]').val("1");
取得此選項是否為勾選狀態
$('select[name="select1"] option[value="val2"]').is(':selected');
取所有option 看是否為勾選
$('select[name="select1"] option').each(function(){
    alert($(this).is(':selected'));

});
```
2. jquery
3. 串接api
   [googlesheet](https://developers.google.com/sheets/quickstart/js)
4. FB登入
5. jquery plugin

