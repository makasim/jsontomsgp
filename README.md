# Copy json to message pack 

The package provides tools for converting json to message pack with minimal overhead.

`jsontomsgp.CopyBytes` - takes json bytes and writes message pack bytes to the writer.

## Benchmarks

```
$go test ./... -bench=. -run=none
goos: darwin
goarch: arm64
pkg: github.com/makasim/jsontomsgp
BenchmarkCopyJSONToMsgp-10    	 2112625	       562.5 ns/op	       0 B/op	       0 allocs/op
PASS
ok  	github.com/makasim/jsontomsgp	1.939s
```

