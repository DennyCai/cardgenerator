# cardgenerator
【仅做研究使用，请遵守当地法律法规，法律后果自负】

## 更新:
- 自动改变头像大小
- 自动从纯色背景中抠图
- 支持pip安装

## ToDo
- 自动从复杂背景下抠图

## 环境
- numpy
- pillow
- opencv

## 下载
## pip安装
`pip install idcardgenerator`

```
from idcardgenerator import gui
gui.run()
```
文件会生成在运行目录

### Windows
[下载](https://github.com/airob0t/idcardgenerator/releases/download/win_v1.3/idcardgenerator.exe)
### Mac
[下载](https://github.com/airob0t/idcardgenerator/releases/download/v1.1/idcardgenerator)

## 打包程序

安装pyinstaller

`pip install pyinstaller`

Mac打包(打包成Mac app尚有问题未解决)

    pyinstaller -i usedres/ico.icns --windowed --clean --noconfirm --onefile --add-data ./usedres:./usedres idcardgenerator.py

Windows打包

    pyinstaller -i usedres/ico.ico --windowed --clean --noconfirm --onefile --add-data "usedres;usedres" idcardgenerator.py
