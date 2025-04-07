# Cabana

## 스트리밍을 이용한 실행

* 노트북과 콤마를 같은 네트워크에 접속
* [콤마에 SSH 접속](ssh1.md)

```
cd /data/openpilot/cereal/messaging/
./bridge &
```

* 노트북의 터미널에서

```
cabana --stream --zmq <ipaddress>
```



## 라우트를 이용한 실행

```
cd tools/cabana
cabana "a2a0ccea32023010|2023-07-27--13-01-19"
```







## 참고

```
$ ./cabana -h
Usage: ./cabana [options] route

Options:
  -h, --help                     Displays help on commandline options.
  --help-all                     Displays help including Qt specific options.
  --demo                         use a demo route instead of providing your own
  --qcam                         load qcamera
  --ecam                         load wide road camera
  --stream                       read can messages from live streaming
  --panda                        read can messages from panda
  --panda-serial <panda-serial>  read can messages from panda with given serial
  --socketcan <socketcan>        read can messages from given SocketCAN device
  --zmq <zmq>                    the ip address on which to receive zmq
                                 messages
  --data_dir <data_dir>          local directory with routes
  --no-vipc                      do not output video
  --dbc <dbc>                    dbc file to open

Arguments:
  route                          the drive to replay. find your drives at
                                 connect.comma.ai
```
