CS61A (SICP Python版) 自学通关全指南

- 该份指南作为后续学习的“操作手册”

-----

## 🎓 UC Berkeley CS61A (SICP Python版) 自学通关全指南

### 一、 课程基准与环境设定

  * **黄金版本**：**Fall 2020**。该学期为全线上授课，视频专为屏幕前的自学者重新录制、剪辑，画质、音质和代码演示极其清晰。
  * **进度总控枢纽**：绝对不要在 YouTube 里盲目列表循环。一切进度以课程归档主页的 **Schedule（课表）** 为唯一准绳。
      * **主页地址**：[cs61a.org/archive/fa20/](https://www.google.com/search?q=https://cs61a.org/archive/fa20/)
  * **官方配套神书**：[*Composing Programs*](http://composingprograms.com/)。John DeNero 教授亲自编写的 Python 版 SICP，完美贴合视频进度。

### 二、 标准学习工作流 (闭环)

请严格按照以下顺序循环推进，从 **Lecture 1** 一直攻克到 **Lecture 37**：

1.  **查阅课表**：进入主页 Schedule，锁定当周/当天的学习任务。
2.  **看视频 (Lecture)**：点击课表上的 Lecture 链接，系统会自动按正确逻辑播放 YouTube 上的知识点切片。
3.  **看书辅助 (Reading)**：配合阅读 *Composing Programs* 对应的章节。视频里一闪而过的代码细节，书里都有极其详尽的拆解。
4.  **实战敲代码 (Lab / HW / Project)**：这是本课程的核心。绝不能只看不练，必须完成课表上对应的每一次上机实验、课后作业和阶段性大型项目。

### 三、 自学者“通关秘籍”：绕过校园登录与本地测试

作为非伯克利在校生，你必然会遇到 `UCB CalNet Authentication Service` 的拦截。请严格按照以下步骤操作以实现完美“白嫖”：

  * **避开“雷区”链接**：课表上的 `Webcast`, `Ed`, `Piazza`, `Submit`, `Grades` 等链接是校内生专属，**绝对不要点击**。
  * **获取作业代码**：
    1.  在课表上直接点击作业的名字（如 `Lab 1`、`HW 01` 或 `Project 1: Hog`）。
    2.  进入纯英文的说明文档页面。
    3.  在页面最顶端寻找类似 *“You can download all of the files you need in a zip archive.”* 的提示。
    4.  点击下载 `.zip` 压缩包，解压到你的本地学习目录中。
  * **本地 Autograder 测试 (核心魔法)**：
    进入终端 (Terminal/命令行)，切换到你解压好的作业文件夹。使用官方提供的 `ok` 脚本测试代码时，**必须加上 `--local` 参数**，这会阻断程序连接伯克利服务器，直接在本地输出跑分结果。
      * **测试特定题目**（最常用）：`python3 ok -q [题目名称] --local`
      * **测试全部题目**：`python3 ok --local`

### 四、 精力分配与核心攻坚战略

Python 前期的变量赋值、基本控制流会显得十分直白，这部分视频完全可以**开启倍速**快速扫过。

请将 **120% 的脑力** 集中轰炸以下四个深水区：

1.  **Environment Diagrams (环境图)**：这是 CS61A 最强悍的思维训练。学会在纸上画出函数调用栈、帧 (Frames) 和变量绑定的完整生命周期，建立对内存状态的绝对直觉。
2.  **Higher-Order Functions & Recursion (高阶函数与递归)**：打破传统的命令式思维，理解“函数本身也可以作为数据传递”，这是走向函数式编程思维的分水岭。
3.  **Object-Oriented Programming (面向对象)**：深入剖析 Python 这种动态语言下的类、对象和继承机制，体会其与静态语言 OOP 的微妙差异。
4.  **最终封神之战：Scheme Interpreter (Project 4)**：在课程末尾，你将用 Python 从零手写一个 Lisp 方言 (Scheme) 的解释器。完成这个大作业，通关 CS61A
