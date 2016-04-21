**`jQuery AdubyTree Plugin `**
  * version: 5.0 (2011-05-20)
  * 
  * Copyright (c) 2011, Crystal, shimingxy@163.com
  * Dual licensed under the MIT and GPL licenses:
  * `http://www.opensource.org/licenses/mit-license.php`
  * `http://www.gnu.org/licenses/gpl.html`
  * Date: 2011-05-20 rev 13


---

**`AdubyTree Plugin  based jquery,Simple and util Utility 、OpenSource and FREE.`**

> _support XML and JSON._

> _support local data and remote AJAX data._

> _support checkbox that you need.,checkbox can before or after the leaf node._

> _support three style,simple、strengthen、extend._

> _have `Basic、Sample、Books、Org、OrgUser、Vista` six themes，you can custom themes youself._

> _have Context Menu with user function define,you can move node use Context Menu._

> Homepage&Blog:

> http://blog.163.com/shimingxy/

> any questions ,you can visite

> demo:
> > http://0070.freejsp.net/0103/


> download source:

> http://code.google.com/p/jquery-adubytree/


**`AdubyTree Plugin基于JQuery框架，实用，调用简单，基于开源协议，免费使用。`**


> _支持XML和JSON两种数据格式_

> _支持本地数据和动态AJAX远程数据。_

> _支持checkbox复选框，方便实际应用,checkbox叶节点的前面或者后面。_

> _支持三种样式，简单样式、增强样式和扩展样式。_

> _自带`Basic、Sample、Books、Org、OrgUser、Vista`六套主题，用户可以扩展定制主题。_

> _支持右键菜单，可自定义事件，可通过右键菜单移动节点。_

> 项目博客：

> http://blog.163.com/shimingxy/

> demo:

> http://0070.freejsp.net/0103/


> 源代码的下载:

> _http://code.google.com/p/jquery-adubytree_




---

**Screenshot**

<img src='http://jquery-adubytree.googlecode.com/files/adubytree5themes.gif' border='0' width='700' />
<br><br>
<img src='http://jquery-adubytree.googlecode.com/files/adubytree5style.gif' border='0' width='700' />
<hr />
<b>How to use</b>

