# NetEaseMusicDownloader

[README.md](https://github.com/Kito0615/NetEaseMusicDownloader/blob/master/README.md)

![](https://img.shields.io/badge/Platform-Python3-009eff.svg) ![](https://img.shields.io/badge/Windows-支持-00efff.svg)  ![](https://img.shields.io/badge/MacOS-支持-00efff.svg) ![](https://img.shields.io/badge/Linux-支持-00efff.svg) ![](https://img.shields.io/badge/WebAPI-可用-00efff.svg)

> **注意:** 这个脚本使用了[AD&#39;s API](https://api.imjad.cn/) 提供的接口，在此表示感谢. 这个脚本仅供个人学习交流使用，不能用于任何商业用途，所有法律问题均与作者无关。
>
> **注意**: **由于三方库已经失效，现在这个项目已经不再那么有用. 如果你想使用这个项目, 可以参考这个[NetEaseCloudMusicApi](https://github.com/Binaryify/NeteaseCloudMusicApi) 项目，并修改本项目中的API链接即可.**

#### 更新：2024-12-23

1. 增加播放列表缓存，以缓解官方服务器压力
2. 修复了播放列表及MV无法下载的问题
3. 修复了其他问题

#### 更新：2024-12-16

1. 移除搜索源QQ音乐。
2. 增加从Cookie文件导入VIP特权，以下载VIP歌曲的功能。
3. 其他更新

#### 更新: 2019-06-06

1. 修改部分代码
2. 增加本地化

#### 更新:2018-09-06

1. **全新版本发布**。现在增加了一些选项：
2. 用法 : `python3 NetEaseMusic.py ` `[OPTIONS]` `URL` or `NetEaseMusic` `[OPTIONS]` `URL`
3. 选项列表:

   | 选项              | 描述                                 |
   | ----------------- | ------------------------------------ |
   | -h, --help        | 打印帮助信息                         |
   | -s, --single      | 指明给定的链接只有一首歌曲           |
   | -l, --list        | 指明给定的链接是一个播放列表(歌单)   |
   | -v, --video       | 指明给定的链接是一个音频视频         |
   | -r, --range RANGE | 指定下载播放列表(歌单)指定索引的歌曲 |
   |                   | RANGE 模板 '1, 2, 5-7, 8'            |
   | -a, --auto        | 自动添加到iTunes                     |
   | -f, --folder      | 指定歌曲下载的存储目录               |

#### 更新：2018-08-09

1. 增加lame歌曲类别标签。
2. 由于官方网页版API解析失败，现在使用的依然是三方API。我会尽快尝试修复。

#### 更新: 2018-07-17

1. 增加官方API获取歌曲链接。
2. 增加歌曲最佳比特率解析。

#### 更新: 2018-06-14

1. 增加“自动添加到iTunes”询问。
2. 修复了当文件存在或搜索QQ音乐失败是停止下载的情况。

#### 更新:2018-05-28

1. 使用网易云音乐非官方API替换原来的API。该API是从互联网获取的。

#### 更新: 2018-05-22

1. 现在可以使用工具下载歌曲/歌单/专辑了。使用*AD's API*。
2. 现已支持Windows平台
3. 现在已经可以下载网易云音乐的MV了。

#### 更新：2018-05-17

1. 当[网易云音乐](http://music.163.com) 音乐资源不可用时，增加新的搜索源[QQ音乐](http://y.qq.com)。
2. 增加新的依赖库[FFMPEG](http://ffmpeg.org)，用来转换从QQ音乐下载的*.m4a*文件为*.mp3*。

#### 更新：2024-12-16

1. 移除搜索源QQ音乐。
2. 增加从Cookie文件导入VIP特权，以下载VIP歌曲的功能。
3. 其他更新

#### 下载:

1. **下载完整工程**

   ```shell
   git clone https://github.com/Kito0615/NetEaseMusic.git
   ```

   在终端直接运行脚本源码文件(NetEaseMusic.py)。需要python3环境。

   ```shell
   python3 NetEaseMusic.py
   ```

   或者:

   ```shell
   chmod +x NetEaseMusic.py
   ./NetEaseMusic.py
   ```
2. **下载发布文件**

   点击 [这里](https://github.com/Kito0615/NetEaseMusicDownloader/releases), 下载你需要的版本. 再在终端执行:

   ```shell
   ./NetEaseMusic
   ```

   或者拷贝二进制文件到 `/usr/local/bin`, 然后你就可以在任何目录执行:

   ```shell
   NetEaseMusic
   ```

#### 用法:

 参考 [Update:2018-09-06](#更新2018-09-06)

#### 环境:

[Python3.0+](https://www.python.org/downloads/mac-osx/) (需要安装[*requests*](https://github.com/requests/requests)库)

~~[lame](http://lame.sourceforge.net) (用于给音乐添加封面) [这里](https://github.com/Kito0615/NetEaseMusicDownloader/blob/master/Install_lame.md)有一点安装指南。~~

~~[Homebrew](https://brew.sh/)~~

[eyeD3](https://pypi.org/project/eyeD3/)

[License](https://github.com/Kito0615/NetEaseMusicDownloader/blob/master/LICENSE)

[FFMPEG](http://ffmpeg.org)
