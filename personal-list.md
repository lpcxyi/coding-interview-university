## 目录

### 学习的主题

- [算法复杂度 / Big-O / 渐进分析法](#算法复杂度--big-o--渐进分析法)
- [数据结构](#数据结构)
    - [数组（Arrays）](#数组arrays)
    - [链表（Linked Lists）](#链表linked-lists)
    - [堆栈（Stack）](#堆栈stack)
    - [队列（Queue）](#队列queue)
    - [哈希表（Hash table）](#哈希表hash-table)
- [更多的知识](#更多的知识)
    - [二分查找（Binary search）](#二分查找binary-search)
    - [按位运算（Bitwise operations）](#按位运算bitwise-operations)
- [树（Trees）](#树trees)
    - [树-介绍](#树-介绍)
    - [二叉查找树（Binary search trees）：BSTs](#二叉查找树binary-search-treesbsts)
    - [堆（Heap） / 优先级队列（Priority Queue） / 二叉堆（Binary Heap）](#堆heap--优先级队列priority-queue--二叉堆binary-heap)
    - 平衡搜索树 (总体概念，不涉及细节)
    - 遍历：前序、中序、后序、BFS、DFS
- [排序](#排序sorting)
    - 选择排序（selection）
    - 插入排序（insertion）
    - 堆排序（heapsort）
    - 快速排序（quicksort）
    - 归并排序（merge sort）
- [图（Graphs）](#图graphs)
    - 有向图（directed）
    - 无向图（undirected）
    - 邻接矩阵（adjacency matrix）
    - 邻接表（adjacency list）
    - 遍历：广度优先(BFS), 深度优先(DFS)
- [更多知识](#更多知识)
    - [递归](#递归recursion)
    - [动态规划](#动态规划dynamic-programming)
    - [设计模式](#设计模式)
    - [组合 & 概率](#组合combinatorics-n-中选-k-个--概率probability)
    - [NP, NP-完全和近似算法](#np-np-完全和近似算法)
    - [缓存](#缓存cache)
    - [进程和线程](#进程processe和线程thread)
    - [测试](#测试)
    - [调度](#调度)
    - [字符串搜索和操作](#字符串搜索和操作)
    - [字典树（Tries）](#字典树tries)
    - [浮点数](#浮点数)
    - [Unicode](#unicode)
    - [字节顺序](#字节序Endianness)
    - [网络](#网络视频)

### 可选的额外主题和资源

- [系统设计、可扩展性和数据处理](#系统设计、可扩展性和数据处理)
- [附加学习](#附加学习)
    - [编译器](#编译器)
    - [Emacs and vi(m)](#emacs-and-vim)
    - [Unix 命令行工具](#unix-命令行工具)
    - [信息论](#信息论-视频)
    - [奇偶校验位 & 汉明码 (视频)](#奇偶校验位--汉明码-视频)
    - [系统熵值](#系统熵值Entropy)
    - [密码学](#密码学)
    - [压缩](#压缩)
    - [计算机安全](#计算机安全)
    - [垃圾回收](#垃圾回收)
    - [并行编程](#并行编程)
    - [消息传递，序列化和队列化的系统](#消息传递序列化和队列系统)
    - [A*搜索算法](#a*搜索算法)
    - [快速傅里叶变换](#快速傅里叶变换)
    - [布隆过滤器](#布隆过滤器)
    - [HyperLogLog](#hyperloglog)
    - [局部敏感哈希](#局部敏感哈希)
    - [van Emde Boas 树](#van-emde-boas-树)
    - [增强数据结构](#增强数据结构)
    - [平衡查找树](#平衡查找树balanced-search-trees)
        - AVL 树
        - 伸缩树（Splay tree）
        - 红黑树
        - 2-3 查找树
        - 2-3-4 树(也称 2-4 树)
        - N-ary (K-ary, M-ary)树
        - B 树
    - [k-D 树](#k-d树)
    - [跳表](#跳表)
    - [网络流](#网络流)
    - [不相交集 & 联合查找](#不相交集--联合查找)
    - [快速处理的数学](#快速处理的数学)
    - [树堆 (Treap)](#树堆-treap)
    - [线性规划](#线性规划linear-programming视频)
    - [几何：凸包（Geometry, Convex hull）](#几何凸包geometry-convex-hull视频)
    - [离散数学](#离散数学)
- [论文](#论文)

---

### 如果你不介意 Git

创建一个新的分支，这样你就可以检查类似这样的项目了，只需在方括号中放入一个x：[x]

1. 在 GitHub 上 Fork 该仓库： 点击 Fork 按钮，将 `https://github.com/jwasham/coding-interview-university` 仓库复制到你的 GitHub 账号中。

2. 克隆项目到本地：

    ```
    git clone git@github.com:<your_github_username>/coding-interview-university.git
    cd coding-interview-university
    git remote add upstream https://github.com/jwasham/coding-interview-university
    git remote set-url --push upstream DISABLE  # 这样你就不会将个人进展推回到原始仓库了。
    ```

3. 在你完成了一些修改后，在框框中打 x：

    ```
    git commit -am "Marked personal progress"
    git pull upstream main  # 将您的分支与原始仓库中的更改保持最新
      
    git push # just pushes to your fork
    ```

## 没有包含的内容

有一些熟悉且普遍的技术在此未被谈及到：

- [] Javascript
- [] HTML，CSS和其他前端技术
- [] SQL

## 算法复杂度 / Big-O / 渐进分析法

- [x] [哈佛大学CS50 - 渐进符号（视频）](https://www.youtube.com/watch?v=iOq5kSKqeR4)
- [x] [大O符号（通用快速教程）（视频）](https://www.youtube.com/watch?v=V6mKVRU1evU)
- [x] [大O符号（以及Ω和Θ）- 最佳数学解释（视频）](https://www.youtube.com/watch?v=ei-A_wy5Yxw&index=2&list=PL1BaGV1cIH4UhkL8a9bJGG356covJ76qN)
- [x] [Skiena（视频）](https://www.youtube.com/watch?v=z1mkCe3kVUA)
- [x] [加州大学伯克利分校关于大O符号（视频）](https://archive.org/details/ucberkeley_webcast_VIS4YDpuP98)
- [x] [摊还分析（视频）](https://www.youtube.com/watch?v=B3SpQZaAZP4&index=10&list=PL1BaGV1cIH4UhkL8a9bJGG356covJ76qN)
- [x] TopCoder（包括递归关系和主定理）：
    - [计算复杂性：第1部分](https://www.topcoder.com/thrive/articles/Computational%20Complexity%20part%20one)
    - [计算复杂性：第2部分](https://www.topcoder.com/thrive/articles/Computational%20Complexity%20part%20two)
- [x] [速查表](http://bigocheatsheet.com/)
- [x] [[Review] Analyzing Algorithms (playlist) in 18 minutes (video)](https://www.youtube.com/playlist?list=PL9xmBV_5YoZMxejjIyFHWa-4nKg6sdoIv)

## 数据结构

- ### 数组（Arrays）
    - [x] 介绍：
        - [数组 CS50 哈佛大学](https://www.youtube.com/watch?v=tI_tIZFyKBw&t=3009s)
        - [数组（视频）](https://www.coursera.org/lecture/data-structures/arrays-OsBSF)
        - [加州大学伯克利分校CS61B - 线性和多维数组（视频）](https://archive.org/details/ucberkeley_webcast_Wp8oiO_CZZE)（从15分32秒开始）
        - [动态数组（视频）](https://www.coursera.org/lecture/data-structures/dynamic-arrays-EwbnV)
        - [嵌套数组（视频）](https://www.youtube.com/watch?v=1jtrQqYpt7g)
    - [x] 实现一个动态数组（可自动调整大小的可变数组）：
        - [x] 练习使用数组和指针去编码，并且指针是通过计算去跳转而不是使用索引
        - [x] 通过分配内存来新建一个原生数据型数组
            - 可以使用 int 类型的数组，但不能使用其语法特性
            - 从大小为16或更大的数（使用2的倍数 —— 16、32、64、128）开始编写
        - [x] size() —— 数组元素的个数
        - [x] capacity() —— 可容纳元素的个数
        - [x] is_empty()
        - [x] at(index) —— 返回对应索引的元素，且若索引越界则愤然报错
        - [x] push(item)
        - [x] insert(index, item) —— 在指定索引中插入元素，并把后面的元素依次后移
        - [x] prepend(item) —— 可以使用上面的 insert 函数，传参 index 为 0
        - [x] pop() —— 删除在数组末端的元素，并返回其值
        - [x] delete(index) —— 删除指定索引的元素，并把后面的元素依次前移
        - [x] remove(item) —— 删除指定值的元素，并返回其索引（即使有多个元素）
        - [x] find(item) —— 寻找指定值的元素并返回其中第一个出现的元素其索引，若未找到则返回 -1
        - [x] resize(new_capacity) // 私有函数
            - 若数组的大小到达其容积，则变大一倍
            - 获取元素后，若数组大小为其容积的1/4，则缩小一半
    - [x] 时间复杂度
        - 在数组末端增加/删除、定位、更新元素，只允许占 O(1) 的时间复杂度（平摊（amortized）去分配内存以获取更多空间）
        - 在数组任何地方插入/移除元素，只允许 O(n) 的时间复杂度
    - [x] 空间复杂度
        - 因为在内存中分配的空间邻近，所以有助于提高性能
        - 空间需求 = （大于或等于 n 的数组容积）* 元素的大小。即便空间需求为 2n，其空间复杂度仍然是 O(n)

- ### 链表（Linked Lists）
    - [x] 介绍：
        - [x] [链表 CS50 哈佛大学](https://www.youtube.com/watch?v=2T-A_GFuoTo&t=650s) - 这样建立了直观感。
        - [x] [单链表（视频）](https://www.coursera.org/lecture/data-structures/singly-linked-lists-kHhgK)
        - [x] [CS 61B - 链表1（视频）](https://archive.org/details/ucberkeley_webcast_htzJdKoEmO0)
        - [x] [CS 61B - 链表 2（视频）](https://archive.org/details/ucberkeley_webcast_-c4I3gFYe3w)
        - [x] [[复习] 4分钟了解链表（视频）](https://youtu.be/F8AbOfQwl1c)
    - [x] [C代码（视频）](https://www.youtube.com/watch?v=QN6FPiD0Gzo)
            - 不是整个视频，只是关于Node结构和内存分配的部分。
    - [x] 链表 vs 数组：
        - [核心链表与数组（视频）](https://www.coursera.org/lecture/data-structures-optimizing-performance/core-linked-lists-vs-arrays-rjBs9)
        - [在现实世界中，链表与数组的比较（视频）](https://www.coursera.org/lecture/data-structures-optimizing-performance/in-the-real-world-lists-vs-arrays-QUaUd)
    - [x] [为什么你需要避免使用链表（视频）](https://www.youtube.com/watch?v=YQs6IC-vgmo)
    - [x] 的确：你需要关于“指向指针的指针”的相关知识：（因为当你传递一个指针到一个函数时，
      该函数可能会改变指针所指向的地址）该页只是为了让你了解“指向指针的指针”这一概念。
      但我并不推荐这种链式遍历的风格。因为，这种风格的代码，其可读性和可维护性太低。
        - [指向指针的指针](https://www.eskimo.com/~scs/cclass/int/sx8.html)
    - [x] 实现（我实现了使用尾指针以及没有使用尾指针这两种情况）：
        - [x] size() —— 返回链表中数据元素的个数
        - [x] empty() —— 若链表为空则返回一个布尔值 true
        - [x] value_at(index) —— 返回第 n 个元素的值（从0开始计算）
        - [x] push_front(value) —— 添加元素到链表的首部
        - [x] pop_front() —— 删除首部元素并返回其值
        - [x] push_back(value) —— 添加元素到链表的尾部
        - [x] pop_back() —— 删除尾部元素并返回其值
        - [x] front() —— 返回首部元素的值
        - [x] back() —— 返回尾部元素的值
        - [x] insert(index, value) —— 插入值到指定的索引，并把当前索引的元素指向到新的元素
        - [x] erase(index) —— 删除指定索引的节点
        - [x] value_n_from_end(n) —— 返回倒数第 n 个节点的值
        - [x] reverse() —— 逆序链表
        - [x] remove_value(value) —— 删除链表中指定值的第一个元素
    - [ ] 双向链表
        - [介绍（视频）](https://www.coursera.org/learn/data-structures/lecture/jpGKD/doubly-linked-lists)
        - 并不需要实现

- ### 堆栈（Stack）
    - [x] [堆栈（视频）](https://www.coursera.org/learn/data-structures/lecture/UdKzQ/stacks)
    - [x] [[Review] Stacks in 3 minutes (video)](https://youtu.be/KcT3aVgrrpU)
    - [x] 可以不实现，因为使用数组来实现是微不足道的事

- ### 队列（Queue）
    - [x] [队列（视频）](https://www.coursera.org/learn/data-structures/lecture/EShpq/queue)
    - [x] [原型队列/先进先出（FIFO）](https://en.wikipedia.org/wiki/Circular_buffer)
    - [x] [[Review] Queues in 3 minutes (video)](https://youtu.be/D6gu-_tmEpQ)
    - [ ] 使用含有尾部指针的链表来实现:
        - enqueue(value) —— 在尾部添加值
        - dequeue() —— 删除最早添加的元素并返回其值（首部元素）
        - empty()
    - [ ] 使用固定大小的数组实现：
        - enqueue(value) —— 在可容的情况下添加元素到尾部
        - dequeue() —— 删除最早添加的元素并返回其值
        - empty()
        - full()
    - [x] 花销：
        - 在糟糕的实现情况下，使用链表所实现的队列，其入列和出列的时间复杂度将会是 O(n)。
        因为，你需要找到下一个元素，以致循环整个队列
        - enqueue：O(1)（平摊（amortized）、链表和数组 [探测（probing）]）
        - dequeue：O(1)（链表和数组）
        - empty：O(1)（链表和数组）

- ### 哈希表（Hash table）
    - [x] 视频：
        - [x] [链式哈希表（视频）](https://www.youtube.com/watch?v=0M_kIqhwbFo&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb&index=8)
        - [x] [Table Doubling 和 Karp-Rabin（视频）](https://www.youtube.com/watch?v=BRO7mVIFt08&index=9&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb)
        - [ ] [Open Addressing 和密码型哈希（Cryptographic Hashing）（视频）](https://www.youtube.com/watch?v=rvdJDijO2Ro&index=10&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb)
        - [ ] [PyCon 2010：强大的字典（视频）](https://www.youtube.com/watch?v=C4Kc8xzcA68)
        - [ ] [PyCon 2017：字典更强大（视频）](https://www.youtube.com/watch?v=66P5FMkWoVU)
        - [ ] [(高级) 随机化：通用和完美哈希（视频）](https://www.youtube.com/watch?v=z0lJ2k0sl1g&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp&index=11)
        - [ ] [(进阶)完美哈希（Perfect hashing）（视频）](https://www.youtube.com/watch?v=N0COwN14gt0&list=PL2B4EEwhKD-NbwZ4ezj7gyc_3yNrojKM9&index=4)

    - [x] 在线课程：
        - [x] [核心哈希表（视频）](https://www.coursera.org/lecture/data-structures-optimizing-performance/core-hash-tables-m7UuP)
        - [x] [数据结构（视频）](https://www.coursera.org/learn/data-structures/home/week/4)
        - [ ] [电话簿问题（视频）](https://www.coursera.org/lecture/data-structures/phone-book-problem-NYZZP)
        - [ ] 分布式哈希表：
            - [Dropbox中的即时上传和存储优化（视频）](https://www.coursera.org/lecture/data-structures/instant-uploads-and-storage-optimization-in-dropbox-DvaIb)
            - [分布式哈希表（视频）](https://www.coursera.org/lecture/data-structures/distributed-hash-tables-tvH8H)

    - [x] 使用线性探测法的数组实现
        - hash(k, m) - m是哈希表的大小
        - add(key, value) - 如果键已存在，则更新值
        - exists(key) - 检查键是否存在
        - get(key) - 获取给定键的值
        - remove(key) - 删除给定键的值

## 更多的知识

- ### 二分查找（Binary search）
    - [ ] [二分查找（视频）](https://www.youtube.com/watch?v=D5SrAga1pno)
    - [ ] [二分查找（视频）](https://www.khanacademy.org/computing/computer-science/algorithms/binary-search/a/binary-search)
    - [ ] [详情](https://www.topcoder.com/community/data-science/data-science-tutorials/binary-search/)
    - [ ] [蓝图](https://leetcode.com/discuss/general-discussion/786126/python-powerful-ultimate-binary-search-template-solved-many-problems)   
    - [ ] 实现：
        - 二分查找（在一个已排序好的整型数组中查找）
        - 迭代式二分查找

- ### 按位运算（Bitwise operations）
    - [x] [Bits 速查表](https://github.com/jwasham/coding-interview-university/blob/main/extras/cheat%20sheets/bits-cheat-sheet.pdf) ── 你需要知道大量2的幂数值（从2^1 到 2^16 及 2^32）
    - [ ] 好好理解位操作符的含义：&、|、^、~、>>、<<
        - [x] [字码（words）](https://en.wikipedia.org/wiki/Word_(computer_architecture))
        - [x] 好的介绍：
            [位操作（视频）](https://www.youtube.com/watch?v=7jkIUgLC29I)
        - [x] [C 语言编程教程 2-10：按位运算（视频）](https://www.youtube.com/watch?v=d0AwjSpNXR0)
        - [x] [位操作](https://en.wikipedia.org/wiki/Bit_manipulation)
        - [x] [按位运算](https://en.wikipedia.org/wiki/Bitwise_operation)
        - [ ] [Bithacks](https://graphics.stanford.edu/~seander/bithacks.html)
        - [ ] [位元抚弄者（The Bit Twiddler）](http://bits.stephan-brumme.com/)
        - [ ] [交互式位元抚弄者（The Bit Twiddler Interactive）](http://bits.stephan-brumme.com/interactive.html)
        - [ ] [位操作技巧（Bit Hacks）（视频）](https://www.youtube.com/watch?v=ZusiKXcz_ac)
        - [ ] [练习位操作](https://pconrad.github.io/old_pconrad_cs16/topics/bitOps/)
    - [ ] 一补数和补码
        - [二进制：利 & 弊（为什么我们要使用补码）（视频）](https://www.youtube.com/watch?v=lKTsv6iVxV4)
        - [一补数（1s Complement）](https://en.wikipedia.org/wiki/Ones%27_complement)
        - [补码（2s Complement）](https://en.wikipedia.org/wiki/Two%27s_complement)
    - [ ] 计算置位（Set Bits）
        - [计算一个字节中置位（Set Bits）的四种方式（视频）](https://youtu.be/Hzuzo9NJrlc)
        - [计算比特位](https://graphics.stanford.edu/~seander/bithacks.html#CountBitsSetKernighan)
        - [如何在一个 32 位的整型中计算置位（Set Bits）的数量](http://stackoverflow.com/questions/109023/how-to-count-the-number-of-set-bits-in-a-32-bit-integer)
    - [ ] 交换值：
        - [交换（Swap）](http://bits.stephan-brumme.com/swap.html)
    - [x] 绝对值：
        - [绝对整型（Absolute Integer）](http://bits.stephan-brumme.com/absInteger.html)

## 树（Trees）

- ### 树-介绍
    - [x] [树的介绍（视频）](https://www.coursera.org/learn/data-structures/lecture/95qda/trees)
    - [x] [树遍历（视频）](https://www.coursera.org/lecture/data-structures/tree-traversal-fr51b)
    - [ ] [BFS（广度优先搜索）和DFS（深度优先搜索）（视频）](https://www.youtube.com/watch?v=uWL6FJhq5fM)
        - BFS 笔记
            - 层次遍历（BFS，使用队列）
            - 时间复杂度： O(n)
            - 空间复杂度：最佳情况：O(1)，最坏情况：O(n/2)=O(n)
        - DFS 笔记：
            - 时间复杂度：O(n)
            - 空间复杂度：
                - 最好情况：O(log n) - 树的平均高度
                - 最坏情况：O(n)
            - 中序遍历（DFS：左、节点本身、右）
            - 后序遍历（DFS：左、右、节点本身）
            - 先序遍历（DFS：节点本身、左、右）

- ### 二叉查找树（Binary search trees）：BSTs
    - [x] [二叉搜索树复习（视频）](https://www.youtube.com/watch?v=x6At0nzX92o&index=1&list=PLA5Lqm4uh9Bbq-E0ZnqTIa8LRaL77ica6)
    - C/C++:
        - [ ] [二叉查找树 —— 在 C/C++ 中实现（视频）](https://www.youtube.com/watch?v=COZK7NATh4k&list=PL2_aWCzGMAwI3W_JlcBbtYTwiQSsOTa6P&index=28)
        - [ ] [BST 的实现 —— 在堆栈和堆中的内存分配（视频）](https://www.youtube.com/watch?v=hWokyBoo0aI&list=PL2_aWCzGMAwI3W_JlcBbtYTwiQSsOTa6P&index=29)
        - [ ] [在二叉查找树中找到最小和最大的元素（视频）](https://www.youtube.com/watch?v=Ut90klNN264&index=30&list=PL2_aWCzGMAwI3W_JlcBbtYTwiQSsOTa6P)
        - [ ] [寻找二叉树的高度（视频）](https://www.youtube.com/watch?v=_pnqMz5nrRs&list=PL2_aWCzGMAwI3W_JlcBbtYTwiQSsOTa6P&index=31)
        - [ ] [二叉树的遍历 —— 广度优先和深度优先策略（视频）](https://www.youtube.com/watch?v=9RHO6jU--GU&list=PL2_aWCzGMAwI3W_JlcBbtYTwiQSsOTa6P&index=32)
        - [ ] [二叉树：层序遍历（视频）](https://www.youtube.com/watch?v=86g8jAQug04&index=33&list=PL2_aWCzGMAwI3W_JlcBbtYTwiQSsOTa6P)
        - [ ] [二叉树的遍历：先序、中序、后序（视频）](https://www.youtube.com/watch?v=gm8DUJJhmY4&index=34&list=PL2_aWCzGMAwI3W_JlcBbtYTwiQSsOTa6P)
        - [ ] [判断一棵二叉树是否为二叉查找树（视频）](https://www.youtube.com/watch?v=yEwSGhSsT0U&index=35&list=PL2_aWCzGMAwI3W_JlcBbtYTwiQSsOTa6P)
        - [ ] [从二叉查找树中删除一个节点（视频）](https://www.youtube.com/watch?v=gcULXE7ViZw&list=PL2_aWCzGMAwI3W_JlcBbtYTwiQSsOTa6P&index=36)
        - [ ] [二叉查找树中序遍历的后继者（视频）](https://www.youtube.com/watch?v=5cPbNCrdotA&index=37&list=PL2_aWCzGMAwI3W_JlcBbtYTwiQSsOTa6P)
    - [ ] 实现：
        - [ ] [insert    // 将值插入树中](https://leetcode.com/problems/insert-into-a-binary-search-tree/submissions/987660183/)
        - [ ] get_node_count // 查找树上的节点数
        - [ ] print_values // 从小到大打印树中节点的值
        - [ ] delete_tree
        - [ ] is_in_tree // 如果值存在于树中则返回 true
        - [ ] [get_height // 以节点为单位返回高度（单个节点的高度为1）](https://www.geeksforgeeks.org/find-the-maximum-depth-or-height-of-a-tree/)
        - [ ] get_min   // 返回树上的最小值
        - [ ] get_max   // 返回树上的最大值
        - [ ] is_binary_search_tree
        - [ ] delete_value
        - [ ] get_successor // 返回给定值的后继者，若没有则返回-1

- ### 堆（Heap） / 优先级队列（Priority Queue） / 二叉堆（Binary Heap）
    - 以树形结构可视化，但通常在存储上是线性的（数组、链表）
    - [ ] [堆（Heap）](https://en.wikipedia.org/wiki/Heap_(data_structure))
    - [ ] [堆简介（视频）](https://www.coursera.org/lecture/data-structures/introduction-2OpTs)
    - [ ] [二叉树（视频）](https://www.coursera.org/learn/data-structures/lecture/GRV2q/binary-trees)
    - [ ] [树高度备注（视频）](https://www.coursera.org/learn/data-structures/supplement/S5xxz/tree-height-remark)
    - [ ] [基本操作（视频）](https://www.coursera.org/learn/data-structures/lecture/0g1dl/basic-operations)
    - [ ] [完全二叉树（视频）](https://www.coursera.org/learn/data-structures/lecture/gl5Ni/complete-binary-trees)
    - [ ] [伪代码（视频）](https://www.coursera.org/learn/data-structures/lecture/HxQo9/pseudocode)
    - [ ] [堆排序 - 跳转到开始部分（视频）](https://youtu.be/odNJmw5TOEE?list=PLFDnELG9dpVxQCxuD-9BSy2E7BWY3t5Sm&t=3291)
    - [ ] [堆排序（视频）](https://www.coursera.org/lecture/data-structures/heap-sort-hSzMO)
    - [ ] [构建堆（视频）](https://www.coursera.org/lecture/data-structures/building-a-heap-dwrOS)
    - [ ] [MIT：堆和堆排序（视频）](https://www.youtube.com/watch?v=B7hVxCmfPtM&index=4&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb)
    - [ ] [CS 61B Lecture 24：优先队列（视频）](https://archive.org/details/ucberkeley_webcast_yIUFT6AKBGE)
    - [ ] [线性时间构建堆（大顶堆）](https://www.youtube.com/watch?v=MiyLo8adrWw)
    - [ ] 实现一个大顶堆：
        - [ ] insert
        - [ ] sift_up —— 用于插入元素
        - [ ] get_max —— 返回最大值但不移除元素
        - [ ] get_size() —— 返回存储的元素数量
        - [ ] is_empty() —— 若堆为空则返回 true
        - [ ] extract_max —— 返回最大值并移除
        - [ ] sift_down —— 用于获取最大值元素
        - [ ] remove(i) —— 删除指定索引的元素
        - [ ] heapify —— 构建堆，用于堆排序
        - [ ] heap_sort() —— 拿到一个未排序的数组，然后使用大顶堆或者小顶堆进行就地排序

## 排序（Sorting）

- [ ] 笔记:
    - 实现各种排序，知道每种排序的最坏、最好和平均的复杂度分别是什么场景:
        - 不要用冒泡排序 - 效率太差 - 时间复杂度 O(n^2), 除非 n <= 16
    - [ ] 排序算法的稳定性 ("快排是稳定的么?")
        - [排序算法的稳定性](https://en.wikipedia.org/wiki/Sorting_algorithm#Stability)
        - [排序算法的稳定性](http://stackoverflow.com/questions/1517793/stability-in-sorting-algorithms)
        - [排序算法的稳定性](http://www.geeksforgeeks.org/stability-in-sorting-algorithms/)
        - [排序算法 - 稳定性](http://homepages.math.uic.edu/~leon/cs-mcs401-s08/handouts/stability.pdf)
    - [ ] 哪种排序算法可以用链表？哪种用数组？哪种两者都可？
        - 并不推荐对一个链表排序，但归并排序是可行的.
        - [链表的归并排序](http://www.geeksforgeeks.org/merge-sort-for-linked-list/)

- 关于堆排序，请查看前文堆的数据结构部分。堆排序很强大，不过是非稳定排序。

- [ ] [Sedgewick ── 归并排序（5个视频）](https://www.coursera.org/learn/algorithms-part1/home/week/3)
    - [ ] [1. 归并排序（Mergesort）](https://www.coursera.org/lecture/algorithms-part1/mergesort-ARWDq)
    - [ ] [2. 自底向上的归并排序（Bottom up Mergesort）](https://www.coursera.org/learn/algorithms-part1/lecture/PWNEl/bottom-up-mergesort)
    - [ ] [3. 排序复杂性（Sorting Complexity）](https://www.coursera.org/lecture/algorithms-part1/sorting-complexity-xAltF)
    - [ ] [4. 比较器（Comparators）](https://www.coursera.org/lecture/algorithms-part1/comparators-9FYhS)
    - [ ] [5. 稳定性（Stability）](https://www.coursera.org/learn/algorithms-part1/lecture/pvvLZ/stability)

- [ ] [Sedgewick ── 快速排序（4个视频）](https://www.coursera.org/learn/algorithms-part1/home/week/3)
    - [ ] [1. 快速排序（Quicksort）](https://www.coursera.org/lecture/algorithms-part1/quicksort-vjvnC)
    - [ ] [2. 选择排序（Selection）](https://www.coursera.org/lecture/algorithms-part1/selection-UQxFT)
    - [ ] [3. 重复键（Duplicate Keys）](https://www.coursera.org/lecture/algorithms-part1/duplicate-keys-XvjPd)
    - [ ] [4. 系统排序（System Sorts）](https://www.coursera.org/lecture/algorithms-part1/system-sorts-QBNZ7)

- [ ] [冒泡排序（视频）](https://www.youtube.com/watch?v=P00xJgWzz2c&index=1&list=PL89B61F78B552C1AB)
- [ ] [冒泡排序分析（视频）](https://www.youtube.com/watch?v=ni_zk257Nqo&index=7&list=PL89B61F78B552C1AB)
- [ ] [插入排序 & 归并排序（视频）](https://www.youtube.com/watch?v=Kg4bqzAqRBM&index=3&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb)
- [ ] [插入排序（视频）](https://www.youtube.com/watch?v=c4BRHC7kTaQ&index=2&list=PL89B61F78B552C1AB)
- [ ] [归并排序（视频）](https://www.youtube.com/watch?v=GCae1WNvnZM&index=3&list=PL89B61F78B552C1AB)
- [ ] [快排（视频）](https://www.youtube.com/watch?v=y_G9BkAm6B8&index=4&list=PL89B61F78B552C1AB)
- [ ] [选择排序（视频）](https://www.youtube.com/watch?v=6nDMgr0-Yyo&index=8&list=PL89B61F78B552C1AB)

- [ ] 归并排序代码：
    - [ ] [使用外部数组（C语言）](http://www.cs.yale.edu/homes/aspnes/classes/223/examples/sorting/mergesort.c)
    - [ ] [使用外部数组（Python语言）](https://github.com/jwasham/practice-python/blob/master/merge_sort/merge_sort.py)
    - [ ] [对原数组直接排序（C++）](https://github.com/jwasham/practice-cpp/blob/master/merge_sort/merge_sort.cc)
- [ ] 快速排序代码：
    - [ ] [实现（C语言）](http://www.cs.yale.edu/homes/aspnes/classes/223/examples/randomization/quick.c)
    - [ ] [实现（C语言）](https://github.com/jwasham/practice-c/blob/master/quick_sort/quick_sort.c)
    - [ ] [实现（Python语言）](https://github.com/jwasham/practice-python/blob/master/quick_sort/quick_sort.py)

- [ ] 实现:
    - [ ] 归并：平均和最差情况的时间复杂度为 O(n log n)。
    - [ ] 快排：平均时间复杂度为 O(n log n)。
    - 选择排序和插入排序的最坏、平均时间复杂度都是 O(n^2)。
    - 关于堆排序，请查看前文堆的数据结构部分。

- [ ] 有兴趣的话，还有一些补充，但并不是必须的:
    - [Sedgewick──基数排序 (6个视频)](https://www.coursera.org/learn/algorithms-part2/home/week/3)
        - [ ] [1. Java 中的字符串](https://www.coursera.org/learn/algorithms-part2/lecture/vGHvb/strings-in-java)
        - [ ] [2. 键值索引计数（Key Indexed Counting）](https://www.coursera.org/learn/algorithms-part2/lecture/2pi1Z/key-indexed-counting)
        - [ ] [3. Least Significant Digit First String Radix Sort](https://www.coursera.org/learn/algorithms-part2/lecture/c1U7L/lsd-radix-sort)
        - [ ] [4. Most Significant Digit First String Radix Sort](https://www.coursera.org/learn/algorithms-part2/lecture/gFxwG/msd-radix-sort)
        - [ ] [5. 3中基数快速排序](https://www.coursera.org/learn/algorithms-part2/lecture/crkd5/3-way-radix-quicksort)
        - [ ] [6. 后继数组（Suffix Arrays）](https://www.coursera.org/learn/algorithms-part2/lecture/TH18W/suffix-arrays)
    - [ ] [基数排序](http://www.cs.yale.edu/homes/aspnes/classes/223/notes.html#radixSort)
    - [ ] [基数排序（视频）](https://www.youtube.com/watch?v=xhr26ia4k38)
    - [ ] [基数排序, 计数排序 (线性时间内)（视频）](https://www.youtube.com/watch?v=Nz1KZXbghj8&index=7&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb)
    - [ ] [随机算法: 矩阵相乘, 快排, Freivalds' 算法（视频）](https://www.youtube.com/watch?v=cNB2lADK3_s&index=8&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp)
    - [ ] [线性时间内的排序（视频）](https://www.youtube.com/watch?v=pOKy3RZbSws&list=PLUl4u3cNGP61hsJNdULdudlRL493b-XZf&index=14)

总结一下，这是[15种排序算法](https://www.youtube.com/watch?v=kPRA0W1kECg)的可视化表示。
如果你需要有关此主题的更多详细信息，请参阅“[一些主题的额外内容](#一些主题的额外内容)”中的“排序”部分。

## 图（Graphs）

- [ ] 图 (复习和其他):

    - [ ] [6.006 单源最短路径问题（视频）](https://www.youtube.com/watch?v=Aa2sqUhIn-E&index=15&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb)
    - [ ] [6.006 Dijkstra算法（视频）](https://www.youtube.com/watch?v=NSHizBK9JD8&t=1731s&ab_channel=MITOpenCourseWare)
    - [ ] [6.006 Bellman-Ford算法（视频）](https://www.youtube.com/watch?v=f9cVS_URPc0&ab_channel=MITOpenCourseWare)
    - [ ] [6.006 加速Dijkstra算法（视频）](https://www.youtube.com/watch?v=CHvQ3q_gJ7E&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb&index=18)
    - [ ] [Aduni：图算法 I - 拓扑排序，最小生成树，Prim算法 - 讲座6（视频）](https://www.youtube.com/watch?v=i_AQT_XfvD8&index=6&list=PLFDnELG9dpVxQCxuD-9BSy2E7BWY3t5Sm)
    - [ ] [Aduni：图算法 II - DFS，BFS，Kruskal算法，Union Find数据结构 - 讲座7（视频）](https://www.youtube.com/watch?v=ufj5_bppBsA&list=PLFDnELG9dpVxQCxuD-9BSy2E7BWY3t5Sm&index=7)
    - [ ] [Aduni：图算法 III：最短路径 - 讲座8（视频）](https://www.youtube.com/watch?v=DiedsPsMKXc&list=PLFDnELG9dpVxQCxuD-9BSy2E7BWY3t5Sm&index=8)
    - [ ] [Aduni：图算法 IV：几何算法入门 - 讲座9（视频）](https://www.youtube.com/watch?v=XIAQRlNkJAw&list=PLFDnELG9dpVxQCxuD-9BSy2E7BWY3t5Sm&index=9)
    - [ ] [CS 61B 2014：加权图（视频）](https://archive.org/details/ucberkeley_webcast_zFbq8vOZ_0k)
    - [ ] [贪婪算法：最小生成树（视频）](https://www.youtube.com/watch?v=tKwnms5iRBU&index=16&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp)
    - [ ] [强连通分量Kosaraju算法图算法（视频）](https://www.youtube.com/watch?v=RpgcYiky7uw)

- 我会实现:
    - [ ] DFS 邻接表 (递归)
    - [ ] DFS 邻接表 (栈迭代)
    - [ ] DFS 邻接矩阵 (递归)
    - [ ] DFS 邻接矩阵 (栈迭代)
    - [ ] BFS 邻接表
    - [ ] BFS 邻接矩阵
    - [ ] 单源最短路径问题 (Dijkstra)
    - [ ] 最小生成树
    - 基于 DFS 的算法 (根据上文 Aduni 的视频):
        - [ ] 检查环 (我们会先检查是否有环存在以便做拓扑排序)
        - [ ] 拓扑排序
        - [ ] 计算图中的连通分支
        - [ ] 列出强连通分量
        - [ ] 检查双向图

## 更多知识

- ### 递归（Recursion）
    - [ ] Stanford 大学关于递归 & 回溯的课程:
        - [ ] [课程 8 | 抽象编程（视频）](https://www.youtube.com/watch?v=gl3emqCuueQ&list=PLFE6E58F856038C69&index=8)
        - [ ] [课程 9 | 抽象编程（视频）](https://www.youtube.com/watch?v=uFJhEPrbycQ&list=PLFE6E58F856038C69&index=9)
        - [ ] [课程 10 | 抽象编程（视频）](https://www.youtube.com/watch?v=NdF1QDTRkck&index=10&list=PLFE6E58F856038C69)
        - [ ] [课程 11 | 抽象编程（视频）](https://www.youtube.com/watch?v=p-gpaIGRCQI&list=PLFE6E58F856038C69&index=11)
    - 什么时候适合使用
    - 尾递归会更好么?
        - [ ] [什么是尾递归以及为什么它如此糟糕?](https://www.quora.com/What-is-tail-recursion-Why-is-it-so-bad)
        - [ ] [尾递归（视频）](https://www.coursera.org/lecture/programming-languages/tail-recursion-YZic1)
    - [ ] [解决任何递归问题的5个简单步骤（视频）](https://youtu.be/ngCos392W4w)

    回溯蓝图: [Java](https://leetcode.com/problems/combination-sum/discuss/16502/A-general-approach-to-backtracking-questions-in-Java-(Subsets-Permutations-Combination-Sum-Palindrome-Partitioning))
	[Python](https://leetcode.com/problems/combination-sum/discuss/429538/General-Backtracking-questions-solutions-in-Python-for-reference-%3A)

- ### 动态规划（Dynamic Programming）
    - [ ] 视频:
        - [ ] 单独的动态规划问题列表（每个都很短）:
            [动态规划（视频）](https://www.youtube.com/playlist?list=PLrmLmBdmIlpsHaNTPP_jHHDx_os9ItYXr)
    - [ ] 耶鲁课程笔记:
        - [ ] [动态规划](http://www.cs.yale.edu/homes/aspnes/classes/223/notes.html#dynamicProgramming)
    - [ ] Coursera 课程:
        - [ ] [RNA 二级结构问题（视频）](https://www.coursera.org/learn/algorithmic-thinking-2/lecture/80RrW/the-rna-secondary-structure-problem)
        - [ ] [动态规划算法（视频）](https://www.coursera.org/learn/algorithmic-thinking-2/lecture/PSonq/a-dynamic-programming-algorithm)
        - [ ] [DP 算法描述（视频）](https://www.coursera.org/learn/algorithmic-thinking-2/lecture/oUEK2/illustrating-the-dp-algorithm)
        - [ ] [DP 算法的运行时间（视频）](https://www.coursera.org/learn/algorithmic-thinking-2/lecture/nfK2r/running-time-of-the-dp-algorithm)
        - [ ] [DP vs 递归实现（视频）](https://www.coursera.org/learn/algorithmic-thinking-2/lecture/M999a/dp-vs-recursive-implementation)
        - [ ] [全局成对序列排列（视频）](https://www.coursera.org/learn/algorithmic-thinking-2/lecture/UZ7o6/global-pairwise-sequence-alignment)
        - [ ] [本地成对序列排列（视频）](https://www.coursera.org/learn/algorithmic-thinking-2/lecture/WnNau/local-pairwise-sequence-alignment)

- ### 设计模式
    - [ ] [UML 统一建模语言概览 (视频)](https://www.youtube.com/watch?v=3cmzqZzwNDM&list=PLGLfVvz_LVvQ5G-LdJ8RLqe-ndo7QITYc&index=3)
    - [ ] 主要有如下的设计模式:
        - [ ] 策略模式（strategy）
        - [ ] 单例模式（singleton）
        - [ ] 适配器模式（adapter）
        - [ ] 原型模式（prototype）
        - [ ] 装饰器模式（decorator）
        - [ ] 访问者模式（visitor）
        - [ ] 工厂模式，抽象工厂模式（factory, abstract factory）
        - [ ] 外观模式（facade）
        - [ ] 观察者模式（observer）
        - [ ] 代理模式（proxy）
        - [ ] 委托模式（delegate）
        - [ ] 命令模式（command）
        - [ ] 状态模式（state）
        - [ ] 备忘录模式（memento）
        - [ ] 迭代器模式（iterator）
        - [ ] 组合模式（composite）
        - [ ] 享元模式（flyweight）
    - [ ] [系列视频（27个）](https://www.youtube.com/playlist?list=PLF206E906175C7E07)
    - [ ] [书籍：《Head First设计模式》](https://www.amazon.com/Head-First-Design-Patterns-Freeman/dp/0596007124)
        - I know the canonical book is "Design Patterns: Elements of Reusable Object-Oriented Software", but Head First is great for beginners to OO.
    - [Handy reference: 101 Design Patterns & Tips for Developers](https://sourcemaking.com/design-patterns-and-tips)

- ### 组合（Combinatorics） (n 中选 k 个) & 概率（Probability）
    - [ ] [数据技巧: 如何找出阶乘、排列和组合(选择)（视频）](https://www.youtube.com/watch?v=8RRo6Ti9d0U)
    - [ ] [来点学校的东西: 概率（视频）](https://www.youtube.com/watch?v=sZkAAk9Wwa4)
    - [ ] [来点学校的东西: 概率和马尔可夫链（视频）](https://www.youtube.com/watch?v=dNaJg-mLobQ)
    - [ ] 可汗学院:
        - 课程设置:
            - [ ] [概率理论基础](https://www.khanacademy.org/math/probability/probability-and-combinatorics-topic)
        - 只有视频 - 41 (每一个都短小精悍):
            - [ ] [概率解释（视频）](https://www.youtube.com/watch?v=uzkc-qNVoOk&list=PLC58778F28211FA19)

- ### NP, NP-Completeness和近似算法
    - 知道最经典的一些 NP-Completeness 问题，比如旅行商问题和背包问题，
    而且能在面试官试图忽悠你的时候识别出他们。
    - 知道 NP-Completeness 是什么意思.
    - [ ] [计算复杂度（视频）](https://www.youtube.com/watch?v=moPtwq_cVH8&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb&index=23)
    - [ ] Simonson:
        - [ ] [贪心算法. II & 介绍 NP-Completeness（视频）](https://youtu.be/qcGnJ47Smlo?list=PLFDnELG9dpVxQCxuD-9BSy2E7BWY3t5Sm&t=2939)
        - [ ] [NP-Completeness II & 归约（视频）](https://www.youtube.com/watch?v=e0tGC6ZQdQE&index=16&list=PLFDnELG9dpVxQCxuD-9BSy2E7BWY3t5Sm)
        - [ ] [NP-Completeness III（视频）](https://www.youtube.com/watch?v=fCX1BGT3wjE&index=17&list=PLFDnELG9dpVxQCxuD-9BSy2E7BWY3t5Sm)
        - [ ] [NP-Completeness IV（视频）](https://www.youtube.com/watch?v=NKLDp3Rch3M&list=PLFDnELG9dpVxQCxuD-9BSy2E7BWY3t5Sm&index=18)
    - [ ] Skiena:
        - [ ] [CSE373 2012 - 课程 23 - 介绍 NP-Completeness IV（视频）](https://youtu.be/KiK5TVgXbFg?list=PLOtl7M3yp-DV69F32zdK7YJcNXpTunF2b&t=1508)
        - [ ] [CSE373 2012 - 课程 24 - NP-Completeness证明（视频）](https://www.youtube.com/watch?v=27Al52X3hd4&index=24&list=PLOtl7M3yp-DV69F32zdK7YJcNXpTunF2b)
        - [ ] [CSE373 2012 - 课程 25 - NP-Completeness挑战（视频）](https://www.youtube.com/watch?v=xCPH4gwIIXM&index=25&list=PLOtl7M3yp-DV69F32zdK7YJcNXpTunF2b)
        - [ ] [CSE373 2020年 - 第26讲 - NP-Completeness挑战（视频）](https://www.youtube.com/watch?v=_EzetTkG_Cc&list=PLOtl7M3yp-DX6ic0HGT0PUX_wiNmkWkXx&index=26)
    - [ ] [复杂度: P, NP, NP-完全性, 规约（视频）](https://www.youtube.com/watch?v=eHZifpgyH_4&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp&index=22)
    - [ ] [复杂度: 近视算法 Algorithms（视频）](https://www.youtube.com/watch?v=MEz1J9wY2iM&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp&index=24)
    - [ ] [复杂度: 固定参数算法（视频）](https://www.youtube.com/watch?v=4q-jmGrmxKs&index=25&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp)
    - Peter Norvik 讨论旅行商问题的近似最优解:
        - [Jupyter 笔记本](http://nbviewer.jupyter.org/url/norvig.com/ipython/TSP.ipynb)
    - 《算法导论》（CLRS）的第 1048 - 1140 页。

- ### 计算机如何处理程序

    - [ ] [CPU如何执行程序（视频）](https://www.youtube.com/watch?v=XM4lGflQFvA)
    - [ ] [计算机如何进行计算 - 算术逻辑单元（视频）](https://youtu.be/1I5ZMmrOfnA)
    - [ ] [寄存器和RAM（视频）](https://youtu.be/fpnE6UAfbtU)
    - [ ] [中央处理器（CPU）（视频）](https://youtu.be/FZGugFqdr60)
    - [ ] [指示和程序（视频）](https://youtu.be/zltgXvg6r3k)

- ### 缓存（Cache）

    - [ ] LRU 缓存:
        - [ ] [LRU 的魔力 (100 Days of Google Dev)（视频）](https://www.youtube.com/watch?v=R5ON3iwx78M)
        - [ ] [实现 LRU（视频）](https://www.youtube.com/watch?v=bq6N7Ym81iI)
        - [ ] [LeetCode - 146 LRU Cache (C++)（视频）](https://www.youtube.com/watch?v=8-FZRAjR7qU)
    - [ ] CPU 缓存:
        - [ ] [MIT 6.004 L15: 存储体系（视频）](https://www.youtube.com/watch?v=vjYF_fAZI5E&list=PLrRW1w6CGAcXbMtDFj205vALOGmiRc82-&index=24)
        - [ ] [MIT 6.004 L16: 缓存的问题（视频）](https://www.youtube.com/watch?v=ajgC3-pyGlk&index=25&list=PLrRW1w6CGAcXbMtDFj205vALOGmiRc82-)

- ### 进程（Processe）和线程（Thread）
    - [ ] 计算机科学 162 - 操作系统 (25 个视频):
        - 视频 1-11 是关于进程和线程
        - [操作系统和系统编程（视频）](https://archive.org/details/ucberkeley-webcast-PL-XXv-cvA_iBDyz-ba4yDskqMDY6A1w_c)
    - [进程和线程的区别是什么?](https://www.quora.com/What-is-the-difference-between-a-process-and-a-thread)
    - 涵盖了:
        - 进程、线程、协程
            - 进程和线程的区别
            - 进程
            - 线程
            - 锁
            - 互斥
            - 信号量
            - 监控
            - 他们是如何工作的
            - 死锁
            - 活锁
        - CPU 活动, 中断, 上下文切换
        - 现代多核处理器的并发式结构
        - [分页（paging），分段（segmentation）和虚拟内存（视频）](https://www.youtube.com/watch?v=LKe7xK0bF7o&list=PLCiOXwirraUCBE9i_ukL8_Kfg6XNv7Se8&index=2)
        - [中断（视频）](https://www.youtube.com/watch?v=uFKi2-J-6II&list=PLCiOXwirraUCBE9i_ukL8_Kfg6XNv7Se8&index=3)
        - 进程资源需要（内存：代码、静态存储器、栈、堆、文件描述符、I/O）
        - 线程资源需要（在同一个进程内和其他线程共享以上（除了栈）的资源，但是每个线程都有独立的程序计数器、栈计数器、寄存器和栈）
        - Fork 操作是真正的写时复制（只读），直到新的进程写到内存中，才会生成一份新的拷贝。
        - 上下文切换
            - [操作系统和底层硬件如何启动上下文切换？](https://www.javatpoint.com/what-is-the-context-switching-in-the-operating-system)
    - [ ] [C++ 的线程 (系列 - 10 个视频)](https://www.youtube.com/playlist?list=PL5jc9xFGsL8E12so1wlMS0r0hTQoJL74M)
    - [ ] [CS 377 春季'14：马萨诸塞大学的操作系统](https://www.youtube.com/playlist?list=PLacuG5pysFbDQU8kKxbUh4K5c1iL5_k7k)
    - [ ] Python 的并发 (视频):
        - [ ] [线程系列](https://www.youtube.com/playlist?list=PL1H1sBF1VAKVMONJWJkmUh6_p8g4F2oy1)
        - [ ] [Python 线程](https://www.youtube.com/watch?v=Bs7vPNbB9JM)
        - [ ] [理解 Python 的 GIL (2010)](https://www.youtube.com/watch?v=Obt-vMVdM8s)
            - [参考](http://www.dabeaz.com/GIL)
        - [ ] [David Beazley - Python 协程 - PyCon 2015](https://www.youtube.com/watch?v=MCs5OvhV9S4)
        - [ ] [Keynote David Beazley - 兴趣主题 (Python 异步 I/O)](https://www.youtube.com/watch?v=ZzfHjytDceU)
        - [ ] [Python 中的互斥](https://www.youtube.com/watch?v=0zaPs8OtyKY)

- ### 测试
    - 涵盖了:
        - 单元测试是如何工作的
        - 什么是模拟对象
        - 什么是集成测试
        - 什么是依赖注入
    - [ ] [James Bach 讲敏捷软件测试（视频）](https://www.youtube.com/watch?v=SAhJf36_u5U)
    - [ ] [James Bach 软件测试公开课（视频）](https://www.youtube.com/watch?v=ILkT_HV9DVU)
    - [ ] [Steve Freeman - 测试驱动的开发（视频）](https://vimeo.com/83960706)
        - [slides](http://gotocon.com/dl/goto-berlin-2013/slides/SteveFreeman_TestDrivenDevelopmentThatsNotWhatWeMeant.pdf)
    - [ ] 依赖注入:
        - [ ] [视频](https://www.youtube.com/watch?v=IKD2-MAkXyQ)
        - [ ] [测试之道](http://jasonpolites.github.io/tao-of-testing/ch3-1.1.html)
    - [ ] [如何编写测试](http://jasonpolites.github.io/tao-of-testing/ch4-1.1.html)

- ### 字符串搜索和操作
    - [ ] [Sedgewick──后缀数组（Suffix Arrays）（视频）](https://www.coursera.org/learn/algorithms-part2/lecture/TH18W/suffix-arrays)
    - [ ] [Sedgewick──子字符串搜寻（视频）](https://www.coursera.org/learn/algorithms-part2/home/week/4)
        - [ ] [1. 子字符串搜寻导论](https://www.coursera.org/learn/algorithms-part2/lecture/n3ZpG/introduction-to-substring-search)
        - [ ] [2. 子字符串搜寻──暴力法](https://www.coursera.org/learn/algorithms-part2/lecture/2Kn5i/brute-force-substring-search)
        - [ ] [3. KMP算法](https://www.coursera.org/learn/algorithms-part2/lecture/TAtDr/knuth-morris-pratt)
        - [ ] [4. Boyer-Moore算法](https://www.coursera.org/learn/algorithms-part2/lecture/CYxOT/boyer-moore)
        - [ ] [5. Rabin-Karp算法](https://www.coursera.org/learn/algorithms-part2/lecture/3KiqT/rabin-karp)
    - [ ] [文本的搜索模式（视频）](https://www.coursera.org/learn/data-structures/lecture/tAfHI/search-pattern-in-text)

- ### 字典树（Tries）

    - 需要注意的是，字典树各式各样。有些有前缀，而有些则没有。有些使用字符串而不使用比特位来追踪路径。
    - [Sedgewick──字典树（3个视频）](https://www.coursera.org/learn/algorithms-part2/home/week/4)
        - [ ] [1. R Way字典树](https://www.coursera.org/learn/algorithms-part2/lecture/CPVdr/r-way-tries)
        - [ ] [2. 三元搜索树](https://www.coursera.org/learn/algorithms-part2/lecture/yQM8K/ternary-search-tries)
        - [ ] [3. 基于字符串的操作](https://www.coursera.org/learn/algorithms-part2/lecture/jwNmV/character-based-operations)
    - [ ] [数据结构笔记及编程技术](http://www.cs.yale.edu/homes/aspnes/classes/223/notes.html#Tries)
    - [ ] 短课程视频：
        - [ ] [对字典树的介绍（视频）](https://www.coursera.org/learn/data-structures-optimizing-performance/lecture/08Xyf/core-introduction-to-tries)
        - [ ] [字典树的性能（视频）](https://www.coursera.org/learn/data-structures-optimizing-performance/lecture/PvlZW/core-performance-of-tries)
        - [ ] [实现一棵字典树（视频）](https://www.coursera.org/learn/data-structures-optimizing-performance/lecture/DFvd3/core-implementing-a-trie)
    - [ ] [字典树：一个被忽略的数据结构](https://www.toptal.com/java/the-trie-a-neglected-data-structure)
    - [ ] [TopCoder —— 使用字典树](https://www.topcoder.com/community/data-science/data-science-tutorials/using-tries/)
    - [ ] [标准教程（现实中的用例）（视频）](https://www.youtube.com/watch?v=TJ8SkcUSdbU)
    - [ ] [MIT，高阶数据结构，字符串（视频中间有点困难）（视频）](https://www.youtube.com/watch?v=NinWEPPrkDQ&index=16&list=PLUl4u3cNGP61hsJNdULdudlRL493b-XZf)

- ### 浮点数
    - [ ] 简单的8位: [浮点数的表示 - 1（视频 - 计算中有错误 - 请查看视频描述）](https://www.youtube.com/watch?v=ji3SfClm8TU)

- ### Unicode
    - [ ] [每一个软件开发者的绝对最低限度，必须要知道的关于 Unicode 和字符集知识](http://www.joelonsoftware.com/articles/Unicode.html)
    - [ ] [关于处理文本需要的编码和字符集，每个程序员绝对需要知道的知识](http://kunststube.net/encoding/)

- ### 字节序（Endianness）
    - [大/小端序](https://web.archive.org/web/20180107141940/http://www.cs.umd.edu:80/class/sum2003/cmsc311/Notes/Data/endian.html)
    - [大端序 Vs 小端序（视频）](https://www.youtube.com/watch?v=JrNF0KRAlyo)
    - [由里入内的大端序与小端序（视频）](https://www.youtube.com/watch?v=oBSuXP-1Tc0)
        - 对于内核开发非常具有技术性，如果大多数的内容听不懂也没关系。
        - 前半部就已经足够了。

- ### 网络（视频）
    - [ ] [UDP 和 TCP：网络传输协议中的数据压缩（视频）](https://www.youtube.com/watch?v=Vdc8TCESIg8)
    - [ ] [TCP/IP 和 OSI 模型解释！（视频）](https://www.youtube.com/watch?v=e5DEVa9eSN0)
    - [ ] [互联网上的数据包传输。网络和 TCP/IP 教程。（视频）](https://www.youtube.com/watch?v=nomyRJehhnM)
    - [ ] [HTTP（视频）](https://www.youtube.com/watch?v=WGJrLqtX7As)
    - [ ] [SSL 和 HTTPS（视频）](https://www.youtube.com/watch?v=S2iBR2ZlZf0)
    - [ ] [SSL/TLS（视频）](https://www.youtube.com/watch?v=Rp3iZUvXWlM)
    - [ ] [HTTP 2.0（视频）](https://www.youtube.com/watch?v=E9FxNzv1Tr8)
    - [ ] [视频系列（21个视频）](https://www.youtube.com/playlist?list=PLEbnTDJUr_IegfoqO4iPnPYQui46QqT0j)
    - [ ] [子网络解密 - 第五部分 经典内部域名指向 CIDR 标记（视频）](https://www.youtube.com/watch?v=t5xYI0jzOf4)
    - [ ] 套接字（Sockets）：
        - [Java──套接字──介绍（视频）](https://www.youtube.com/watch?v=6G_W54zuadg&t=6s)
        - [套接字编程（视频）](https://www.youtube.com/watch?v=G75vN2mnJeQ)

## 当面试来临的时候

随着下面列举的问题思考下你可能会遇到的 20 个面试问题，每个问题准备 2-3 种回答。
准备点故事，不要只是摆一些你完成的事情的数据，相信我，人人都喜欢听故事。

- 你为什么想得到这份工作？
- 你解决过的最有难度的问题是什么？
- 面对过的最大挑战是什么?
- 见过的最好或者最坏的设计是怎么样的?
- 对某个产品提出改进建议。
- 你作为一个个体同时也是团队的一员，如何达到最好的工作状态?
- 你的什么技能或者经验是你的角色中不可或缺的，为什么？
- 你在某份工作或某个项目中最享受的是什么?
- 你在某份工作或某个项目中面临过的最大挑战是什么?
- 你在某份工作或某个项目中遇到过的最硬的 Bug 是什么样的？
- 你在某份工作或某个项目中学到了什么？
- 你在某份工作或某个项目中哪些地方还可以做的更好？

## 问面试官的问题

我会问的一些：(可能我已经知道了答案但我想听听面试官的看法或者了解团队的前景):

- 团队多大规模?
- 开发周期是怎样的? 会使用瀑布流/极限编程/敏捷开发么?
- 经常会为截止日期（deadlines）加班么? 或者是有弹性的?
- 团队里怎么做技术选型?
- 每周平均开多少次会?
- 你觉得工作环境有助于员工集中精力吗?
- 目前正在做什么工作?
- 喜欢这些事情吗?
- 工作期限是怎么样的?
- 工作生活怎么平衡?

## 额外书籍

    你可以从以下的书单挑选你有兴趣的主题来研读。

- [UNIX环境高级编程](https://www.amazon.com/dp/013937681X)
    - 老，但却很棒
- [Linux 命令行大全](https://www.amazon.com/dp/1593273894/)
    - 现代选择
- [TCP-IP详解系列](https://en.wikipedia.org/wiki/TCP/IP_Illustrated)
- [Head First 设计模式](https://www.amazon.com/gp/product/0596007124/)
    - 设计模式入门介绍
- [设计模式：可复用面向对象软件的基础](https://www.amazon.com/Design-Patterns-Elements-Reusable-Object-Oriented/dp/0201633612)
    - 也被称为“四人帮”（Gang of Four(GOF)）
    - 经典设计模式书籍
- [算法设计手冊（Skiena）](http://www.amazon.com/Algorithm-Design-Manual-Steven-Skiena/dp/1849967202)
    - 作为复习以及问题辨别
    - 这本书中算法的部分难度已经超过面试会出现的
    - 本书分为两个部分:
        - 数据结构和算法课本
            - 优点:
                - 跟其他算法课本一样是个很棒的复习素材
                - 包含作者以往解决工业及学术上问题的经验的故事
                - 含C语言代码示例
            - 缺点:
                - 某些地方跟《算法导论》（CLRS）一样艰深，但在某些主题，算法导论或许是更好的选择。
                - 第7、8、9章有点难以消化，因为某些地方并没有解释得很清楚，或者根本上我就是个学渣
                - 别会错意了，我很喜欢 Skiena 的教学方法以及他的风格。
        - 算法目录:
            - 这个部分是买这本书的最大原因
            - 我即将着手进行这部分，一旦完成这部分我会再更新上来
    - 可以在 kindle 上租
    - 解答：
        - [解答](https://web.archive.org/web/20150404194210/http://www.algorithm.cs.sunysb.edu/algowiki/index.php/The_Algorithms_Design_Manual_(Second_Edition))
    - [勘误表](http://www3.cs.stonybrook.edu/~skiena/algorist/book/errata)
- [算法](http://jeffe.cs.illinois.edu/teaching/algorithms/) (Jeff Erickson)
- [编程卓越之道（第一卷）：深入理解计算机](https://www.amazon.com/Write-Great-Code-Understanding-Machine/dp/1593270038)
    - 该书于2004年出版，虽然有些过时，但是对于简单了解计算机而言，这是一个了不起的资源
    - 作者发明了[高阶组合语言 HLA](https://en.wikipedia.org/wiki/High_Level_Assembly)，所以提到，并且举了一些HLA的例子。里面没有用到很多，但都是很棒的组合语言的例子。
    - 这些章节值得阅读，为你提供良好的基础：
        - 第2章──数字表示
        - 第3章──二进制算术和位运算
        - 第4章──浮点表示
        - 第5章──字符表示
        - 第6章──内存组织和访问
        - 第7章──组合数据类型和内存对象
        - 第9章──CPU体系结构
        - 第10章──指令集架构
        - 第11章──内存体系结构和组织
- [算法导论](https://www.amazon.com/Introduction-Algorithms-fourth-Thomas-Cormen/dp/026204630X)
    - **重要提示**：读这本书的价值有限。本书很好地回顾了算法和数据结构，但不会教你如何编写良好的代码。你必须能够有效地编写一个不错的解决方案
    - 又称 CLR，有时是 CLRS，因为 Stein 最后才加入
- [计算机体系结构，第六版：定量方法](https://www.amazon.com/dp/0128119055)
    - 对于更丰富、更时新（2017年）但较长的处理方式

## 系统设计、可扩展性和数据处理

**如果您有4年以上的工作经验，可以预期会遇到系统设计问题。**

- 可扩展性和系统设计是一个非常广泛的主题，涵盖了许多内容和资源，
因为在设计一个可以扩展的软件/硬件系统时需要考虑很多因素。
预计需要花费相当多的时间来学习这方面的知识。
- 考虑要点：
    - 可扩展性
        - 将大数据集归纳为单一值
        - 将一个数据集转换为另一个数据集
        - 处理海量数据
    - 系统设计
        - 功能集
        - 接口
        - 类层次结构
        - 在特定约束下设计系统
        - 简单性和鲁棒性
        - 权衡
        - 性能分析和优化
- [ ] **从这里开始**: [The System Design Primer](https://github.com/donnemartin/system-design-primer)
- [ ] [HiredInTech的系统设计](http://www.hiredintech.com/system-design/)
- [ ] [如何准备回答技术面试中的设计问题？](https://www.quora.com/How-do-I-prepare-to-answer-design-questions-in-a-technical-interview?redirected_qid=1500023)
- [ ] [通过8个步骤掌握系统设计面试](https://javascript.plainenglish.io/8-steps-guide-to-ace-a-system-design-interview-7a5a797f4d7d)
- [ ] [数据库规范化 - 第一范式、第二范式、第三范式和第四范式（视频）](https://www.youtube.com/watch?v=UrYLYV7WSHM)
- [ ] [系统设计面试 ](https://github.com/checkcheckzz/system-design-interview) - 这个资源有很多内容。浏览文章和示例。我列出了一些示例在下面。
- [ ] [如何在系统设计面试中脱颖而出](https://web.archive.org/web/20120716060051/http://www.palantir.com/2011/10/how-to-rock-a-systems-design-interview/)
- [ ] [每个人都应该了解的数字](http://everythingisdata.wordpress.com/2009/10/17/numbers-everyone-should-know/)
- [ ] [进行上下文切换需要多长时间？](http://blog.tsunanet.net/2010/11/how-long-does-it-take-to-make-context.html)
- [ ] [跨数据中心的事务（视频）](https://www.youtube.com/watch?v=srOgpXECblk)
- [ ] [CAP定理的简明英文介绍](http://ksat.me/a-plain-english-introduction-to-cap-theorem)
- [ ] [MIT 6.824：分布式系统，2020年春季（20个视频）](https://www.youtube.com/watch?v=cQP8WApzIQQ&list=PLrw6a1wE39_tb2fErI4-WkMbsvGQk9_UB)
- [ ] 共识算法：
    - [ ] Paxos - [Paxos协议 - Computerphile（视频）](https://www.youtube.com/watch?v=s8JqcZtvnsM)
    - [ ] Raft - [Raft分布式共识算法简介（视频）](https://www.youtube.com/watch?v=P9Ydif5_qvE)
        - [ ] [易于理解的论文](https://raft.github.io/)
        - [ ] [信息图](http://thesecretlivesofdata.com/raft/)
- [ ] [一致性哈希](http://www.tom-e-white.com/2007/11/consistent-hashing.html)
- [ ] [NoSQL模式](http://horicky.blogspot.com/2009/11/nosql-patterns.html)
- [ ] 可扩展性：
    - 您不需要掌握所有这些内容，只需选择一些您感兴趣的。
    - [ ] [优秀的概述（视频）](https://www.youtube.com/watch?v=-W9F__D3oY4)
    - [ ] 短系列：
        - [克隆](http://www.lecloud.net/post/7295452622/scalability-for-dummies-part-1-clones)
        - [数据库](http://www.lecloud.net/post/7994751381/scalability-for-dummies-part-2-database)
        - [缓存](http://www.lecloud.net/post/9246290032/scalability-for-dummies-part-3-cache)
        - [异步性](http://www.lecloud.net/post/9699762917/scalability-for-dummies-part-4-asynchronism)
    - [ ] [可扩展的Web架构和分布式系统](http://www.aosabook.org/en/distsys.html)
    - [ ] [分布式计算的谬误解释](https://pages.cs.wisc.edu/~zuyu/files/fallacies.pdf)
    - [ ] [Jeff Dean - 在Google构建软件系统以及吸取的教训（视频）](https://www.youtube.com/watch?v=modXC5IWTJI)
    - [ ] [架构师为规模而设计的介绍](http://lethain.com/introduction-to-architecting-systems-for-scale/)
    - [ ] [缩放移动游戏以面向全球受众使用App Engine和Cloud Datastore（视频）](https://www.youtube.com/watch?v=9nWyWwY2Onc)
    - [ ] [谷歌是如何进行面向全球基础设施的大规模工程的（视频）](https://www.youtube.com/watch?v=H4vMcD7zKM0)
    - [ ] [算法的重要性](https://www.topcoder.com/thrive/articles/The%20Importance%20of%20Algorithms)
    - [ ] [分片](http://highscalability.com/blog/2009/8/6/an-unorthodox-approach-to-database-design-the-coming-of-the.html)
    - [ ] [针对长期目标的工程 - Astrid Atkinson主题演讲（视频）](https://www.youtube.com/watch?v=p0jGmgIrf_M&list=PLRXxvay_m8gqVlExPC5DG3TGWJTaBgqSA&index=4)
    - [ ] [在30分钟内了解YouTube 7年的可扩展性经验](http://highscalability.com/blog/2012/3/26/7-years-of-youtube-scalability-lessons-in-30-minutes.html)
        - [视频](https://www.youtube.com/watch?v=G-lGCC4KKok)
    - [ ] [PayPal如何使用仅8台VM每天处理数十亿次交易](http://highscalability.com/blog/2016/8/15/how-paypal-scaled-to-billions-of-transactions-daily-using-ju.html)
    - [ ] [如何在大型数据集中去重](https://blog.clevertap.com/how-to-remove-duplicates-in-large-datasets/)
    - [ ] [通过Jon Cowie深入了解Etsy的规模和工程文化（视频）](https://www.youtube.com/watch?v=3vV4YiqKm1o)
    - [ ] [Amazon是如何转向自己的微服务架构的](http://thenewstack.io/led-amazon-microservices-architecture/)
    - [ ] [压缩还是不压缩，这是Uber面临的问题](https://eng.uber.com/trip-data-squeeze/)
    - [ ] [何时应使用近似查询处理？](http://highscalability.com/blog/2016/2/25/when-should-approximate-query-processing-be-used.html)
    - [ ] [谷歌从单一数据中心到故障转移再到本地多家数据中心架构的转变]( http://highscalability.com/blog/2016/2/23/googles-transition-from-single-datacenter-to-failover-to-a-n.html)
    - [ ] [为每天处理数百万请求的图像优化技术](http://highscalability.com/blog/2016/6/15/the-image-optimization-technology-that-serves-millions-of-re.html)
    - [ ] [Patreon架构简介](http://highscalability.com/blog/2016/2/1/a-patreon-architecture-short.html)
    - [ ] [如何在Instagram庞大的推荐引擎中决定您将看到谁？](http://highscalability.com/blog/2016/1/27/tinder-how-does-one-of-the-largest-recommendation-engines-de.html)
    - [ ] [现代缓存设计](http://highscalability.com/blog/2016/1/25/design-of-a-modern-cache.html)
    - [ ] [在Facebook规模下进行直播视频流](http://highscalability.com/blog/2016/1/13/live-video-streaming-at-facebook-scale.html)
    - [ ] [在亚马逊AWS上如何扩展到1100万以上的用户](http://highscalability.com/blog/2016/1/11/a-beginners-guide-to-scaling-to-11-million-users-on-amazons.html)
    - [ ] [全面了解Netflix整个堆栈](http://highscalability.com/blog/2015/11/9/a-360-degree-view-of-the-entire-netflix-stack.html)
    - [ ] [延迟无处不在，而且它会让您丧失销售机会 - 如何应对](http://highscalability.com/latency-everywhere-and-it-costs-you-sales-how-crush-it)
    - [ ] [Instagram的动力：数百个实例，几十种技术](http://instagram-engineering.tumblr.com/post/13649370142/what-powers-instagram-hundreds-of-instances)
    - [ ] [Salesforce架构 - 如何处理每天13亿次交易](http://highscalability.com/blog/2013/9/23/salesforce-architecture-how-they-handle-13-billion-transacti.html)
    - [ ] [ESPN规模上的架构 - 每秒操作10万次“嘟嘟噜嘟嘟噜”](http://highscalability.com/blog/2013/11/4/espns-architecture-at-scale-operating-at-100000-duh-nuh-nuhs.html)
    - [ ]  在下面的“消息、序列化和队列系统”部分查看一些将服务连接在一起的技术信息
    - [ ] Twitter:
        - [O'Reilly MySQL CE 2011: Jeremy Cole, "Big and Small Data at @Twitter" (视频)](https://www.youtube.com/watch?v=5cKTP36HVgI)
        - [时间轴扩展](https://www.infoq.com/presentations/Twitter-Timeline-Scalability)
    - 欲知更多信息，请参阅[Video Series](#video-series) 部分中的“Mining Massive Datasets”视频系列
- [ ] 练习系统设计过程：以下是一些建议您在纸上尝试的想法，每个想法都有一些关于如何在现实世界中处理的文档：
    - 复习: [The System Design Primer](https://github.com/donnemartin/system-design-primer)
    - [HiredInTech的系统设计](http://www.hiredintech.com/system-design/)
    - [速查表](https://github.com/jwasham/coding-interview-university/blob/main/extras/cheat%20sheets/system-design.pdf)
    - 流程：
        1. 理解问题和范围：
            - 定义用例，与面试官的帮助
            - 提出额外的功能
            - 移除面试官认为超出范围的项目
            - 假设需要高可用性，并将其添加为用例
        2. 考虑限制：
            - 询问每月有多少个请求
            - 询问每秒有多少个请求（他们可能会主动提供或让您计算）
            - 估计读取与写入的百分比
            - 保持估计时考虑80/20法则
            - 每秒写入多少数据
            - 在5年内所需的总存储量
            - 每秒读取多少数据
        3. 抽象设计：
            - 层（服务、数据、缓存）
            - 基础架构：负载均衡、消息传递
            - 驱动服务的任何关键算法的粗略概述
            - 考虑瓶颈并确定解决方案
    - 练习：
        - [设计一个随机唯一ID生成系统](https://blog.twitter.com/2010/announcing-snowflake)
        - [设计一个键值数据库](http://www.slideshare.net/dvirsky/introduction-to-redis)
        - [设计一个图片分享系统](http://highscalability.com/blog/2011/12/6/instagram-architecture-14-million-users-terabytes-of-photos.html)
        - [设计一个推荐系统](http://ijcai13.org/files/tutorial_slides/td3.pdf)
        - [设计一个URL缩短系统：来自上面的复制](http://www.hiredintech.com/system-design/the-system-design-process/)
        - [设计一个缓存系统](https://web.archive.org/web/20220217064329/https://adayinthelifeof.nl/2011/02/06/memcache-internals/)


## 附加学习

    我把它们加进来是为了让你成为更全方位的软件工程师，并且留意一些技术以及算法，让你拥有更大的工具箱。

- ### 编译器
    - [编译器的工作方式，约1分钟（视频）](https://www.youtube.com/watch?v=IhC7sdYe-Jg)
    - [Harvard CS50-编译器（视频）](https://www.youtube.com/watch?v=CSZLNYF4Klo)
    - [C ++（视频）](https://www.youtube.com/watch?v=twodd1KFfGk)
    - [了解编译器优化（C ++）（视频）](https://www.youtube.com/watch?v=FnGCDLhaxKU)

- ### Emacs and vi(m)
    - 熟悉基于 unix 的代码编辑器
    - vi(m):
        - [使用 vim 进行编辑 01 - 安装, 设置和模式 (视频)](https://www.youtube.com/watch?v=5givLEMcINQ&index=1&list=PL13bz4SHGmRxlZVmWQ9DvXo1fEg4UdGkr)
        - [VIM 的冒险之旅](http://vim-adventures.com/)
        - 4 个视频集:
            - [vi/vim 编辑器 - 课程 1](https://www.youtube.com/watch?v=SI8TeVMX8pk)
            - [vi/vim 编辑器 - 课程 2](https://www.youtube.com/watch?v=F3OO7ZIOaJE)
            - [vi/vim 编辑器 - 课程 4](https://www.youtube.com/watch?v=1lYD5gwgZIA)
            - [vi/vim 编辑器 - 课程 3](https://www.youtube.com/watch?v=ZYEccA_nMaI)
        - [使用 Vi 而不是 Emacs](http://www.cs.yale.edu/homes/aspnes/classes/223/notes.html#Using_Vi_instead_of_Emacs)
    - emacs:
        - [基础 Emacs 教程 (视频)](https://www.youtube.com/watch?v=hbmV1bnQ-i0)
        - 3 个视频集:
            - [Emacs 教程 (初学者) -第 1 部分- 文件命令, 剪切/复制/粘贴,  自定义命令](https://www.youtube.com/watch?v=ujODL7MD04Q)
            - [Emacs 教程 (初学者 -第 2 部分- Buffer 管理, 搜索, M-x grep 和 rgrep 模式](https://www.youtube.com/watch?v=XWpsRupJ4II)
            - [Emacs 教程 (初学者 -第 3 部分- 表达式, 声明, ~/.emacs 文件和包机制](https://www.youtube.com/watch?v=paSgzPso-yc)
        - [Evil 模式: 或许, 我是怎样对 Emacs 路人转粉的 (视频)](https://www.youtube.com/watch?v=JWD1Fpdd4Pc)
        - [使用 Emacs 开发 C 程序](http://www.cs.yale.edu/homes/aspnes/classes/223/notes.html#Writing_C_programs_with_Emacs)
	- [Emacs 绝对初学者指南（David Wilson的视频）](https://www.youtube.com/watch?v=48JlgiBpw_I&t=0s)
	- [Emacs 绝对初学者指南（David Wilson 批注）](https://systemcrafters.net/emacs-essentials/absolute-beginners-guide-to-emacs/)

- ### Unix 命令行工具
    - 下列内容包含优秀工具
    - bash
    - cat
    - grep
    - sed
    - awk
    - curl or wget
    - sort
    - tr
    - uniq
    - [strace](https://en.wikipedia.org/wiki/Strace)
    - [tcpdump](https://danielmiessler.com/study/tcpdump/)

- ### 信息论 (视频)
    - [Khan Academy 可汗学院](https://www.khanacademy.org/computing/computer-science/informationtheory)
    - 更多有关马尔可夫的内容:
        - [马尔可夫内容生成（Core Markov Text Generation）](https://www.coursera.org/learn/data-structures-optimizing-performance/lecture/waxgx/core-markov-text-generation)
        - [Core Implementing Markov Text Generation马尔可夫内容生成实现](https://www.coursera.org/learn/data-structures-optimizing-performance/lecture/gZhiC/core-implementing-markov-text-generation)
        - [一个马尔可夫内容生成器的项目（Project = Markov Text Generation Walk Through）](https://www.coursera.org/learn/data-structures-optimizing-performance/lecture/EUjrq/project-markov-text-generation-walk-through)
    - 关于更多信息，请参照下方 MIT 6.050J 信息和系统复杂度的内容。

- ### 奇偶校验位 & 汉明码 (视频)
    - [入门](https://www.youtube.com/watch?v=q-3BctoUpHE)
    - [奇偶校验位](https://www.youtube.com/watch?v=DdMcAUlxh1M)
    - 汉明码(Hamming Code):
        - [发现错误](https://www.youtube.com/watch?v=1A_NcXxdoCc)
        - [修正错误](https://www.youtube.com/watch?v=JAMLuxdHH8o)
    - [检查错误](https://www.youtube.com/watch?v=wbH2VxzmoZk)

- ### 压缩
    - 观看之前，请先确定观看了信息论的视频
    - Computerphile (视频)：
        - [压缩](https://www.youtube.com/watch?v=Lto-ajuqW3w)
        - [压缩熵值](https://www.youtube.com/watch?v=M5c_RFKVkko)
        - [由上而下的树 (霍夫曼编码树)](https://www.youtube.com/watch?v=umTbivyJoiI)
        - [额外比特 - 霍夫曼编码树](https://www.youtube.com/watch?v=DV8efuB3h2g)
        - [优雅的压缩数据 (无损数据压缩方法)](https://www.youtube.com/watch?v=goOa3DGezUA)
        - [Text Compression Meets Probabilities](https://www.youtube.com/watch?v=cCDCfoHTsaU)
    - [数据压缩的艺术](https://www.youtube.com/playlist?list=PLOU2XLYxmsIJGErt5rrCqaSGTMyyqNt2H)
    - [(可选) 谷歌开发者：GZIP 还差远了呢!](https://www.youtube.com/watch?v=whGwm0Lky2s)

- ### 垃圾回收
    - [ ] [Python 中的垃圾回收 (视频)](https://www.youtube.com/watch?v=iHVs_HkjdmI)
    - [ ] [深度解析：论垃圾回收在 JAVA 中的重要性](https://www.infoq.com/presentations/garbage-collection-benefits)
    - [ ] [深度解析：论垃圾回收在 Python 中的重要性(视频)](https://www.youtube.com/watch?v=P-8Z0-MhdQs&list=PLdzf4Clw0VbOEWOS_sLhT_9zaiQDrS5AR&index=3)

- ### 并行编程
    - [ ] [Coursera (Scala)](https://www.coursera.org/learn/parprog1/home/week/1)
    - [ ] [用于高性能并行计算的高效Python（视频）](https://www.youtube.com/watch?v=uY85GkaYzBk)

- ### 消息传递，序列化和队列系统
    - [Thrift](https://thrift.apache.org/)
        - [教程](http://thrift-tutorial.readthedocs.io/en/latest/intro.html)
    - [协议缓冲](https://developers.google.com/protocol-buffers/)
        - [教程](https://developers.google.com/protocol-buffers/docs/tutorials)
    - [gRPC](http://www.grpc.io/)
        - [gRPC 对于JAVA开发者的入门教程（视频）](https://www.youtube.com/watch?v=5tmPvSe7xXQ&list=PLcTqM9n_dieN0k1nSeN36Z_ppKnvMJoly&index=1)
    - [Redis](http://redis.io/)
        - [教程](http://try.redis.io/)
    - [Amazon的 SQS 系统 (队列)](https://aws.amazon.com/sqs/)
    - [Amazon的 SNS 系统 (pub-sub)](https://aws.amazon.com/sns/)
    - [RabbitMQ](https://www.rabbitmq.com/)
        - [入门教程](https://www.rabbitmq.com/getstarted.html)
    - [Celery](http://www.celeryproject.org/)
        - [Celery入门](http://docs.celeryproject.org/en/latest/getting-started/first-steps-with-celery.html)
    - [ZeroMQ](http://zeromq.org/)
        - [入门教程](http://zeromq.org/intro:read-the-manual)
    - [ActiveMQ](http://activemq.apache.org/)
    - [Kafka](http://kafka.apache.org/documentation.html#introduction)
    - [MessagePack](http://msgpack.org/index.html)
    - [Avro](https://avro.apache.org/)

- ### A*搜索算法
    - [A 搜索算法](https://en.wikipedia.org/wiki/A*_search_algorithm)
    - [A* 路径搜索（E01：算法解释）（视频）](https://www.youtube.com/watch?v=-L-WgKMFuhE)

- ### 快速傅里叶变换
    - [傅立叶变换的交互式指南](https://betterexplained.com/articles/an-interactive-guide-to-the-fourier-transform/)
    - [什么是傅立叶变换？论傅立叶变换的用途](http://www.askamathematician.com/2012/09/q-what-is-a-fourier-transform-what-is-it-used-for/)
    - [什么是傅立叶变换？ (视频)](https://www.youtube.com/watch?v=Xxut2PN-V8Q)
    - [分而治之：FFT（视频）](https://www.youtube.com/watch?v=iTMn0Kt18tg&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp&index=4)
    - [FTT 是什么](http://jakevdp.github.io/blog/2013/08/28/understanding-the-fft/)

- ### 布隆过滤器
    - 给定布隆过滤器m比特位和k个哈希函数，插入和成员检测都会是 O(k)。
    - [布隆过滤器（视频）](https://www.youtube.com/watch?v=-SuTGoFYjZs)
    - [布隆过滤器 | 数据挖掘 | Stanford University（视频）](https://www.youtube.com/watch?v=qBTdukbzc78)
    - [教程](http://billmill.org/bloomfilter-tutorial/)
    - [如何写一个布隆过滤器应用](http://blog.michaelschmatz.com/2016/04/11/how-to-write-a-bloom-filter-cpp/)

- ### HyperLogLog
    - [如何仅使用1.5KB内存计算十亿个不同的对象](http://highscalability.com/blog/2012/4/5/big-data-counting-how-to-count-a-billion-distinct-objects-us.html)

- ### 局部敏感哈希
    - 用于确定文件的相似性
    - MD5 或 SHA 的反义词，用于确定2个文档/字符串是否完全相同
    - [Simhashing（希望如此）变得简单](http://ferd.ca/simhashing-hopefully-made-simple.html)

- ### van Emde Boas 树
    - [分而治之：van Emde Boas 树 (视频)](https://www.youtube.com/watch?v=hmReJCupbNU&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp&index=6)
    - [MIT课堂笔记](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-046j-design-and-analysis-of-algorithms-spring-2012/lecture-notes/MIT6_046JS12_lec15.pdf)

- ### 增强数据结构
    - [CS 61B 第 39 课: 增强数据结构](https://youtu.be/zksIj9O8_jc?list=PL4BBB74C7D2A1049C&t=950)

- ### 平衡查找树（Balanced search trees）
    - 掌握至少一种平衡查找树（并懂得如何实现）：
    - “在各种平衡查找树当中，AVL 树和2-3树已经成为了过去，而红黑树（red-black trees）看似变得越来越受人青睐。
    这种令人特别感兴趣的数据结构，亦称伸展树（splay tree）。
    它可以自我管理，且会使用轮换来移除任何访问过根节点的键。” —— Skiena
    - 因此，在各种各样的平衡查找树当中，我选择了伸展树来实现。
      虽然，通过我的阅读，我发现在面试中并不会被要求实现一棵平衡查找树。
      但是，为了胜人一筹，我们还是应该看看如何去实现。在阅读了大量关于红黑树的代码后，
      我才发现伸展树的实现确实会使得各方面更为高效。
        - 伸展树：插入、查找、删除函数的实现，而如果你最终实现了红黑树，那么请尝试一下：
        - 跳过删除函数，直接实现搜索和插入功能
    - 我希望能阅读到更多关于 B 树的资料，因为它也被广泛地应用到大型的数据集当中。
    - [自平衡二叉查找树](https://en.wikipedia.org/wiki/Self-balancing_binary_search_tree)

    - **AVL 树**
        - 实际中：
        我能告诉你的是，该种树并无太多的用途，但我能看到有用的地方在哪里：
        AVL 树是另一种平衡查找树结构。其可支持时间复杂度为 O(log n) 的查询、插入及删除。
        它比红黑树严格意义上更为平衡，从而导致插入和删除更慢，但遍历却更快。正因如此，才彰显其结构的魅力。
        只需要构建一次，就可以在不重新构造的情况下读取，
        适合于实现诸如语言字典（或程序字典，如一个汇编程序或解释程序的操作码）。
        - [MIT AVL 树 / AVL 树的排序（视频）](https://www.youtube.com/watch?v=FNeL18KsWPc&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb&index=6)
        - [AVL 树（视频）](https://www.coursera.org/learn/data-structures/lecture/Qq5E0/avl-trees)
        - [AVL 树的实现（视频）](https://www.coursera.org/learn/data-structures/lecture/PKEBC/avl-tree-implementation)
        - [分离与合并](https://www.coursera.org/learn/data-structures/lecture/22BgE/split-and-merge)
        - [[Review] AVL Trees (playlist) in 19 minutes (video)](https://www.youtube.com/playlist?list=PL9xmBV_5YoZOUFgdIeOPuH6cfSnNRMau-)

    - **伸展树**
        - 实际中：
        伸展树一般用于缓存、内存分配者、路由器、垃圾回收者、数据压缩、ropes
        （字符串的一种替代品，用于存储长串的文本字符）、
        Windows NT（虚拟内存、网络及文件系统）等的实现。
        - [CS 61B：伸展树（Splay trees）（视频）](https://www.youtube.com/watch?v=Najzh1rYQTo&index=23&list=PL-XXv-cvA_iAlnI-BQr9hjqADPBtujFJd)
        - MIT 教程：伸展树（Splay trees）：
            - 该教程会过于学术，但请观看到最后的10分钟以确保掌握。
            - [视频](https://www.youtube.com/watch?v=QnPl_Y6EqMo)

    - **红黑树**
        - 这些是2-3棵树的翻译（请参见下文）。
        - 实际中：红黑树提供了在最坏情况下插入操作、删除操作和查找操作的时间保证。
        这些时间值的保障不仅对时间敏感型应用有用，例如实时应用，
        还对在其他数据结构中块的构建非常有用，
        而这些数据结构都提供了最坏情况下的保障；
        例如，许多用于计算几何学的数据结构都可以基于红黑树，
        而目前 Linux 内核所采用的完全公平调度器（the Completely Fair Scheduler）也使用到了该种树。
        在 Java 8中，Collection HashMap也从原本用Linked List实现，
        储存特定元素的哈希码，改为用红黑树实现。
        - [Aduni —— 算法 —— 课程4（该链接直接跳到开始部分）（视频）](https://youtu.be/1W3x0f_RmUo?list=PLFDnELG9dpVxQCxuD-9BSy2E7BWY3t5Sm&t=3871)
        - [Aduni —— 算法 —— 课程5（视频）](https://www.youtube.com/watch?v=hm2GHwyKF1o&list=PLFDnELG9dpVxQCxuD-9BSy2E7BWY3t5Sm&index=5)
        - [黑树（Black Tree）](https://en.wikipedia.org/wiki/Red%E2%80%93black_tree)
        - [二分查找及红黑树的介绍](https://www.topcoder.com/community/data-science/data-science-tutorials/an-introduction-to-binary-search-and-red-black-trees/)
        - [[Review] Red-Black Trees (playlist) in 30 minutes (video)](https://www.youtube.com/playlist?list=PL9xmBV_5YoZNqDI8qfOZgzbqahCUmUEin)

    - **2-3查找树**
        - 实际中：
        2-3树的元素插入非常快速，但却有着查询慢的代价（因为相比较 AVL 树来说，其高度更高）。
        - 你会很少用到2-3树。这是因为，其实现过程中涉及到不同类型的节点。因此，人们更多地会选择红黑树。
        - [2-3树的直感与定义（视频）](https://www.youtube.com/watch?v=C3SsdUqasD4&list=PLA5Lqm4uh9Bbq-E0ZnqTIa8LRaL77ica6&index=2)
        - [2-3树的二元观点](https://www.youtube.com/watch?v=iYvBtGKsqSg&index=3&list=PLA5Lqm4uh9Bbq-E0ZnqTIa8LRaL77ica6)
        - [2-3树（学生叙述）（视频）](https://www.youtube.com/watch?v=TOb1tuEZ2X4&index=5&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp)

    - **2-3-4树 (亦称2-4树)**
        - 实际中：
        对于每一棵2-4树，都有着对应的红黑树来存储同样顺序的数据元素。
        在2-4树上进行插入及删除操作等同于在红黑树上进行颜色翻转及轮换。
        这使得2-4树成为一种用于掌握红黑树背后逻辑的重要工具。
        这就是为什么许多算法引导文章都会在介绍红黑树之前，先介绍2-4树，尽管**2-4树在实际中并不经常使用**。
        - [CS 61B Lecture 26：平衡查找树（视频）](https://www.youtube.com/watch?v=zqrqYXkth6Q&index=26&list=PL4BBB74C7D2A1049C)
        - [自底向上的2-4树（视频）](https://www.youtube.com/watch?v=DQdMYevEyE4&index=4&list=PLA5Lqm4uh9Bbq-E0ZnqTIa8LRaL77ica6)
        - [自顶向下的2-4树（视频）](https://www.youtube.com/watch?v=2679VQ26Fp4&list=PLA5Lqm4uh9Bbq-E0ZnqTIa8LRaL77ica6&index=5)

    - **N 叉树（K 叉树、M 叉树）**
        - 注意：N 或 K 指的是分支系数（即树的最大分支数）：
        - 二叉树是一种分支系数为2的树
        - 2-3树是一种分支系数为3的树
        - [K 叉树](https://en.wikipedia.org/wiki/K-ary_tree)

    - **B 树**
        - 有趣的是：为啥叫 B 仍然是一个神秘。因为 B 可代表波音（Boeing）、平衡（Balanced）或 Bayer（联合创造者）
        - 实际中：
        B 树会被广泛适用于数据库中，而现代大多数的文件系统都会使用到这种树（或变种）。
        除了运用在数据库中，B 树也会被用于文件系统以快速访问一个文件的任意块。
        但存在着一个基本的问题，
        那就是如何将文件块 i 转换成一个硬盘块（或一个柱面-磁头-扇区）上的地址。
        - [B 树](https://en.wikipedia.org/wiki/B-tree)
        - [B 树数据结构](http://btechsmartclass.com/data_structures/b-trees.html)
        - [B 树的介绍（视频）](https://www.youtube.com/watch?v=I22wEC1tTGo&list=PLA5Lqm4uh9Bbq-E0ZnqTIa8LRaL77ica6&index=6)
        - [B 树的定义及其插入操作（视频）](https://www.youtube.com/watch?v=s3bCdZGrgpA&index=7&list=PLA5Lqm4uh9Bbq-E0ZnqTIa8LRaL77ica6)
        - [B 树的删除操作（视频）](https://www.youtube.com/watch?v=svfnVhJOfMc&index=8&list=PLA5Lqm4uh9Bbq-E0ZnqTIa8LRaL77ica6)
        - [MIT 6.851 —— 内存层次模块（Memory Hierarchy Models）（视频）](https://www.youtube.com/watch?v=V3omVLzI0WE&index=7&list=PLUl4u3cNGP61hsJNdULdudlRL493b-XZf)
            - 覆盖有高速缓存参数无关型（cache-oblivious）B 树和非常有趣的数据结构
            - 头37分钟讲述的很专业，或许可以跳过（B 指块的大小、即缓存行的大小）
        - [[Review] B-Trees (playlist) in 26 minutes (video)](https://www.youtube.com/playlist?list=PL9xmBV_5YoZNFPPv98DjTdD9X6UI9KMHz)


- ### k-D树
    - 非常适合在矩形或更高维度的对象中查找点数
    - 最适合k近邻
    - [kNN K-d树算法（视频）](https://www.youtube.com/watch?v=Y4ZgLlDfKDg)

- ### 跳表
    - "有一种非常迷幻的数据类型" - Skiena
    - [随机化: 跳表 (视频)](https://www.youtube.com/watch?v=2g9OSRKJuzM&index=10&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp)
    - [更生动详细的解释](https://en.wikipedia.org/wiki/Skip_list)

- ### 网络流
    - [5分钟简析 Ford-Fulkerson──一步步示例 (视频)](https://www.youtube.com/watch?v=v1VgJmkEJW0)
    - [Ford-Fulkerson 算法 (视频)](https://www.youtube.com/watch?v=v1VgJmkEJW0)
    - [网络流 (视频)](https://www.youtube.com/watch?v=2vhN4Ice5jI)

- ### 不相交集 & 联合查找
    - [UCB 61B - 不相交集；排序 & 选择(视频)](https://www.youtube.com/watch?v=MAEGXTwmUsI&list=PL-XXv-cvA_iAlnI-BQr9hjqADPBtujFJd&index=21)
    - [Sedgewick算法──Union-Find（6视频）](https://www.coursera.org/learn/algorithms-part1/home/week/1)

- ### 快速处理的数学
    - [整数运算, Karatsuba 乘法 (视频)](https://www.youtube.com/watch?v=eCaXlAaN2uE&index=11&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb)
    - [中国剩余定理 (在密码学中的使用) (视频)](https://www.youtube.com/watch?v=ru7mWZJlRQg)

- ### 树堆 (Treap)
    - 一个二叉搜索树和一个堆的组合
    - [树堆](https://en.wikipedia.org/wiki/Treap)
    - [数据结构：树堆的讲解（视频）](https://www.youtube.com/watch?v=6podLUYinH8)
    - [集合操作的应用(Applications in set operations)](https://www.cs.cmu.edu/~scandal/papers/treaps-spaa98.pdf)

- ### 线性规划（Linear Programming）（视频）
    - [线性规划](https://www.youtube.com/watch?v=M4K6HYLHREQ)
    - [寻找最小成本](https://www.youtube.com/watch?v=2ACJ9ewUC6U)
    - [寻找最大值](https://www.youtube.com/watch?v=8AA_81xI3ik)
    - [用 Python 解决线性方程式──单纯形算法](https://www.youtube.com/watch?v=44pAWI7v5Zk)

- ### 几何：凸包（Geometry, Convex hull）（视频）
    - [Graph Alg. IV: 几何算法介绍 - 第 9 课](https://youtu.be/XIAQRlNkJAw?list=PLFDnELG9dpVxQCxuD-9BSy2E7BWY3t5Sm&t=3164)
    - [Graham & Jarvis: 几何算法 - 第 10 课](https://www.youtube.com/watch?v=J5aJEcOr6Eo&index=10&list=PLFDnELG9dpVxQCxuD-9BSy2E7BWY3t5Sm)
    - [分而治之: 凸包, 中值查找](https://www.youtube.com/watch?v=EzeYI7p9MjU&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp&index=2)

- ### 离散数学
    - [计算机科学70，001 - 2015年春季 - 离散数学与概率论](http://www.infocobuild.com/education/audio-video-courses/computer-science/cs70-spring2015-berkeley.html)
    - [离散数学由Shai Simonson（19个视频）](https://www.youtube.com/playlist?list=PLWX710qNZo_sNlSWRMVIh6kfTjolNaZ8t)
    - [离散数学由印度理工学院罗帕尔分校NPTEL提供](https://nptel.ac.in/courses/106/106/106106183/)

---

## 一些主题的额外内容

- **SOLID**
    - [ ] [Bob Martin SOLID Principles of Object Oriented and Agile Design (视频)](https://www.youtube.com/watch?v=TMuno5RZNeE)
    - [ ] S - [单一职责原则 | 每个对象负责一个单一职责](http://www.oodesign.com/single-responsibility-principle.html) | [Single responsibility to each Object](http://www.javacodegeeks.com/2011/11/solid-single-responsibility-principle.html)
        - [更多解释](https://docs.google.com/open?id=0ByOwmqah_nuGNHEtcU5OekdDMkk)
    - [ ] O - [开闭原则](http://www.oodesign.com/open-close-principle.html)  | [在生产级别上，对象应准备好进行扩展，但不进行修改](https://en.wikipedia.org/wiki/Open/closed_principle)
        - [更多解释](http://docs.google.com/a/cleancoder.com/viewer?a=v&pid=explorer&chrome=true&srcid=0BwhCYaYDn8EgN2M5MTkwM2EtNWFkZC00ZTI3LWFjZTUtNTFhZGZiYmUzODc1&hl=en)
    - [ ] L - [里氏替换原则](http://www.oodesign.com/liskov-s-substitution-principle.html) | [基类和派生类遵循‘是一个’原则](http://stackoverflow.com/questions/56860/what-is-the-liskov-substitution-principle)
        - [更多解释](http://docs.google.com/a/cleancoder.com/viewer?a=v&pid=explorer&chrome=true&srcid=0BwhCYaYDn8EgNzAzZjA5ZmItNjU3NS00MzQ5LTkwYjMtMDJhNDU5ZTM0MTlh&hl=en)
    - [ ] I - [接口隔离原则](http://www.oodesign.com/interface-segregation-principle.html) | 客户端不应被强制实现不使用的接口
        - [5分钟内的接口隔离原则（视频）](https://www.youtube.com/watch?v=3CtAfl7aXAQ)
        - [更多解释](http://docs.google.com/a/cleancoder.com/viewer?a=v&pid=explorer&chrome=true&srcid=0BwhCYaYDn8EgOTViYjJhYzMtMzYxMC00MzFjLWJjMzYtOGJiMDc5N2JkYmJi&hl=en)
    - [ ] D -[依赖反转原则](http://www.oodesign.com/dependency-inversion-principle.html) | 在对象的组合中减少依赖
        - [为何依赖反转原则如此重要](http://stackoverflow.com/questions/62539/what-is-the-dependency-inversion-principle-and-why-is-it-important)
        - [更多解释](http://docs.google.com/a/cleancoder.com/viewer?a=v&pid=explorer&chrome=true&srcid=0BwhCYaYDn8EgMjdlMWIzNGUtZTQ0NC00ZjQ5LTkwYzQtZjRhMDRlNTQ3ZGMz&hl=en)


- **Union-Find**
    - [概览](https://www.coursera.org/learn/data-structures/lecture/JssSY/overview)
    - [初级实践](https://www.coursera.org/learn/data-structures/lecture/EM5D0/naive-implementations)
    - [树状结构](https://www.coursera.org/learn/data-structures/lecture/Mxu0w/trees)
    - [合并树状结构](https://www.coursera.org/learn/data-structures/lecture/qb4c2/union-by-rank)
    - [路径压缩](https://www.coursera.org/learn/data-structures/lecture/Q9CVI/path-compression)
    - [分析选项](https://www.coursera.org/learn/data-structures/lecture/GQQLN/analysis-optional)

- **动态规划的更多内容** (视频)
    - [6.006: 动态规划 I: 斐波那契数列, 最短路径](https://www.youtube.com/watch?v=OQ5jsbhAv_M&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb&index=19)
    - [6.006: 动态规划 II: 文本匹配, 二十一点/黑杰克](https://www.youtube.com/watch?v=ENyox7kNKeY&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb&index=20)
    - [6.006: 动态规划 III: 最优加括号方式, 最小编辑距离, 背包问题](https://www.youtube.com/watch?v=ocZMDMZwhCY&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb&index=21)
    - [6.006: 动态规划 IV: 吉他指法，拓扑，超级马里奥.](https://www.youtube.com/watch?v=tp4_UXaVyx8&index=22&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb)
    - [6.046: 动态规划: 动态规划进阶](https://www.youtube.com/watch?v=Tw1k46ywN6E&index=14&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp)
    - [6.046: 动态规划: 所有点对最短路径](https://www.youtube.com/watch?v=NzgFUwOaoIw&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp&index=15)
    - [6.046: 动态规划: 更多示例](https://www.youtube.com/watch?v=krZI60lKPek&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp&index=12)

- **图形处理进阶** (视频)
    - [异步分布式算法: 对称性破缺，最小生成树](https://www.youtube.com/watch?v=mUBmcbbJNf4&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp&index=27)
    - [异步分布式算法: 最小生成树](https://www.youtube.com/watch?v=kQ-UQAzcnzA&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp&index=28)

- **字符串匹配**
    - Rabin-Karp（视频）
        - [Rabin Karps 算法](https://www.coursera.org/learn/data-structures/lecture/c0Qkw/rabin-karps-algorithm)
        - [预计算](https://www.coursera.org/learn/data-structures/lecture/nYrc8/optimization-precomputation)
        - [优化：实施和分析](https://www.coursera.org/learn/data-structures/lecture/h4ZLc/optimization-implementation-and-analysis)
        - [表翻倍，Karp-Rabin](https://www.youtube.com/watch?v=BRO7mVIFt08&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb&index=9)
        - [滚动哈希，摊销分析](https://www.youtube.com/watch?v=w6nuXg0BISo&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb&index=32)
    - Knuth-Morris-Pratt (KMP)：
        - [Knuth-Morris-Pratt（KMP）字符串匹配算法](https://www.youtube.com/watch?v=5i7oKodCRJo)
    - Boyer–Moore 字符串搜索算法
        - [Boyer–Moore 字符串搜索算法](https://en.wikipedia.org/wiki/Boyer%E2%80%93Moore_string_search_algorithm)
        - [高级字符串搜索Boyer-Moore-Horspool算法（视频）](https://www.youtube.com/watch?v=QDZpzctPf10)
    - [Coursera：字符串算法](https://www.coursera.org/learn/algorithms-on-strings/home/week/1)
        - 刚开始时很棒，但是当它超过 KMP 时，它变得比需要复杂得多
        - 很好的字典树解释
        - 可以跳过

- NAND 到 Tetris: [从第一原理构建现代计算机](https://www.coursera.org/learn/build-a-computer)

## 论文

- [喜欢经典的论文？](https://www.cs.cmu.edu/~crary/819-f09/)
- [1978: 通信顺序处理](http://spinroot.com/courses/summer/Papers/hoare_1978.pdf)
    - [Go 实现](https://godoc.org/github.com/thomas11/csp)
- [2003: The Google 文件系统](http://static.googleusercontent.com/media/research.google.com/en//archive/gfs-sosp2003.pdf)
    - 2012 年被 Colossus 取代了
- [2004: MapReduce: Simplified Data Processing on Large Clusters](http://static.googleusercontent.com/media/research.google.com/en//archive/mapreduce-osdi04.pdf)
    - 大多被云数据流取代了?
- [2006年：Bigtable：结构化数据的分布式存储系统](https://static.googleusercontent.com/media/research.google.com/en//archive/bigtable-osdi06.pdf)
- [2006年：针对松散耦合的分布式系统的Chubby Lock服务](https://research.google.com/archive/chubby-osdi06.pdf)
- [2007年：Dynamo：亚马逊的高可用键值存储](http://s3.amazonaws.com/AllThingsDistributed/sosp/amazon-dynamo-sosp2007.pdf)
    - Dynamo论文启动了NoSQL革命
- [2007: 每个程序员都应该知道的内存知识 (非常长，作者建议跳过某些章节来阅读)](https://www.akkadia.org/drepper/cpumemory.pdf)
- 2012: AddressSanitizer: 快速的内存访问检查器:
    - [论文](http://static.googleusercontent.com/media/research.google.com/en//pubs/archive/37752.pdf)
    - [视频](https://www.usenix.org/conference/atc12/technical-sessions/presentation/serebryany)
- 2013: Spanner: Google 的分布式数据库:
    - [论文](http://static.googleusercontent.com/media/research.google.com/en//archive/spanner-osdi2012.pdf)
    - [视频](https://www.usenix.org/node/170855)
- [2015: Google的持续流水线](http://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43790.pdf)
- [2015: 大规模高可用性：构建Google广告数据基础设施](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44686.pdf)
- [2015: 开发人员如何搜索代码：一个案例研究](http://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43835.pdf)
- 更多论文： [1,000篇论文](https://github.com/0voice/computer_expert_paper)

