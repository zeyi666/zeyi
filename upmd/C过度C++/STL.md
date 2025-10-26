	a.size(); 计算长度
	vector
		矢量 向量 动态数组
		头文件
			- #include <vector>
		创建
			- vector <int> v; 创建向量v 
				- vector <float> v2(10,7); 
				- vector <float> v3(10); == vector <float> v3(10,0);
		处理
			- vector v.resize(10); 定义大小为10个元素
			- vector v.push_back(7); 末尾追加一个元素 值为7
		迭代器
			for(auto p=c.begin(); p!=c.end();p++)
				cout << *p << " ";
		
	set
		集合 会自动从小到大排列
		头文件
			- #include <set>
		创建
			- set <int> a;
		处理
			- 插入
				- a.insert(a);
			- 遍历
				- 迭代器
			- 查找
				- a.find(7);
				- a.find() 返回值是一个指针
			- 删除
				- a.erase(7);
	map
		键值对 会将所有键值对从小到大排列
		头文件
			- #includde <map>
		创建键值对
			map <string,int> m;
		处理
			- 添加
				- m["hello"] = 2;
			- 访问
				- cout << m["world"];
				- 如果存在"world",就返回值 否则返回0
			- 遍历
				- 迭代器
				- 获取值时类似结构体指针
			- 获取长度
				- m.size()
			- 输出
				- for (auto p=m.begin();p != m.end();p++)
					cout << p->frist << " : " << p->second
					p->frist 键
					p->second 值
	stack
		栈
		头文件
			- #include <stack>
		创建栈
			- stack <int> s;
		处理
			- 压栈
				- s.push(i);
			- 出栈
				- s.pop();
			- 访问栈顶
				- s.top();
			- 获取长度
				- s.size();
	queue
		队列
		头文件
			- #include <queue>
		创建队列
			- queue <int> s;
		处理
			- 入队
				- s.push(i);
			- 出队
				- s.pop();
			- 访问
				- 访问队首
					- s.front();
				- 访问队尾
					- s.back();
			- 获取长度
				- s.size();
	unordered_map && unordered_set
		不会排序的map和set
		头文件
			- #include <unordered_map>
			- #include <unordered_set>