![[4.png]]链表的图例实现
```
#include <iostream>

using std::cout;
using std::cin;

struct Node {
	int data;
	Node* link;
};

int main() {
	// C语言实现 
	Node* A;
	Node* temp = (Node *)malloc(sizeof(Node));
	(*temp).data = 17;
	temp->link = NULL;
	A = temp;
	cout << A->data << '\n';
	// C++实现
	Node *p;
	Node *t = new Node();
	t->data = 18;
	t->link = NULL;
	p = t;
	cout << p->data << '\n';
} 
```
![[5.png]]
注意点
	- new Node() 加括号是为了调用默认狗在函数初始化对象
	- 链表节点必须在堆区 （malloc / new 开辟）创建, 因为堆区内存的生命周期可由程序员控制，能满足链表节点”长期存在“的需求, 而栈区和代码区无法满足这一要求