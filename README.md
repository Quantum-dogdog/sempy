# sempy
a Python Open-Source Toolbox for Non-Keplerian Astrodynamics, Used for Mission Analysis in the Sun-Earth-Moon System forked from "gitlab.isae-supaero.fr/sempy"


#

我把源码上传到release栏目下了，大家可以去那里下载。


# 保姆级配置教程

原网页 gitlab.isae-supaero.fr/sempy 上的配置教程not work,我摸索出的成功的保姆级配置方法写在下面：

1.将下载的 sempy-user-master.zip 解压到你喜欢的 E:/ 盘

2.打开 miniforge prompt 或者 anaconda prompt ,在命令提示符后面输入 conda create -name xiaoheiwu python==3.8.5     (xiaoheiwu是你的虚拟环境的名字-小黑屋)

3.环境创建成功后，输入 conda activate xiaoheiwu

4.然后在命令提示符后面输入 E: 跳转到E盘，然后输入 cd sempy-user-master/sempy_core ,打开 requirements.txt 删除其中的pykep、pygmo、python这三行，点击保存

5.然后依次在命令提示符后输入 conda install pygmo==2.16.1   、   conda install pykep==2.6

6.然后输入 conda install --file requirements.txt

7.然后输入 python setup.py install ,这样就安装成功了，大部分的例子都能完美运行，个别例子有bug,可能作者好久没维护了
