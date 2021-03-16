这是我学跨域时做的一个小实验
大致步骤
1. 创建目录
qq-com中有一个server.js，用来模拟QQ空间
marshall-com中有一个server.js，用来模拟坏人的网站。
安装 node-dev
`yarn global add node-dev`
2. qq-com
/index.html是首页
/qq.js是JS脚本文件
/friends.json是模拟的友好数据
监听端口为8888，访问https://127.0.0.1:8888
3. marshall-com
/index.html是首页
/marshall.js是JS脚本文件
监听端口为9999，访问https://127.0.0.1:9999

4. 设置 hosts
    ```
    127.0.0.1 qq.com
    127.0.0.1 marshall.com
    ```
5. 打开两个页面 qq.com:8888/index.html 和 marshall.com:9999/index.html
6. 记得做完之后，删掉 hosts 里的两行，否则 qq.com 无法正常访问！