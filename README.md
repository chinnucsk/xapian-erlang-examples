Examples for Xapian
===================

It is an implementation of PHP examples in Erlang.
http://xapian.org/docs/bindings/php/examples/

```shell
$ echo "erlang" | ./bin/simpleindex.escript priv/test_db/test
$ ./bin/simplesearch.escript priv/test_db/test/ erlang
1 results found:
1: 100% docid=1 [erlang
]

```


```shell
./bin/index_filters.escript ./priv/100-objects-v1-utf8.csv ./priv/test_db/index_filters 
```

Installation
============

```shell
rebar get-deps && rebar compile
```
