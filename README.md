
## nanopb

Protocol Buffers with small code size.

License: zlib license.

Download: `https://github.com/nanopb/nanopb.git`

Version: Commits on Jan 13 2020, Fix errors in fuzztest testcase

## howto

1. install python

2. install python-protobuf 

`$ pip install protobuf>=2.5`

update pip if need

3. install protoc

`https://github.com/protocolbuffers/protobuf/releases`

put `protoc.exe` into `PATH` directory.

4. build nanopb_pb2.py

enter `src/nanopb/generator/proto` directory:

```
$ ../protoc --python_out=. nanopb_pb2.py
```

5. build fileproto.pb.c

enter `src\nanopb\examples\network_server` directory:

```
$ ../../generator/protoc --plugin=protoc-gen-nanopb=D:/Work/workspace_iot/msrtos_base/nanopb/src/nanopb/generator/protoc-gen-nanopb.bat --nanopb_out=. fileproto.proto
```

