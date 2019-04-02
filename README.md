### Tetris-WebSocket
#### Introduction
imooc原课程网址：https://www.imooc.com/video/15619  
原课程完成双人版
1. **Single版：** 俄罗斯方块的JS实现，完整的游戏逻辑，包括七种方块、旋转、下坠、消行计分、定时增加干扰行。
    
    Single的全部前端代码位于webapp的single文件夹
1. **双人版：** 基于socket.io通信与JS实现双人火拼俄罗斯方块，双人双屏，本地多开网页.  

    双人版的全部前端代码位于webapp的socket-io文件夹

   **游戏机制：**
   1. 游戏渲染计时器200ms
   2. 消行得分：1-100, 2-300, 3-500, 4-700
   3. 每隔十秒在底部添加 1 个干扰行，若游戏时间超过 2 分钟则变为增加 2 行
   4. 若同时消除两行及以上则在对方游戏区域内添加一个底部干扰行
   
   双人版除了直接打开本地文件外你还可以通过Tomcat发布JavaWeb在本地进行测试...只需用同样的方式node wsServer.js启动Socket.io的服务即可
3. **天梯版：** JavaEE - WebSocket双人双屏天梯积分匹配，真实对战（开发中...）

#### Technical selection
**双人版**
1. Socket.io 1.3.7
2. JS

**天梯版**  

持续更新...