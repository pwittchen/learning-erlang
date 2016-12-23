learning-erlang
===============
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

IDE
---
http://ignatov.github.io/intellij-erlang/

References
----------

### More technical
- http://www.erlang.org/
- http://erlang.org/faq/getting_started.html
- http://www.thegeekstuff.com/2010/05/erlang-hello-world-example/
- http://learnyousomeerlang.com/
- http://stackoverflow.com/questions/1017017/what-is-the-best-way-to-learn-erlang

### About Erlang fuss
- https://pragprog.com/articles/erlang
- https://www.fastcompany.com/3026758/inside-erlang-the-rare-programming-language-behind-whatsapps-success
