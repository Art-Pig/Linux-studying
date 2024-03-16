# Linux-studying
I will share my studying of linux.
 
  我目前是大专二年级，专业是电子信息工程技术，众所周知，这个专业学得特别的杂，万金油专业，学校啥都教，这样就无法什么都学得好。学得再多总不如学得精，我原本打算插本，但一转念想，升学的目的不还是为了找工作，况且我现在的学校在一线城市而且口碑还是不错的，而我插本能选择的学校在四线城市，那么城市间所能提供的就业机会就不可同日而语了。思前想后，我决定了我想要的职业——嵌入式软件开发。为什么想要从事这门行业呢?原因是我真的学不懂硬件，硬件的学习资源，学习条件要比软件要求的苛刻的多，要有实际工具来操作。而软件开发则一台电脑便绰绰有余，况且软件学习的线上资源远比硬件学习资源要多得多。如今按我现在的学习进程要与企业要求的学习技能相匹配的话，我则需要学好Linux、ARM、stm32与数据结构，但当我今天学习Linux时，我便遇到了一个非常棘手的问题。我在Centos终端面板中输入“ifconfig”，但是却没有找到IP地址，导致我无法连接上FinalShell。在昨天，我的FianlSehll还能连上我的Linux，但是今天却怎么也连不上了，在网上找了下解决方法，发现我的公用网络防火墙没关，但是还是不行。之后按B站弹幕里的方法输入“ip addr”也不行，之后用看到可以输入“sudo ........”还是不行，因为我未将我的用户加入什么管理文件，学到这里，我觉得我还是先不要盲目自学了，先暂停一会儿，到油管看看老外是怎样讲Linux的吧。
  


差不多拉到这里，可以看到Linux的目录
GitHub里的网址:https://github.com/m3y54m/Embedded-Engineering-Roadmap






介绍Linux	嵌入式操作系统	油管视频
		
网址:Introduction to Embedded Linux Part 1 - Buildroot | Digi-Key Electronics

![image](https://github.com/Art-Pig/Linux-studying/assets/121549293/367394f7-e711-4057-8932-91c9a6dfd474)
嵌入式Linux让你可以操作驱动，但是如果说要自己写出程序来会非常复杂，应该要学会使用工具软件。演示了Linux如何在stm32上运行

介绍了Yocto这个免费的软件，能专门为你的嵌入式驱动做Linux操作（自行定制化)

