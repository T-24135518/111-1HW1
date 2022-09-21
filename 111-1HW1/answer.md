# 第1次作業-作業-HW1
>
>學號：109111122
><br />
>姓名：蔡旻蓉
><br />
>作業撰寫時間：10 (mins，包含程式撰寫時間)
><br />
>最後撰寫文件日期：2022/09/21
>

本份文件包含以下主題：(至少需下面兩項，若是有多者可以自行新增)
- [x]說明內容
- [x]個人認為完成作業須具備觀念

## 說明程式與內容

依據readme的要求先在Test.aspx.cs輸入Response.Write("Hello App")在切換至Test.aspx拉出一個按鈕更改id後
雙擊按鈕就可以輸入Response.Write("Hello Buttom")，執行該程式後，在按下上網頁的按鈕，會在Hello App後面加入Hello Buttom
<br>下段程式碼則為使用後結果：

```csharp
protected void Page_Load(object sender, EventArgs e)
        {
            Response.Write("Hello App");
        }

        protected void btn_Show_Click(object sender, EventArgs e)
        {
            Response.Write("Hello Buttom");
        }
```

根據readme的要求在Test.aspx的檔案，拉出一個按鈕插入至div，並將ID更改為btn_Show，
下段程式碼則為使用後結果：

```html
<%@ Page Language="C#" AutoEventWireup="true" CodeBehind="Test.aspx.cs" Inherits="_111_1HW1.Test" %>

<!DOCTYPE html>

<html xmlns="http://www.w3.org/1999/xhtml">
<head runat="server">
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title></title>
</head>
<body>
    <form id="form1" runat="server">
        <div>
            <asp:Button ID="btn_Show" runat="server" Text="Button" OnClick="btn_Show_Click" />
        </div>
    </form>
</body>
</html>

```


## 個人認為完成作業須具備觀念

需要熟悉建立web表單及git的使用方式，要在Test.aspx使用工具箱拉出按鈕插入至div，並在屬性處更改id後雙擊切換至Test.aspx.cs在btn_Show_Click裡輸入程式碼。

