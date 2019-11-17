# UFO_Hand-in_3
Prototyping, Evaluation, and Documentation Exercise 

## Formulate a hypothesis/problem statement about the influence of location of client and server.
Our hypothesis is that depending on the geographical location of the client and server, the response time differ. The further the server is from the client, the slower the response would be, and in turn, the slower the client application will seem in terms of responsiveness.

## Plan an experiment, which will give you numbers regarding the influence of geographic location of server and client.
Our experiment included booting up 3 servers on Digital Ocean in different locations, one in New York, one in Singapore, and one in Amsterdam, and pinging them (locally from Copenhagen) to see the difference in response time.

## Execute the experiment.
The measurements have been achieved with a simple ping command in a windows cmd.

Here is the result of our experiment:

### New York Server
Pinging 157.245.124.150 with 32 bytes of data:
Reply from 157.245.124.150: bytes=32 time=199ms TTL=56
Reply from 157.245.124.150: bytes=32 time=426ms TTL=56
Reply from 157.245.124.150: bytes=32 time=116ms TTL=56
Reply from 157.245.124.150: bytes=32 time=143ms TTL=56

Ping statistics for 157.245.124.150:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 116ms, Maximum = 426ms, Average = 221ms
    
### Singapore Server
Pinging 167.71.196.88 with 32 bytes of data:
Reply from 167.71.196.88: bytes=32 time=295ms TTL=49
Reply from 167.71.196.88: bytes=32 time=302ms TTL=49
Reply from 167.71.196.88: bytes=32 time=220ms TTL=49
Reply from 167.71.196.88: bytes=32 time=236ms TTL=49

Ping statistics for 167.71.196.88:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 220ms, Maximum = 302ms, Average = 263ms
    
### Amsterdam Server
Pinging 142.93.234.150 with 32 bytes of data:
Reply from 142.93.234.150: bytes=32 time=17ms TTL=57
Reply from 142.93.234.150: bytes=32 time=15ms TTL=57
Reply from 142.93.234.150: bytes=32 time=17ms TTL=57
Reply from 142.93.234.150: bytes=32 time=15ms TTL=57

Ping statistics for 142.93.234.150:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 15ms, Maximum = 17ms, Average = 16ms
    

## Evaluate your experiment and interpret the measurements and results.
By interpreting the 3 measurements that we have taken, we can conclude that the location of the server has an effect on the response time, since our closest server, in Amsterdam, performed, on average, 1643% better than our Singapore server, and 1381% better than our New York Server, in terms of response time.
