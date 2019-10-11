# w

import socket

client = socket.socket()  # 生成一个socket连接对象

client.connect(("localhost", 6666))  # 和目标主机建立连接

client.send('hello world!'.encode())  # 向对方发送数据

client.close()  # 断开连接
