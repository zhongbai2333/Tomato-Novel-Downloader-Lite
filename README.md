# 番茄小说下载器精简版
如你所见，这个程序只有不到16kb的python文件，但这不影响它的功能！这个程序简单易操作，可以满足你的小说下载需求，需要运行此程序的话，最好是在终端中，以下的所有需要输入的内容都需要在终端中进行，并且在使用此程序之前，您必须先安装python！
## 我该如何使用？
你可以通过输入书籍id以及需要保存的路径来进行下载
你还需要依次输入以下的命令来保证程序的运行：
(电脑端只需要运行以下命令的第3、4个即可)
```bash
sed -i 's@^\(deb.*stable main\)$@#\1\ndeb https://mirrors.tuna.tsinghua.edu.cn/termux/apt/termux-main stable main@' $PREFIX/etc/apt/sources.list
apt update && apt upgrade
pkg install python
pip install requests beautifulsoup4 lxml tqdm fake-useragent
```
## 常见问题
1.`此程序的优势在哪？`

本程序的初衷就是极致简化番茄小说下载器的代码，使程序更加易于操作与运行、更加稳定和快速，并且全平台通用，小白也能轻松上手！

2.`为什么我在安装lxml库的时候始终安装不了？`

按照以下步骤解决：
```bash
apt install clang 
apt install libxml2
apt install libxslt 
pip install cython 
CFLAGS="-O0" pip install lxml
```

3.`手机端该如何运行？`

可以正常运行，为了防止有些零基础的小白下载到了此程序，我们为您准备了一些教程：

*下载termux(链接:(https://github.com/termux/termux-app/releases/tag/v0.118.1 )，用文件管理器，找到自己下载的源代码(2.py)，复制当前的目录，返回termux，输入cd+空格+复制的目录，然后回车，最后输入`python 2.py`

再次回车即可。

（先运行安装命令后再进行以上操作）

4.`电脑端该如何运行？`

步骤是和手机端差不多的，有一些适用于手机端的安装命令不适用于电脑端，还请仔细辨别！
步骤：查看下载的2.py代码的目录位置，返回终端后输入：cd+空格+复制的目录，然后回车，最后再输入`python 2.py`

再次回车即可。

注意：如果要切换到有空格的目录中，您需要使用引号来引起来：

> cd+空格+"复制的目录"

**注意**：请确保您要运行的2.py文件与当前工作目录位于同一驱动器（例如D盘）。如果2.py文件位于其他驱动器，请先切换到该驱动器。您可以通过输入驱动器名称加冒号(例如【D:】)并按回车键来切换驱动器。

（先运行安装命令后再进行以上操作）

5.`小说id是什么？在哪里获取？`

首先你需要找到自己想下载的小说的详情页(例如https://fanqienovel.com/page/7143038691944959011 )，链接中“7143038691944959011”就是小说id

6.`我是纯小白，2.py代码在哪里下载啊`

直接点击此链接(https://github.com/Dlmily/Tomato-Novel-Downloader-Lite/releases/ )先找到最新版本，然后在最新版本中找到”Assets”并点击来展开内容(如果已展开就不必进行此操作)。在展开的内容中找到2.py代码，点击下载即可

7.`我无法正常运行代码，有没有可执行文件代替？`

先将代码以zip格式下载，之后解压到文件夹，接着运行“build-executable.yml”即可

## 注意事项（必看）
由于使用的是api，所以未来不知道有哪一天突然失效，如果真的出现了，请立即在“Issues”页面中回复！

如果您在使用本程序的时候出现了下载章节失败的情况，也许并不是api失效了，可能是因为调用api人数过多，导致api暂时关闭，如果遇到了这种情况，请稍后再试，另外，您需要下载的小说api可能会因没有更新所以下载失败。

千万不要想着耍小聪明：“欸，我改一下线程数不就能快速下载了吗？”请打消这种念头！因为这样会加大服务器压力！！！

在v1.6.3.2版本以后已经可以使用vpn或其他网络代理了，之前的版本依旧不能使用！

如果您也没有遇到以上的这种情况，请检查要下载的小说章节数量有多少，不建议大于1000章！如果真的出现了这种情况，可以先中断程序，再运行程序

>划重点：切记！不能将此程序用于违法用途，例如将下载到的小说进行转载、给不良人员分享此程序使用等。本开发者严禁不支持这样做！！！并且请不要将api进行转载使用，除非您已经与开发者协商过，否则后果自负！下载到的小说仅供自行阅读，看完之后请立即删除文件，以免造成侵权，如果您还是偷尝禁果，需自行承担由此引发的任何法律责任和风险。程序的作者及项目贡献者不对因使用本程序所造成的任何损失、损害或法律后果负责！

## 赞助/了解新产品
https://afdian.com/a/dlbaokanluntanos

## 免责声明
  本程序仅供 Python 网络爬虫技术、网页数据处理及相关研究的学习用途。请勿将其用于任何违反法律法规或侵犯他人权益的活动。
  
  使用本程序的用户需自行承担由此引发的任何法律责任和风险。程序的作者及项目贡献者不对因使用本程序所造成的任何损失、损害或法律后果负责。
  
  在使用本程序之前，请确保您遵守适用的法律法规以及目标网站的使用政策。如有任何疑问或顾虑，请咨询专业法律顾问。

## 感谢
感谢用户选择此程序，如果喜欢可以加star，如果有什么对本程序的建议，请在“Issues”页面提出。您的喜欢就是我更新的最大动力❤️
***
感谢来自QQ用户@终忆的api！

感谢来自Github用户@jingluopro的api！

感谢来自[此项目](https://github.com/POf-L/Fanqie-novel-Downloader)的api！

感谢所有赞助此程序的赞助者们！
