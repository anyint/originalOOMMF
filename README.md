# originalOOMMF
original edition copy from http://math.nist.gov/oommf/


###简单介绍OOMMF在linux中的安装
#### 环境配置
1. 下载软件包
http://math.nist.gov/oommf/dist/oommf12a5bis_20120928.tar.gz
                依赖的库
2. 设置 tcl/tk的环境变量,
下载安装 ActiveTcltk
http://downloads.activestate.com/ActiveTcl/releases/
在.bashrc文件中写入Active 路径
并source生效

3. 检查系统环境
```bsh
cd .../path/to/oommf
```

 进入解压后的文件夹 运行

```sh
 tclsh  oommf.tcl +platform
```
会显示检查 的 如下面类似系统信息  
```zsh
Platform Name:		linux-x86_64
Tcl name for OS:	Linux 3.10.0-123.20.1.el7.x86_64
C++ compiler:   	/usr/bin/g++ 
 Version string:	 g++ (GCC) 4.8.2 20140120 (Red Hat 4.8.2-16)
Shell details ---
 tclsh (running): 	/opt/ActiveTcl-8.6/bin/tclsh
                  	 --> Version 8.6.3, 64 bit, threaded
 tclsh (OOMMF): 	/opt/ActiveTcl-8.6/bin/tclsh8.6
                  	 --> Version 8.6.3, 64 bit, threaded
 filtersh:           	/home/admint/oommftcl64/app/omfsh/linux-x86_64/filtersh
                  	 --> Version 8.6.3, 64 bit, threaded
 tclConfig.sh:        	/opt/ActiveTcl-8.6/lib/tcl8.6/tclConfig.sh
                      	 --> Version 8.6.3
 wish (OOMMF):        	/opt/ActiveTcl-8.6/bin/wish8.6
                  	 --> Version 8.6.3, Tk 8.6.3, 64 bit, threaded
 tkConfig.sh:         	/opt/ActiveTcl-8.6/lib/tkConfig.sh
                      	 --> Tk Version 8.6.3
OOMMF threads:         	Yes
  Default thread count:	  4
  NUMA support:        	  No
OOMMF API index:       	20120928
Temp file directory: 	/tmp
```
如有缺少组件，如 C++   tcl tk 必须补充

#### 编译安装
```css
tclsh oommf.tcl pimake
```

#### 基本运行，进入所在文件夹
```css
tclsh oommf.tcl
```
