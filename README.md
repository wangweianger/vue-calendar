# vue-calendar

### Case pictures

![输入图片说明](https://git.oschina.net/uploads/images/2017/0929/170241_8561545c_818875.png "在这里输入图片标题")
![输入图片说明](https://git.oschina.net/uploads/images/2017/0929/170243_068b0494_818875.png "在这里输入图片标题")
![输入图片说明](https://git.oschina.net/uploads/images/2017/0929/170246_ee897477_818875.png "在这里输入图片标题")

### Requirements
>  * Vue.js 1.1.0 ~   适用于vue1.0版本 
>  * Vue.js 2.3.0 ~   2.0vue版本需要大于2.3.0版本

>  *依赖插件为：zane-calendar ，不依赖任何第三方插件，包大小26K


### Demo

http://www.seosiwei.com/zaneDate/index.html   //参数一致


### Instllation

```
$ npm install vue-date-calendar@1.2.0   vue1.0版本
$ npm install vue-date-calendar         vue2.0版本

```

### Usage


```

<vue-date-calendar :option.sync="option"></vue-date-calendar>


import vueDateCalendar from 'vue-date-calendar'
export default {
	components: {
	  vueDateCalendar
	},
	data(){
    return {
    	option{
    		elem:'#zane-calendar',   	控件的dom原生 注意：仅限制于id选择器     (必填,id前必须有#号)
				type:'day',   				可选类型 day year month time doubleday doubleyear doublemonth doubletime (必填)
				lang:'cn',   				可选择语言类型 cn , en  (可选)
				width:280,  				插件宽度配置   250 <= X <= 500 (可选)
				height:300, 				插件高度配置   250 <= X <= 350 (可选)
				behindTop:10,   			插件于输入框的高度  	(可选)
				format:'yyyy-MM-dd HH:mm:ss',  时间格式化 		(可选)
				value:'',  					插件初始默认值  		(参数名必须，双向绑定value值)
				min:'',  					  可选取时间最小范围 1900-10-01 (可选)
				max: '',  					可选取时间最大范围 	2099-12-31 (可选)
				zindex:100,   				z-index值 (可选)
				showtime:true,  			是否显示选择时间 (可选)
				showclean:true,  			是否显示清除按钮 (可选)
				shownow:true,  				是否显示当前按钮 (可选)
				showsubmit:true, 			是否显示提交按钮 (可选)
				haveBotBtns:true, 			是否有底部按钮列表 (可选)
				calendarName:'', 			此参数勿动 表示当前时间插件实例化对象 (可选)
				mounted:()=>{}, 			插件加载完成之后调用 (可选)
				change:()=>{}, 				时间变更之后调用 (可选)
				done:()=>{}, 				选择完成之后调用 (可选)
    	}
    }
	}    
}


//常用的option方式
option:{
	elem:"#demo1",
	type:'year',
	fromate:'yyyy-MM-dd'
}

option:{
	elem:"#demo2",
	type:'doubleday',
	fromate:'yyyy-MM-dd',
	showtime:true,
}

//参数配合会有很多的功能

```

### License

The MIT License












