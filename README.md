# learning-erlang
learning basics of Erlang

Compiling and running programs under Linux
------------------------------------------

### Installation

```
sudo apt-get install erlang-ic
```

### Hello world program

```erl
% hello world program
-module(helloworld).
-export([start/0]).

start() ->
    io:fwrite("Hello, world!\n").
```

### Compilation

```
erlc helloworld.erl
```

This command will create `helloworld.beam` file.

### Execution

```
erl -noshell -s helloworld start -s init stop
```
