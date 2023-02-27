# network_learning

# check port

- socket check and build
    ```
    import socket 
    def check_port(port):
      sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
      res = sock.connect_ex(('localhost', port))
      sock.close()
      return res == 0
    print(check_port(36439))
    ```
    
    ```
    from socket import *
    serverNegSocket = socket(AF_INET, SOCK_DGRAM)
    serverNegSocket.bind(('', 0))
    print(serverNegSocket.getsockname()[1])

    ```

