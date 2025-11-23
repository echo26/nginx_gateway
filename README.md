## traffic test

#### apache benchmark

```
ab -n 10000 -c 100 -k -t 60 http://3.238.182.73/
```

#### TCP connection Lifecycle

**Connection Establishment**

- SYN : client sends a SYN
- SYN-ACK : Server responds with a SYN-ACK
- ACK : Client sends a final ACK
- State : Connection ESTABLISHED

**Data Transfer**

**Connection Termination**

- FIN : One side sends a FIN
- ACK : The other side acknowledges the FIN
- ACK : The first side acknowledges the second FIN
- STATE : The connection enters the TIME_WAIT state on the actively closing side

#### Keep-Alive

HTTP Keep-Alive (Application Layer)

- keeps TCP connection established state and waits for a new request from the client

TCP Keep-Alive (Transport Layer)

-
