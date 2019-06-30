```
curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.sh #下载miniconda3
bash Miniconda3-latest-MacOSX-x86_64.sh #安装miniconda3
source /Users/shenkefeng/.bash_profile 或者 source ~/.bash_profile #更新环境变量（说明书source ~/.bashrc无效, Linux 里面是 .bashrc 而 Mac 是 .bash_profile）
conda -h #验证是否安装成功
conda upgrade conda #升级conda
conda list #查看已安装的软件列表
conda-env list #查看env列表
conda create -n biosoft python=2.7 #创建env
conda activate biosoft  #切换env
conda config --get channels #查看镜像源，发现为空
#逐一添加镜像源，后加入的优先级高
conda config --add channels conda-forge　　　
conda config --add channels defaults　　　
conda config --add channels r　　　
conda config --add channels bioconda
conda config --set show_channel_urls yes
vi ~/.condarc #也可vim编辑器写入镜像源：wq!保存退出
conda config --add channels conda-forge　　　
conda config --add channels defaults　　　
conda config --add channels r　　　
conda config --add channels bioconda
conda config --set show_channel_urls yes
```

