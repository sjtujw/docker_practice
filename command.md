# Dockerfile 常用命令
* FROM<br>
指定base镜像
* MAINTAINER<br>
设置镜像的作者，可以是任意字符串
* COPY<br>
将文件从build context复制到镜像
* ADD<br>
和COPY类似，但对于压缩文件，会自动解压
* ENV<br>
设置环境变量，可被后面的指令使用
* EXPOSE<br>
指定容器中的进程会监听某个端口，Docker可以将该端口暴露出来
* VOLUME<br>
将文件或目录声明为volume
* WORKDIR<br>
为后面的指令设置镜像中的当前工作目录
* RUN<br>
在容器中运行指定的命令
* CMD<br>
容器启动时运行指定的命令<br>
Dockerfile 中可以有多个 CMD 指令，但只有最后一个生效。CMD 可以被 docker run 之后的参数替换。
* ENTRYPOINT<br>
设置容器启动时运行的命令。<br>
Dockerfile 中可以有多个 ENTRYPOINT 指令，但只有最后一个生效。CMD 或 docker run 之后的参数会被当做参数传递给 ENTRYPOINT
