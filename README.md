h1. Test AWSIoTPython in local machine
*Pre-condition*

Window:
- install mosquitto broker
- install paho library

Linux:
- AWSIoTPythonSDK
- install paho (optional, paho may installed when setting up AWSIoTPythonSDK )


*Topology Overview*
- Linux is client which publishes message
- Window is client which subscribes to receive message from Linux

*How to run*
On window
1. Start mosquitto broker
Open command prompt
mosquitto -p 8883

2. Start subcriber
Open command prompt
python D:\workspace\AWSIoTPython\win\client_sub.py

On linux
3. Start publisher
Open terminal
python \home\mTrumpy\workspace\AWSIoTPython\linux\basicPubSub.py

4. Chek received message on subcriber command prompt (step 2)

Note:
- Publisher program is runnable in Window also.
- Path file is specified for particular machine. Repalce it by yours path.
