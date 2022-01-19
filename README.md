# 音视频处理基础知识学习笔记
学习地址：https://coding.imooc.com/learn/list/415.html

---

## 第1章：课程导学与准备
## 第2章：音视频环境基础
**音视频应用场景：**
1. 互动直播系统（实时互动、强交互、一对一、一对多、比如在线会议）
2. 娱乐直播系统（）
3. 音视频特效（短视频、配音、配视频、变声）
4. 音视频编辑（素材剪切）

**音视频处理常用工具：**
1. ffmpeg
2. ffmplay
3. vlc

**简单的网络直播架构模型**

<img src="https://github.com/Sunshine162/audio-video-basics/blob/main/others/img001.png" alt="简单的网络直播架构模型"
     width="300px" align="left"><br>

推流工具：向流媒体服务器推送音视频数据<br>
流媒体服务器：负责音视频服务器的转发<br>
拉流工具：从流媒体服务器拉取音视频数据<br><br>

**环境变量** <br>
vim打开 ~/.bashrc,添加
```
export PATH=path_of_ffmepg:PATH
export PKG_CONFIG_PATH=xxxx  #设置头文件与库文件位置
```
使环境变量生效：
```
source ~/.bashrc
```
查看libavutil库的库文件和头文件
```
pkg-config --libs --cflags libavutil
```
