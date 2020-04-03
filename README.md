# 纪念日网站变灰浏览器全兼容方案

#-----------------------------------------------------------------------------------------
/*
* 网站变灰代码
*/
html{
filter: grayscale(100%);
-webkit-filter: grayscale(100%);
-moz-filter: grayscale(100%);
-ms-filter: grayscale(100%);
-o-filter: grayscale(100%);
filter: url("data:image/svg+xml;utf8,&lt;svg xmlns='http://www.w3.org/2000/svg'&gt;&lt;filter id='grayscale'&gt;&lt;fecolormatrix type='matrix' values='0.3333 0.3333 0.3333 0 0 0.3333 0.3333 0.3333 0 0 0.3333 0.3333 0.3333 0 0 0 0 0 1 0'&gt;&lt;/fecolormatrix&gt;&lt;/filter>&lt;/svg&gt;#grayscale");
filter:progid:DXImageTransform.Microsoft.BasicImage(grayscale=1);
-webkit-filter: grayscale(1);
}
body{
	filter: grayscale(100%);/*火狐*/
    -webkit-filter:grayscale(100%);/*chrome*/
    filter:gray; /*IE7-9*/
}

<script type="text/javascript" src="./grayscale.js"></script>
<script type="text/javascript">
window.onload=function(){
    grayscale(document.body);
}
</script>
