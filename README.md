# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.
   Name:A.Afifa Reg.no:212223040008
## PROGRAM:
## client:
```import socket
s=socket.socket()
s.bind(('localhost',8000))
s.listen(5)
c,addr=s.accept()
while True:
clientMessage=c.recv(1024).decode()
c.send((clientMessage.encode()))
```
## server :
```import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
msg=input("client>")
s.send(msg.encode())
print("server>",s.recv(1024).decode())
```
## OUPUT:
## client:
![320844996-9eb79a9e-25da-4c33-8051-39c4785b9902](https://github.com/afifa17112005/3a.Sockets_Creation_for_Echo_Client_and_Echo_Server/assets/147080931/181efa82-785b-4717-a2fd-53db2ab6a3e4)

## server :
![320845075-06e36138-3ee0-41d8-96c6-d20b97a18c8f](https://github.com/afifa17112005/3a.Sockets_Creation_for_Echo_Client_and_Echo_Server/assets/147080931/4718a63a-11eb-4663-8264-8f0b57912bc0)

## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
