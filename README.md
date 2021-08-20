1.
<div id="dvContents" style="border: 1px dotted black; padding: 5px; width:305px">
    <table cellspacing="0" rules="all" border="1">
        <tr>
            <th>Customer Id</th>
            <th>Name</th>
            <th>Country</th>
        </tr>
        <tr>
            <td>1</td>
            <td>John Hammond</td>
            <td>United States</td>
        </tr>
        <tr>
            <td>2</td>
            <td>Mudassar Khan</td>
            <td>India</td>
        </tr>
        <tr>
            <td>3</td>
            <td>Suzanne Mathews</td>
            <td>France</td>
        </tr>
        <tr>
            <td>4</td>
            <td>Robert Schidner</td>
            <td>Russia</td>
        </tr>
    </table>
</div>
<br/>
<input type="button" onclick="PrintTable();" value="Print"/>

2.

3.

SELECT *
FROM Address
WHERE PersonId = N;

4.






















5.

TempData:

TempData用於將數據從當前請求傳遞到下一個請求
它保留 HTTP 請求時間的信息。這意味著只能從一頁到另一頁。當我們從一個控制器移動到另一個控制器或從一個動作移動到另一個動作時，它有助於維護數據
它需要對複雜數據類型進行類型轉換並檢查空值以避免錯誤。通常，它僅用於存儲錯誤消息和驗證消息等一次性消息

ViewData: 
ViewData用於將數據從控制器傳遞到視圖
它派生自 ViewDataDictionary 類
僅適用於當前請求
需要對複雜數據類型進行類型轉換並檢查空值以避免錯誤
如果發生重定向，則其值變為 null

ViewBag:
ViewBag還用於將數據從控制器傳遞到相應的視圖
ViewBag是一個動態屬性，它利用了 C# 4.0 中的新動態特性
它也僅適用於當前請求
如果發生重定向，則其值變為 null
不需要對複雜數據類型進行類型轉換

6.
授權篩選器 =IAuthorizationFilter。
操作篩選器 =IActionFilter。
結果篩選器 =IResultFilter。
異常篩選器 =IExceptionFilter。
