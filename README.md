Examples for Xapian
===================

It is an implementation of PHP examples in Erlang.
http://xapian.org/docs/bindings/php/examples/

```shell
$ echo "erlang" | ./bin/simpleindex.escript priv/test_db/simple/
$ ./bin/simplesearch.escript priv/test_db/simple/ erlang
1 results found:
1: 100% docid=1 [erlang
]

```


```shell
./bin/index_filters.escript ./priv/100-objects-v1-utf8.csv ./priv/test_db/filters 
./bin/index_facets.escript ./priv/100-objects-v1-utf8.csv ./priv/test_db/facets
./bin/index_ranges2.escript priv/states.csv priv/test_db/ranges2
./bin/index_ranges.escript ./priv/100-objects-v1-utf8.csv ./priv/test_db/ranges
./bin/search_facets.escript ./priv/test_db/facets clock
./bin/search_filters.escript priv/test_db/filters clock 'steel (metal)' 
```

Installation
============

```shell
rebar get-deps && rebar compile
```
