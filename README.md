# Erlang learning

## hello_bin

Example of command line tool on Erlang.

To run:
```bash
$ ./hello_bin
```
Or:
```bash
$ escript hello_bin
```

## hello.erl

Example of Elang module.

To run:
```bash
$ erl
Erlang/OTP 22 [erts-10.4] [source] [64-bit] [smp:4:4] [ds:4:4:10] [async-threads:1] [hipe] [dtrace]

Eshell V10.4  (abort with ^G)
1> c(hello).
{ok,hello}
2> hello:world().
Hello, world
ok
```

## gen_tcp_server.erl

Simple Erlang server based on `gen_tcp` module.

To run:
```bash
$ erl
Erlang/OTP 22 [erts-10.4] [source] [64-bit] [smp:4:4] [ds:4:4:10] [async-threads:1] [hipe] [dtrace]

Eshell V10.4  (abort with ^G)
1> c(gen_tcp_server).
{ok,hello}
2> Pid = gen_tcp_server:start(4000).
<0.85.0>
```
Server will be started on port `4000`.

## inets_server.erl

Simple Erlang server based on `inets` module.

To run:
```bash
$ erl
Erlang/OTP 22 [erts-10.4] [source] [64-bit] [smp:4:4] [ds:4:4:10] [async-threads:1] [hipe] [dtrace]

Eshell V10.4  (abort with ^G)
1> c(inets_server).
{ok,inets_server}
2> {ok, Pid} = inets_server:start().
{ok,<0.96.0>}
```
Server will be started on port `4000`.

Also you can run in script style:
```bash
$ escript inets_server.erl
```
