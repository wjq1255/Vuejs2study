#### hello world 实例

	'''
		<div id="hello">
		  <p>{{ message }}</p>
		</div>
	'''

	'''
		var hello =	new Vue({
			el:"#hello",
			data:{
				message:"hello world !",
			}
		});

	'''

#### 构造器
	每个 Vue.js 应用都是通过构造函数 Vue 创建一个 Vue 的根实例 启动的。
	在实例化 Vue 时，需要传入一个选项对象，它可以包含数据、模板、挂载元素、方法、生命周期钩子等选项。

#### 属性与方法
	'''
		var data = { a: 1 }
		var vm = new Vue({
		  el: '#example',
		  data: data
		})
		vm.$data === data // -> true
		vm.$el === document.getElementById('example') // -> true
		// $watch 是一个实例方法
		vm.$watch('a', function (newVal, oldVal) {
		  // 这个回调将在 `vm.a`  改变后调用
		})
	'''

#### 实例生命周期
    每个 Vue 实例在被创建之前都要经过一系列的初始化过程。例如，实例需要配置数据观测(data observer)、编译模版、挂载实例到 DOM ，然后在数据变化时更新 DOM 。在这个过程中，实例也会调用一些 生命周期钩子 ，这就给我们提供了执行自定义逻辑的机会。

#### 生命周期图示

http://cn.vuejs.org/images/lifecycle.png