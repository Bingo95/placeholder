# placeholder
ie8下placeholder无效解决，原生js<br/>
1.ie兼容h5引入html5shiv.js，respond.min.js<br/>
>><script src="https://oss.maxcdn.com/libs/html5shiv/3.7.0/html5shiv.js"></script><br/>
>><script src="https://oss.maxcdn.com/libs/respond.js/1.3.0/respond.min.js"></script><br/>
2.附加时是absolute属性，因此页面大小改变时需要重新定位<br/>
>>window[_event](_eventadd + 'resize', function() {<br/>
&nbsp;&nbsp;_placeholder.removediv('iEnew_placeholder');<br/>
&nbsp;&nbsp;_placeholder.add('input').add('textarea');<br/>
})