YouTube 上有官方出品的stm32教程
它的视频看不懂，需要一些基础。
一块电路板中有许多的元件，而Linux的作用就是为这些元件加上驱动
![image](https://github.com/Art-Pig/Linux-studying/assets/121549293/c13742f1-6867-4bfc-816b-81e969f4ba0e)

我还是没有解决昨天的FinalShell网络连接问题，但是想着不能停下练习Linux终端命令操作的脚步，就直接用CentOS里的终端吧。还好边看书籍《Linux命令行大全》，总算练得还不错，不过我觉得这本书没必要全跟着它一起一个一个打，练完。应该把它当成字典工具用来查就好了，嗯，我今天还上油管看了Linux与嵌入式的介绍，博主演示了Linux如何在电子板上跑的过程，博主在上面敲代码，我看不太懂，还是得有点基础再去看。Linux不止命令行什么的，还有内存管理，数据结构什么的，这些都要学。把这些概念看的差不多了，再准备拿个板子直接开始跑Linux吧。UP主Frank的C语言新版课程好像快更新完了，有时间得去看看跟老版的差异（老版的被他删了）。

Micro_Frank 《步入Linux的现代方法》
GUI与GUN的区别，GUI是图形界面，GUN是命令；Linux是内核
Linux内核；
1.硬件设备 管理使用
2.软件程序 （系统） 操作管理
3.系统内存
4.文件管理 、保存文件，对文件的操作
文件系统：读、写的标准
win常用NTFS文件系统
Linux常用ext标准
Ubuntu与centOS的区别，目前来看前者要比后者UI设计好看多了，而且动画更加流畅。
安装什么的，软件安装多了自然就知道怎么安装了。
目前已经看到了第三章中间，怎么讲了这是Frank21年的课，而我在看这个前已经先学了几天的Linux，命令也都大概跑了一遍，但是对于环境与父子shell有一点模糊，外加上单单只有一本书没有过多的强化训练，想来看看frank的课程有没有我想要的知识点与强化训练。不过前几章frank也是理论偏多，我也挺喜欢他以讲故事的方式来讲理论。
我个人在看书的时候也觉得单单按书敲一遍命令是没啥用的，还是要有点小项目来训练，因为我打算走嵌入式反相，那么这个内存管理、与工作环境便显得格外重要，frank讲的话也应证了我先前的观点。
![image](https://github.com/Art-Pig/Linux-studying/assets/121549293/bbc1befd-551a-4608-8a25-1cf8bb334d98)

第二天学习：
GUI（图形界面）
Unity用于Ubuntu
GUI:
1.X windows
2.KDE
3.GNOME
4.unity

Linux/GUN:Linux内核，GUN命令（shell）；

Linux发行版：
Ubuntu、CentOS、Red Hat

shell 命令：
写命令时要注意空格
~波浪线表示当前所在命令，当前用户/home目录
$表示等待用户输入
bash 手册，man命令可以查询用处，但是都是英文；可以用这个网站“wangchujiang.com”，这是一个免费的在线命令查找网站

Linux根目录
Linux一切皆文件
注意：Linux的文件不要乱删，可能会使系统崩溃
cd:切换目录
“\”正斜线，Windows
/反斜线是Linux
/$代表根目录
Linux没有盘符的概念（无C、D盘）

Linux根目录解析：

/bin 二进制目录GNC工具，ls等自带的命令

/cdrom

/etc 系统配制文件目录

/home 主目录，显示所有用户目录

/lib 库目录

/lost + found

/mnt 挂载目录，U盘挂载--外在的设备和电脑进行连接

/proc 伪文件系统

/run 运行目录

/snap 

/temp 临时目录

/var 可变目录 .log

/dev 设备目录，驱动程序

/media 媒体目录

/opt 可选目录

/root root用户的主目录管理员


/sbin 系统二进制目录，GNU/高级管理员使用的命令工具

/src 服务目录本地服务


FHS 文件系统层级标准

CD命令：

cd切换目录

cd 默认回到home

cd /dirtory 到指定目录

cd .当前目录

cd ..上一个目录

Linux复制 Crtl+Shift+C

Linux撤回不行

文件目录：

1.绝对路径（全）

太阳系地球亚洲中国广东省深圳市南山区沙河西路西丽街道深圳职业技术大学东区快递驿站

2.相对路径（不全）

*一定要设置故事背景

相对谁？

相对于快递员只负责西丽街道：派送快递员，只负责一个小区域，那就只看深圳职业技术大学东区快递驿站

Linux上的路径

前面有/，就会被系统认为绝对路径

写相对路径时，在上一条路径前，末尾要加/，或者.+相对路径（.点是前文件目录）

如何练习非常重要

文件扩展匹配符

？，*

ls -l frank*,*能代替多个字符

ls -l frank?,?只能代替一个字符

ls -l frank[a-x],带有a-x的范围，当然还可以相反[!a-x]

touch 创建文件

cp 可以复制文件 文件夹

cp 你想复制的文件？ 你想复制到哪？

cp 源文件 目标文件


cp 文件 目录

cp -r 目录 目录

Tab 制表符 自动补全，快速写入

键盘快捷键 移动光标

lnk链接文件，类似于win里的快捷方式

链接文件 

1.符号链接 （软链接）——快捷方式

2.硬链接

软链接 ln -s 源文件 快捷方式

硬链接 ln 源文件 快捷方式 （前提是要在同一块盘里 ）

副本

原来的文件/文件夹 必须是存在的

符号链接（软链接）

Symbolic links

soft links

Linux

mv 重命名

!$ 执行上一条目录最后一条           

rm (removing删除) 最危险的命令，删库跑路  

注意注意，删东西前，一定要加-i询问

 太可怕了。这条命令太恐怖了，所以公司一定要备份，个人最好不要用管理员身份；

 删库跑路：“sudo mv -i -rf /*”

 sudo 临时管理员身份

 mv 删除

 -i 询问

 -rf 遍历文件

 /* 根目录里的所有文件

 删库跑路是犯法的，会被判刑的

 目录（文件夹）

 mkdir (make directories) 创建文件

cat 可以直接在终端上打开文件，在终端里显示（适用于内容比较小的地方）

cat -n 每一行带上符号

more 以全屏展示，可以翻页，翻页字母B上一页，空格下一页，Q是退出

less cat more 是打开文本文件的三大命令

hed n -2 demo.c 打开前两行

tail n -2 demo.c 打开后两行

Bash shell

Linux 任务管理器 System Monitor

使用命令形式查看 top

ps (process atatus 进程状态) 

ps -aux | grep named # 查看named进程详细信息

kill 中断进程

挂载：

插上了U盘，电脑上出现，于是电脑创建了一个临时的盘供用户使用，电脑一关机就没了

mnt 放自动挂载的文件目录

mount 挂载到另一个目录上

umount 卸载

为什么要有挂载

df 可以看到挂载目录

以前的系统要自己挂载

安卓挂载，开发者选项

du -h 能看目录和文件大小

sort -r 文件内容按倒序排序

sort -m 按月份排序

实例
将 /home/vivek/bin/ 目录打包，并使用 gzip 算法压缩。保存为 /tmp/bin-backup.tar.gz 文件。

tar -zcvf /tmp/bin-backup.tar.gz /home/vivek/bin/  (解压是-zxvf，注意查文件格式，命令自己去网上找)

- z：有gzip属性的
- 
- j：有bz2属性的
- 
- Z：有compress属性的
- 
- v：显示所有过程
- 
- O：将文件解开到标准输出
- 
tar -cf archive.tar foo bar  # 从文件 foo 和 bar 创建归档文件 archive.tar。

tar -tvf archive.tar         # 详细列举归档文件 archive.tar 中的所有文件。

tar -xf archive.tar          # 展开归档文件 archive.tar 中的所有文件。

下面的参数-f是必须的

-f: 使用档案名字，切记，这个参数是最后一个参数，后面只能接档案名。

父子shell的概念：

bash 本质是一个终端

bash 下又用一次bash

父bash 和 子bash

PID 子，PPID 父

exit 退出最新的bash

ps -- forest 可以看到父子shell的叠层关系

;分号的作用

ls;pwd;cd 这样子可以依次执行

sleep 10,让终端倒计时10秒（休眠）

sleeo 10&,&是放在后台10s

jobs ,看后台工作，jobs -l 能看到PID

挂在后台coproc

history 查看历史命令

Linux环境变量

printenv 环境变量

全局变量 大写，单词间下划线隔开

局部变量小写，单词间下划线隔开

PATH

包管理系统 PMS

软件安装，更新，卸载 

工具依赖

dpkg (ubuntu Debian)        

用户与权限

id 身份证

用户 id UID 数字

系统账户 : 数字（<500）

密码被隐藏，用X表示

作业：自学chmod

编辑器之神VIM

vi nano emacs vim

学习vim

安装vim

sudo apt install vim

vim的使用

编辑模式 i键（insert，插入模式）

普通模式 ESC

保存 ，退出 ：wq (write 写入，quit 退出)

i 光标位置的前面插入

a光标位置后面插入

o直接enter到下一行插入

x 删除光标所在字符

dd 删除整一行

u 撤销

dw 移除当前所在光标往后的单词

b 跳跃单词首字母

e 跳跃单词最后

w 跳跃单词下一个单词的首字母

shift 联合操作

复制文本则要稍微复杂点。vim中复制命令是y（代表yank）。可以在y后面使用和d命令相同的第二字符（yw表示复制一个单词，y$表示复制到行尾）。在复制文本后，把光标移动到你想放置文本的地方，输入p命令。复制的文本就会出现在该位置。 

/ 查找

替换命令的格式是： :s/old/new/

vim编辑器会跳到old第一次出现的地方，并用new来替换。可以对替换命令作一些修改来替换多处文本。 

 :s/old/new/g：一行命令替换所有old。 

 :n,ms/old/new/g：替换行号n和m之间所有old。 

 :%s/old/new/g：替换整个文件中的所有old。 

 :%s/old/new/gc：替换整个文件中的所有old，但在每次出现时提示。 

可视化模式 选择文本

v ——》 hjkl 操作选择

y p

V 行

gg(删除一行) v G（删除全部）

V 跳跃命令（继续用O和hJKL）

0 补全

vaw 快速选择单词

vab 包含括号

vaB 包括大括号

va> 包括中括号 删除

v+shift+<> 代码缩进(往前/往后)

~ 反，小写——》大写，大-》小
v shift+~

v+u  全部转换成小写

v+U 全部转换成大写

vim 基础配置

设置高亮

设置行号

设置tab 

字符编码

number+gg 跳行号

成为大佬——》用最简单的工具写代码（没有提示，vim）
