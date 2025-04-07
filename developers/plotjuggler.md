# PlotJuggler

## 초기 설치

```
cd tools/plotjuggler && ./juggle.py --install
```

## 스트리밍을 이용

* 노트북을 콤마와 같은 네트워크에 접속
* [`콤마에 SSH로 접속`](ssh1.md)

```
cd /data/openpilot && ./cereal messaging/bridge 
```

* 노트북의 터미널에서

```
cd tools/plotjuggler
ZMQ=1 ./juggle.py --stream
```

* `입력 후,`드롭다운에서 Cereal Subscriber 플러그인을 찾아 시작을 클릭



## 라우트 이름을 이용

```
cd tools/plotjuggler
./juggle.py "a2a0ccea32023010/2023-07-27--13-01-19"
```





## 참고

```
$ ./juggle.py -h
usage: juggle.py [-h] [--demo] [--can] [--stream] [--layout [LAYOUT]] [--install] [--dbc DBC]
                 [route_or_segment_name] [segment_count]

A helper to run PlotJuggler on openpilot routes

positional arguments:
  route_or_segment_name
                        The route or segment name to plot (cabana share URL accepted) (default: None)
  segment_count         The number of segments to plot (default: None)

optional arguments:
  -h, --help            show this help message and exit
  --demo                Use the demo route instead of providing one (default: False)
  --can                 Parse CAN data (default: False)
  --stream              Start PlotJuggler in streaming mode (default: False)
  --layout [LAYOUT]     Run PlotJuggler with a pre-defined layout (default: None)
  --install             Install or update PlotJuggler + plugins (default: False)
  --dbc DBC             Set the DBC name to load for parsing CAN data. If not set, the DBC will be automatically
                        inferred from the logs. (default: None)
```
