	小球场景
		Area2D 节点 
			用于检测范围
			可以检测其他碰撞对象和时进入、退出或重叠该区域 并在相应事件发生时发出信号
			Area2D还可用于覆盖物理属性 
				例如设置一定区域内的重力阻尼等
			其主要用途包括检测实体的进入和退出、覆盖物理参数以及检查区域重叠等
			常用于攻击范围检测、物品拾取区域等场景。
			
			- CollisionShape2D 节点
				CollisionShape2D节点用于表示2D空间中的碰撞形状数据 
				它需要与其他节点（如Area2D、PhysicsBody2D等）配合使用 
				为这些节点提供具体的碰撞形状 
				例如将CollisionShape2D作为Area2D的子节点
				可以为Area2D定义一个检测形状
				使其能够检测与该形状重叠的其他碰撞对象
				CollisionShape2D可以设置多种形状，如矩形、圆形、多边形等
			
			- Sprite2D 节点
				添加图片
	地图场景
		ColorRect 节点
			- 显示单色矩形的控件
		Line2D 节点
			- 显示一根线条
		get_overlapping_areas() 函数
			- 返回当前位置重叠在一起的所有区域节点
				for i in get_overlapping_areas():
					pass
		add_to_group() 函数
			- 将一个节点添加到指定的组中
		is_in_group() 函数
			- 检测一个节点是否属于某个指定的组 返回的是布尔型
		@export var y = 2 定义
			- 使用@export将定义改为开发工具可修改的值
		var player1:int = 0 定义
			- 新建一个脚本定义两名玩家的分数
		text=String.num_int64(记分版.player1)
			- 获取int类型分数并转换为String文本类型
		Input.get_action_strength("玩家2上移动")
			- 获取创建的输入映射