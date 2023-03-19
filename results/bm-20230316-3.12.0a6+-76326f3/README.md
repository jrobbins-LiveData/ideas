# Results

- fork: faster-cpython
- ref: no_deep_freeze
- version: 3.12.0a6+
- commit hash: [76326f3](https://github.com/faster%2dcpython/cpython/commit/76326f3)
- commit date: 2023-03-16T03:28:03+00:00
- commit merge base: [4f5774f648eafd1a7076ecf9af9629fb81baa363](https://github.com/faster%2dcpython/cpython/commit/4f5774f648eafd1a7076ecf9af9629fb81baa363)

## linux x86_64

- [GitHub Action run](https://github.com/faster-cpython/benchmarking/actions/runs/4447134458)
- cpu model: Intel(R) Xeon(R) W-2255 CPU @ 3.70GHz
- platform: Linux-5.4.0-122-generic-x86_64-with-glibc2.31
- [raw results](bm-20230316-linux-x86_64-faster%252dcpython-no_deep_freeze-3.12.0a6%2B-76326f3.json)

### vs. 3.10.4

- 1.30x faster \*
- missing benchmarks: flaskblogging, mypy, pylint
- new benchmarks: asyncio_tcp, comprehensions, create_gc_cycles, dask, djangocms, gc_traversal, mypy2
- [table](bm-20230316-linux-x86_64-faster%252dcpython-no_deep_freeze-3.12.0a6%2B-76326f3-vs-3.10.4.md)
- [plot](bm-20230316-linux-x86_64-faster%252dcpython-no_deep_freeze-3.12.0a6%2B-76326f3-vs-3.10.4.png)

### vs. 3.11.0

- 1.03x faster \*
- missing benchmarks: flaskblogging, mypy, pylint
- new benchmarks: asyncio_tcp, comprehensions, create_gc_cycles, dask, djangocms, gc_traversal, mypy2
- [table](bm-20230316-linux-x86_64-faster%252dcpython-no_deep_freeze-3.12.0a6%2B-76326f3-vs-3.11.0.md)
- [plot](bm-20230316-linux-x86_64-faster%252dcpython-no_deep_freeze-3.12.0a6%2B-76326f3-vs-3.11.0.png)

### vs. base

- 1.01x slower
- [table](bm-20230316-linux-x86_64-faster%252dcpython-no_deep_freeze-3.12.0a6%2B-76326f3-vs-base.md)
- [plot](bm-20230316-linux-x86_64-faster%252dcpython-no_deep_freeze-3.12.0a6%2B-76326f3-vs-base.png)
