<div align="center">

## Add parameter to URL


</div>

### Description

This example uses a javascript to append a value entered into a text box to a URL request. The URL is passed in the form of a query string parameter and is launched from an Anchor tag.

http://www.truegeeks.com/asp/mam/osdoc/osframe.asp
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[N/A](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/empty.md)
**Level**          |Beginner
**User Rating**    |4.0 (20 globes from 5 users)
**Compatibility**  |
**Category**       |[Internet/ Browsers/ HTML](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/internet-browsers-html__2-68.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/add-parameter-to-url__2-1775/archive/master.zip)





### Source Code

```

<HTML>
<HEAD></HEAD>
<SCRIPT Language="JavaScript">
<!--
function Validator(lURL) {
var oform = document.form1
var qsparm = oform.TB1.value
if (qsparm == "") {
  alert("You must provide a value")
  oform.TB1.focus()
  return false }
document.location.href = lURL + "?" + escape(qsparm)
return false
}
//-->
</SCRIPT>
<BODY>
<FORM NAME="form1">
<STRONG>
QueryString Parameter:
<INPUT TYPE="TEXT" NAME="TB1">
</STRONG>
<BR><BR>
<A HREF="" onClick="return Validator('YourURL.asp')">Click me to continue </A>
</FORM>
</BODY>
</HTML>
```