在网页的头加入js和css,在body中加入adubytree的定义标签<code>&lt;div id="adubytree" &gt;&lt;/div&gt;</code>
<pre><code><br>
&lt;html&gt;<br>
<br>
&lt;head&gt;<br>
<br>
&lt;script src="jquery.js" type="text/javascript"&gt;<br>
<br>
Unknown end tag for &lt;/script&gt;<br>
<br>
<br>
<br>
&lt;script src="jquery.easing.1.3.js" type="text/javascript"&gt;<br>
<br>
Unknown end tag for &lt;/script&gt;<br>
<br>
<br>
<br>
&lt;script src="jquery.adubytree.js" type="text/javascript"&gt;<br>
<br>
Unknown end tag for &lt;/script&gt;<br>
<br>
<br>
<br>
&lt;link rel="StyleSheet" href="themes/basic/adubytree.css" type="text/css" /&gt;<br>
<br>
<br>
<br>
Unknown end tag for &lt;/head&gt;<br>
<br>
<br>
<br>
&lt;body&gt;<br>
<br>
&lt;div id="adubytree" &gt;<br>
<br>
Unknown end tag for &lt;/div&gt;<br>
<br>
<br>
<br>
<br>
<br>
Unknown end tag for &lt;/body&gt;<br>
<br>
<br>
<br>
<br>
<br>
Unknown end tag for &lt;/html&gt;<br>
<br>
<br>
<br>
</code></pre>
<br>
Aduby code<br>
<pre><code><br>
$("#adubytree").AdubyTree({<br>
<br>
url:"",//if you want get data from server,set url,else load data from data param<br>
id:"-1",//if url param is set,send the root id to server<br>
type: "GET",//if url param is set,the POST method ,GET or POST,default is GET<br>
dataType:"json",//datatype json、xml，default is json<br>
checkboxes:true,//is use checkbox,true is user,false is not,default is false<br>
themes	: "themes/vista/images/",//default is "themes/basic/images/"<br>
data:"dataEg",//if url param is set ,not need set data<br>
treeType:"simple",//simple、strengthen、extend,default is extend<br>
checkboxPos:"before",//checkbox position before or after,default is before<br>
cookie: true,//Is use cookie,true or false<br>
themes:"Basic",//Basic,Sample,Books,Org,OrgUser,Vista six themes<br>
onSelected:function(node){<br>
//selected node add you code,node is return Node type<br>
},<br>
onClick:function(node){<br>
//onClick node add you code,node is return Node type<br>
},<br>
onDblClick:function(node){<br>
//onDblClick node add you code,node is return Node type<br>
}<br>
onCBXClick:function(node){<br>
//onCBXClick node add you code,node is return Node type<br>
},<br>
onCBXDblClick:function(node){<br>
//onCBXDblClick node add you code,node is return Node type<br>
},<br>
onMouseOver:function(node){<br>
//onMouseOver node add you code,node is return Node type<br>
},<br>
onMouseOut:function(node){<br>
//onMouseOut node add you code,node is return Node type<br>
},<br>
onOpen:function(node){<br>
//onOpen node add you code,node is return Node type<br>
},<br>
onAddNewNode:function(node){<br>
//onAddNewNode add you code,click contextMenu add<br>
},<br>
onEditNode:function(node){<br>
//onEditNode node add you code,click contextMenu Edit<br>
},<br>
onMoveNode:function(node){<br>
//onMoveNode node add you code,click contextMenu Move<br>
},<br>
onMoveToNextNode:function(node){<br>
//onMoveToNextNode node add you code,click contextMenu MoveToNext<br>
<br>
},<br>
onMoveToChildNode:function(node){<br>
//onMoveToChildNode node add you code,click contextMenu MoveToChild<br>
<br>
},<br>
onDeleteNode:function(node){<br>
//onDeleteNode node add you code,click contextMenu delete<br>
<br>
}<br>
});<br>
</code></pre>
<br>
Opration function<br>
<pre><code><br>
open all tree items<br>
$("#adubytree").openAll();<br>
<br>
close all tree  items<br>
$("#adubytree").closeAll();<br>
<br>
get the  node you give the nodeid<br>
$("#adubytree").getNode(nodeid)<br>
<br>
get the current selected node id<br>
$("#adubytree").getSelected()<br>
<br>
add node to adubtytree pid is nodeid<br>
node ={<br>
id : "node-3-1-1-2" ,<br>
data: "node3.1.1.2",<br>
};<br>
node.id=node.id+"-"+x;<br>
node.data=node.data+"-"+x;<br>
$("#adubytree").addNode(node,nodeid);<br>
<br>
modify node when id eq nodeid,value is in node<br>
$("#adubytree").modify(nodeid,node)<br>
<br>
remove the Node id eq nodeid<br>
$("#adubytree").removeNode(nodeid);<br>
<br>
get all checkbox checked item ids<br>
$("#adubytree").getChecked()<br>
<br>
refresh the adubytree<br>
$("#adubytree").refresh();<br>
</code></pre>
<br>
dataEg<br>
JSON<br>
<pre><code><br>
var jsondata ={id : "node-0" , data: "C:",<br>
children: [<br>
{ id : "node-1" ,data: "node1",<br>
children: [<br>
{ id : "node-1-1" ,data: "node1.1",<br>
children: [<br>
{ id : "node-1-1-1" ,data: "node1.1.1"},<br>
{ id : "node-1-1-2" ,data: "node1.1.2"}<br>
]},<br>
{id : "node-1-2" , data: "node1.2"},<br>
{id : "node-1-3" ,data: "node1.3"}<br>
]<br>
},<br>
{id : "node-2" ,data: "node2"},<br>
{id : "node-3", data: "node3",<br>
children: [<br>
{ id : "node-3-1" ,data: "node3.1",<br>
children: [<br>
{id : "node-3-1-1" , data: "node3.1.1",<br>
children: [<br>
{ id : "node-3-1-1-1" , data: "node3.1.1-1"},<br>
{ id : "node-3-1-1-2" , data: "node3.1.1-2"}<br>
]<br>
}<br>
]<br>
}<br>
]<br>
}<br>
]<br>
};<br>
</code></pre>
XML<br>
<pre><code><br>
var xmldata ='&lt;?xml version="1.0"?&gt;&lt;root&gt;';<br>
xmldata +="&lt;id&gt;node-1<br>
<br>
Unknown end tag for &lt;/id&gt;<br>
<br>
&lt;data&gt;c:<br>
<br>
Unknown end tag for &lt;/data&gt;<br>
<br>
&lt;children&gt;";<br>
xmldata +=		"&lt;node&gt;&lt;id&gt;node-1-1<br>
<br>
Unknown end tag for &lt;/id&gt;<br>
<br>
&lt;data&gt;node-1-1<br>
<br>
Unknown end tag for &lt;/data&gt;<br>
<br>
<br>
<br>
Unknown end tag for &lt;/node&gt;<br>
<br>
";<br>
xmldata +=		"&lt;node&gt;&lt;id&gt;node-1-2<br>
<br>
Unknown end tag for &lt;/id&gt;<br>
<br>
&lt;data&gt;node-1-2<br>
<br>
Unknown end tag for &lt;/data&gt;<br>
<br>
<br>
<br>
Unknown end tag for &lt;/node&gt;<br>
<br>
";<br>
xmldata +=		"&lt;node&gt;&lt;id&gt;node-1-3<br>
<br>
Unknown end tag for &lt;/id&gt;<br>
<br>
&lt;data&gt;node-1-3<br>
<br>
Unknown end tag for &lt;/data&gt;<br>
<br>
&lt;children&gt;";<br>
xmldata +=			"&lt;node&gt;&lt;id&gt;node-3-1<br>
<br>
Unknown end tag for &lt;/id&gt;<br>
<br>
&lt;data&gt;node-3-1<br>
<br>
Unknown end tag for &lt;/data&gt;<br>
<br>
&lt;children&gt;";<br>
xmldata +=				"&lt;node&gt;&lt;id&gt;node-3-1-1<br>
<br>
Unknown end tag for &lt;/id&gt;<br>
<br>
&lt;data&gt;node-3-1-1<br>
<br>
Unknown end tag for &lt;/data&gt;<br>
<br>
<br>
<br>
Unknown end tag for &lt;/node&gt;<br>
<br>
";<br>
xmldata +=				"&lt;node&gt;&lt;id&gt;node-3-1-2<br>
<br>
Unknown end tag for &lt;/id&gt;<br>
<br>
&lt;data&gt;node-3-1-2<br>
<br>
Unknown end tag for &lt;/data&gt;<br>
<br>
<br>
<br>
Unknown end tag for &lt;/node&gt;<br>
<br>
";<br>
xmldata +=			"<br>
<br>
Unknown end tag for &lt;/children&gt;<br>
<br>
<br>
<br>
Unknown end tag for &lt;/node&gt;<br>
<br>
";<br>
xmldata +=		"&lt;node&gt;&lt;id&gt;node-3-2<br>
<br>
Unknown end tag for &lt;/id&gt;<br>
<br>
&lt;data&gt;node-3-2<br>
<br>
Unknown end tag for &lt;/data&gt;<br>
<br>
<br>
<br>
Unknown end tag for &lt;/node&gt;<br>
<br>
";<br>
xmldata +=	"<br>
<br>
Unknown end tag for &lt;/children&gt;<br>
<br>
<br>
<br>
Unknown end tag for &lt;/node&gt;<br>
<br>
";<br>
xmldata +="<br>
<br>
Unknown end tag for &lt;/children&gt;<br>
<br>
<br>
<br>
Unknown end tag for &lt;/root&gt;<br>
<br>
";<br>
</code></pre>

<hr />
<b>adubytreeWeb</b>
<pre><code><br>
is eclipse Project ,you can import to eclipse workspace<br>
<br>
is include src,WebRoot<br>
<br>
lib<br>
<br>
commons-logging-1.1.1.jar<br>
<br>
Apache Commons Logging<br>
<br>
Copyright 2003-2007 The Apache Software Foundation<br>
<br>
<br>
This product includes software developed by<br>
<br>
The Apache Software Foundation (http://www.apache.org/).<br>
<br>
flexjson-2.0.jar<br>
<br>
Apache License Version 2.0, January 2004<br>
<br>
http://www.apache.org/licenses/<br>
<br>
http://flexjson.sourceforge.net/<br>
</code></pre>
<b>adubytreeWeb.war</b>
<pre><code><br>
deploy to tomcat ,or copy to $TOMCAT_HOME$/webapps<br>
<br>
visit url http://website:port/adubytreeWeb/demo.html<br>
<br>
http://website:port/adubytreeWeb/themesdemo.html<br>
<br>
http://website:port/adubytreeWeb/styledemo.html<br>
<br>
http://website:port/adubytreeWeb/ajaxdemo.html<br>
</code></pre>
