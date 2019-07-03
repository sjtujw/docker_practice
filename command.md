# Dockerfile 常用命令
* <strong>FROM</strong><br>
指定base镜像
* <strong>MAINTAINER</strong><br>
设置镜像的作者，可以是任意字符串
* <strong>COPY</strong><br>
将文件从build context复制到镜像
* <strong>ADD</strong><br>
和COPY类似，但对于压缩文件，会自动解压
* <strong>ENV</strong><br>
设置环境变量，可被后面的指令使用
* <strong>EXPOSE</strong><br>
指定容器中的进程会监听某个端口，Docker可以将该端口暴露出来
* <strong>VOLUME</strong><br>
将文件或目录声明为volume
* <strong>WORKDIR</strong><br>
为后面的指令设置镜像中的当前工作目录
* <strong>RUN</strong><br>
在容器中运行指定的命令
* <strong>CMD</strong><br>
容器启动时运行指定的命令<br>
Dockerfile 中可以有多个 CMD 指令，但只有最后一个生效。CMD 可以被 docker run 之后的参数替换。
* <strong>ENTRYPOINT</strong><br>
设置容器启动时运行的命令。<br>
Dockerfile 中可以有多个 ENTRYPOINT 指令，但只有最后一个生效。CMD 或 docker run 之后的参数会被当做参数传递给 ENTRYPOINT
