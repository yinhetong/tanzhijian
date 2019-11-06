1.使用github的目的

　　借助github托管代码

2.需要掌握的基本概念

　　a.仓库（Repository）

　　　　仓库指的是你的一个开源项目，

　　b.收藏（star）

　　　　仓库主页的star按钮，意思为收藏项目的人数，在Github上若果你有一个100的star项目

　　　　就很不容易了

　　c. 复制克隆项目（fork）

　　　　将他人的仓库，copy成一个自己的仓库(该仓库是独立存在)

　　d.发起请求（pull request）

　　　　把自己copy的仓库做了更改后，通过pull request发给原作者，如果原作者同意，并　　　              原仓库

　　e.关注（Watch）

　　　　当你关注了某个项目，该项目有任何更新，你会接到提醒，关注人，你会看到他的动态

　　f. 事物卡片（issue）

　　　　发现代码bug,但是目前没有被解决，讨论时使用；

　　　　情景：当我们浏览他人的项目的时候，可以通过创建一个Issue向作者发起一个讨论

　　　　　　　作者在登陆后发现Issue之后，反馈

　　Github主页，仓库主页，个人主页

　　　　a.GitHub主页

　　　　b.仓库主页

　　　　　创建文件

　　　　　　 Commit directly to the master branch.

　　　　　　 Create a new branch for this commit and start a pull request. 

　　　　　 修改文件，删除文件

　　　　　上传文件

　　　　　查找文件

Git的安装和使用

　　目的：通过Git在本地管理远程仓库github的项目代码

　　1.下载安装

　  2.Git的基本工作流程

　　　　工作区（Working Directory）：添加，编辑，修改文件等

　　　　暂存区：暂存已经修改的文件最后统一提交的git仓库中

　　　　Git  Repository(Git 仓库):最终确定的文件保存到仓库，成为一个新的版本，并且可见

　　3.Git的初始化仓库和操作

　　　　a.基本信息配置git config --list查看信息

　　　　　　1.设置用户名　　　

　　　　　　　　git config --global user.name ‘coldBreeze‘

　　　　　　2.设置用户名邮箱

　　　　　　　　git config --global user.email ‘804421392@qq.com‘

　　　　b.初始化一个新的Git仓库

　　　　　　创建目录：mkdir test 　　进入目录：cd test　　

　　　　　　初始化为Git目录：git init,形成.git文件（默认是隐藏的）

　　4.向仓库中添加文件

　　　　1.创建文件  touch a.java                查看状态（git stutas）

　　　　2.将文件添加到暂存区  git add a.java     查看状态（git stutas）

　　　　3.将暂存区的文件添加到仓库 git commit -m ‘add a.java‘     查看状态（git stutas）

　　5.修改仓库文件

　　　　1.进入vim编辑模式 vi a.java（退出vim的方法：一直按住esc ，再连续按大写的z两次就退出来了）

　　　　2.查看文件内容  cat a.java     查看状态（git stutas）　　　

　　　　3.将文件添加到暂存区  git add a.java     查看状态（git stutas）

　　　　4.将暂存区的文件添加到仓库 git commit -m ‘第一次通过git修改‘     查看状态（git stutas）

　　6.删除仓库文件　

　　　　1.删除工作区文件 rm -rf　a.java　　

　　　　2.删除暂存区文件 git rm a.java

　　　　3.提交操作 git commit -m ‘第一次通过git删除‘

　　7. Git管理远程仓库

　　　使用远程的目的：备份，实现代码的共享和集中化管理

　　       a.Git克隆操作（git clone 项目地址[例：git@github.com:coldBreeze/Snake.git]）--需要等待

　　　　　　目的：将远程仓库的项目复制到本地

　　　　b.创建文件 vi b.txt

　　　　c.添加到暂存区

　　　　d.添加到本地仓库

　　　　e.同步到远程仓库  git pull

　　8.Github pages搭建个人网站

　　　　a.访问：https://用户名.github.io

　　　　　b.搭建步骤：　

　　　　　　1)创建个人站点---->新建仓库（注：仓库名必须是.github.io）

　　　　　　2)在仓库下中创建index.html作为网站首页

　　9.Project Pages 项目站点

　　　　访问：https://用户名.github.io/仓库名

　　　　搭建步骤：

　　　　　　1）进入项目主页，点击settings

　　　　　　2)在GIthub Pages中复制站点https://coldbreeze.github.io/Snake/

　　　　　　3）选择主题