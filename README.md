# Git的基本操作
<a href = "https://www.bilibili.com/video/BV1Cr4y1J7iQ/?spm_id_from=333.788&vd_source=be66e6ef1fad40de68ba8ca5b7b14465"> 这是git入门教学 </a>   


## 一.基本操作
* 克隆clone
* 创建(初始化)工作区, 理解暂存区(index/stage)
* 连接git
* 上传/提交(commit)及修改文件
* checkout命令恢复code


<br/>

## 1.git克隆: git clone + 网址

<br/>

## 2. 工作区和暂存区
暂存区可以理解为一个抽象的文件夹. 它的具体实现则在.git文件夹里. 工作区和(仓库)数据库之间通常不是直接连接的, 是通过这个暂存区提交给数据库</br>
暂存区: 看下面的内容: 准备提交的状态, 也就是把文件放入暂存区(index/stage)
工作区 -> 暂存区: add <br/>
暂存区 -> 仓库: commit
<br/>
<br/>

## 3.初始化 init

在指定文件夹(初始化本地工作区)下面用git init指令进行初始化.
这个文件夹下的大的目录叫做工作区<br/>


## 4. 提交commit<br/>
1   git add .  <u> 所有文件和非空文件夹设置成准备提交的状态<br/></u>
然后 git commit -m " "  引号里的内容是对这次提交的备注 <br/>
可以用git log来查看提交记录, 包括作者,时间以及备注<br/>
git log之后, commit 后面跟的7f30f79dc072..... 这个可以理解为身份证号,用来唯一标识每一次提交 <br/>
2   git add + 名字，此时设置成准备状态  <u>可以单独提交文件</u>， 然后 git commit -m " "  引号里的内容是对这次提交的备注 <br/>

<br/>

## 5. checkout命令恢复<br/>
git checkout HEAD + 文件名(e.g. main.py)<br/>
这个指令是从最后一次的提交里, 将这个文件复制到工作区(覆盖)

</br>

* * *
* * *

# git常用指令
* ls:   查看当前所在文件夹下的所有内容. （蓝色代表目录， 绿色代表程序， 白色代表文件）
* cd:   改变目录
* cd .. :返回上一级目录（..前要加空格）
* pwd:  显示当前所在的目录路径
* mkdir：新建一个目录， 就是新建一个文件夹 e.g. mkdir test （在这个当前目录下 创建了test文件夹）
* touch：新建一个文件，如touch index.js 就会在当前目录下新建一个index.js 文件
* rm： 删除一个文件 e.g. rm index.js 就会把index.js文件删除 （不能删除文件夹directory）
* rm -r: 删除一个文件夹，rm -r test 删除test目录
* clear: 清屏
* reset： 重新初始化终端/清屏
* ! ！ rm -rf/ 切勿轻易使用， 会删除电脑中全部文件！包括系统
* mv：移动当前目录下 某个文件到某个文件夹中（都在这个大的目录下）
* history： 查看命令历史
* help：帮助
* exit: 退出