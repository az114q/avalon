今天的主角是ms-visible，它的效果类拟于jQuery的toggle，如果它后面跟着的表达式为真值时则显示它所在的元素，为假值时则隐藏。不过显示不是 display:none这么简单，众所周知，display拥有inline, inline-block, block, list-item, table, table-cell等十来个值，比如用户之前是让此LI元素表示inline-block，实现水平菜单效果，你直接display:block就会撑破布局。因此元素之前是用什么样式显示，需要保存下来，当表达式转换为真值时再还原。  
we are talking about ms-visible today,it works very samilarly to the jQuery toggle(),if ms-visible is set a true Expression,the element will display,otherwise it will disapper.This attr does not only toggle your element between display:none and display:block, we all know that dispaly attr has many oppional values:inline, inline-block, block, list-item, table, table-cell ETC, you can't simply toggle your element between display:none and display:block otherwise your element may not display correctly.The original display value must be saved for restoring your element the original style when ms-visible:true.  

这里用到ms-for循环指令及ms-click事件指令，语法与ng没有二致，不懂可以暂时忽略。  
this example use ms-for loop directive and ms-click event diretive,the grammar is exactly the same as ng,you may skip this if you don‘t know diretives.

再看它能否处理内联样式的干扰：  
let‘s see if it can precede over a inline style:  

我们再来一个有用的例子，做一个切换卡。
a useful example,tab switcher  