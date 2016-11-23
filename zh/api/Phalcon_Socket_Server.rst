Class **Phalcon\\Socket\\Server**
=================================

*extends* abstract class :doc:`Phalcon\\Socket <Phalcon_Socket>`

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/dreamsxin/cphalcon7/blob/master/ext/socket/server.c" class="btn btn-default btn-sm">Source on GitHub</a>`




Constants
---------

*integer* **AF_UNIX**

*integer* **AF_INET**

*integer* **AF_INET6**

*integer* **SOCK_STREAM**

*integer* **SOCK_DGRAM**

*integer* **SOCK_RAW**

*integer* **SOCK_SEQPACKET**

*integer* **SOCK_RDM**

*integer* **IPPROTO_IP**

*integer* **IPPROTO_IPV6**

*integer* **SOL_SOCKET**

*integer* **SOL_TCP**

*integer* **SOL_UDP**

*integer* **SO_DEBUG**

*integer* **SO_REUSEADDR**

*integer* **SO_REUSEPORT**

*integer* **TCP_NODELAY**

*integer* **TCP_QUICKACK**

*integer* **USE_SELECT**

*integer* **USE_EPOLL**

Methods
-------

public  **__construct** (*string* $address, *int* $port, [*int* $domain], [*int* $type], [*int* $protocol])

Phalcon\\Socket\\Server constructor



public *boolean*  **setEvent** (*unknown* $event)

Sets the event



public *int*  **getEvent** ()

Gets the event



public *boolean*  **listen** ([*int* $backlog])

Listens for a connection on a socket



public :doc:`Phalcon\\Socket\\Client <Phalcon_Socket_Client>`  **accept** ()

Accept a connection



public :doc:`Phalcon\\Socket\\Client <Phalcon_Socket_Client>`  **getClients** ()

Gets all connections



public :doc:`Phalcon\\Socket\\Client <Phalcon_Socket_Client>`  **getClient** (*unknown* $socketId)

Gets a connection



public :doc:`Phalcon\\Socket\\Server <Phalcon_Socket_Server>`  **disconnect** (*unknown* $socketId)

Close a client



public  **run** ()

Run the Server



public *resource*  **getSocket** () inherited from Phalcon\\Socket

Gets the socket



public *int*  **getSocketId** () inherited from Phalcon\\Socket

Gets the socket id



protected  **_throwSocketException** () inherited from Phalcon\\Socket

Throws an socket exception



public *boolean*  **setBlocking** (*int* $flag) inherited from Phalcon\\Socket

Set the socket to blocking / non blocking



public *boolean*  **isBlocking** () inherited from Phalcon\\Socket

Checks the socket blocking / non blocking



public *boolean*  **setOption** (*int* $level, *int* $optname, *mixed* $optval) inherited from Phalcon\\Socket

Set the socket to blocking / non blocking



public  **close** () inherited from Phalcon\\Socket

Close the socket



public  **isClose** () inherited from Phalcon\\Socket

Check if the socket close



public  **__destruct** () inherited from Phalcon\\Socket

Cleans up the socket and the resource



