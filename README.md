# Data-structure-memo

# 数据结构算法

## 红黑树

#### 一、红黑树性质（满足条件）<br>
1. 每个节点不是红色就是黑色 <br>
2. 根节点为黑色 <br>
3. 父子两节点不得同时为红 <br>
4. 任意节点至NULL（树尾端）的任何路径，所含之黑节点必须相同 <br>
5. 每个叶子结点都为黑（树尾端NIL指针或NULL结点）

#### 二、红黑树数据结构定义<br>
	 
	enum Color  
	{  
	      RED = 0,  
	      BLACK = 1  
	};  
	  
	struct RBTreeNode  
	{  
	       struct RBTreeNode*left, *right, *parent;  
	       int   key;  
	       int data;  
	       Color color;  
	};  

#### 三、左旋 <br>
<font face="menlo"> 1.出现红色右链接 2.两条连续的红链接 </font><br>
![Alt text](left.jpg)

#### 四、右旋
