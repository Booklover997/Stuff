#python 
Sockets allows for connections over [[UDP]] and [[TCP]]

---

```python
import socket

client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
client_socket.connect(('127.0.0.1', 1337))
client_socket.send(b"Do you want to play a game?\n")
received = client_socket.recv(1024)
print(received)
client_socket.close()
```
socket.AF_INET[^1] means that the connection will be over [[IPv4]] not [[IPv6]] which would be done using socket.AF_INET6 or Bluetooth

The second argument socket.SOCK_STREAM tells the socket wether to use [[TCP]] or [[UDP]]
1. First we connect to an ip and port using the .connect() [[Method]]
2. Then we use .send() to send data which much be prefaced with a b for a [[byte object]]
3. The .recv() message since we are connecting to the [[Loopback Address]] and allowing 1024 bytes of data
4. .close() initiates the [[TCP teardown]]

#cheatsheat

| Effect              | Parameter |
| ------------------- | --------- |
| socket.AF_INET      | [[IPv4]]  |
| socket.AF_INET6     | [[IPv6]]  |
| socket.SOCK_STREAM  | [[TCP]]   |
| socket.SOCK_DGRAM   | [[UDP]]   |
| socket.AF_BLUETOOTH | [[Bluetooth]]          |


[^1]: AF_INET stands for Address Family Internet which is used to designate which address families a socket can connect to 







