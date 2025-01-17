
# Results vs. 3.11.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 61f1e67
- commit date: 2023-02-18
- overall geometric mean: 1.03x faster \*

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230218-linux-x86_64-python-main-3.12.0a5+-61f1e67 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 257 ms                                                 | 247 ms: 1.04x faster                                   |
| chameleon      | 6.41 ms                                                | 6.49 ms: 1.01x slower                                  |
| docutils       | 2.60 sec                                               | 2.54 sec: 1.02x faster                                 |
| html5lib       | 63.2 ms                                                | 61.1 ms: 1.03x faster                                  |
| tornado_http   | 96.6 ms                                                | 95.2 ms: 1.02x faster                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230218-linux-x86_64-python-main-3.12.0a5+-61f1e67 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pidigits       | 199 ms                                                 | 189 ms: 1.05x faster                                   |
| float          | 76.3 ms                                                | 73.1 ms: 1.04x faster                                  |
| nbody          | 95.0 ms                                                | 92.9 ms: 1.02x faster                                  |
| Geometric mean | (ref)                                                  | 1.04x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230218-linux-x86_64-python-main-3.12.0a5+-61f1e67 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 136 ms                                                 | 130 ms: 1.05x faster                                   |
| regex_v8       | 22.3 ms                                                | 22.0 ms: 1.01x faster                                  |
| regex_effbot   | 3.36 ms                                                | 3.38 ms: 1.01x slower                                  |
| regex_dna      | 203 ms                                                 | 220 ms: 1.08x slower                                   |
| Geometric mean | (ref)                                                  | 1.01x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230218-linux-x86_64-python-main-3.12.0a5+-61f1e67 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_dumps           | 12.7 ms                                                | 9.58 ms: 1.32x faster                                  |
| unpickle_pure_python | 225 us                                                 | 198 us: 1.14x faster                                   |
| json_loads           | 26.2 us                                                | 23.7 us: 1.11x faster                                  |
| pickle_pure_python   | 304 us                                                 | 283 us: 1.07x faster                                   |
| xml_etree_parse      | 158 ms                                                 | 149 ms: 1.06x faster                                   |
| xml_etree_iterparse  | 103 ms                                                 | 100 ms: 1.03x faster                                   |
| unpickle_list        | 4.95 us                                                | 5.06 us: 1.02x slower                                  |
| pickle_list          | 4.17 us                                                | 4.29 us: 1.03x slower                                  |
| xml_etree_process    | 53.8 ms                                                | 55.4 ms: 1.03x slower                                  |
| pickle               | 9.79 us                                                | 10.1 us: 1.03x slower                                  |
| pickle_dict          | 31.4 us                                                | 32.5 us: 1.04x slower                                  |
| xml_etree_generate   | 76.2 ms                                                | 81.2 ms: 1.06x slower                                  |
| Geometric mean       | (ref)                                                  | 1.04x faster                                           |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230218-linux-x86_64-python-main-3.12.0a5+-61f1e67 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 8.36 ms                                                | 9.00 ms: 1.08x slower                                  |
| python_startup_no_site | 5.96 ms                                                | 6.52 ms: 1.09x slower                                  |
| Geometric mean         | (ref)                                                  | 1.08x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230218-linux-x86_64-python-main-3.12.0a5+-61f1e67 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| genshi_xml      | 52.1 ms                                                | 48.3 ms: 1.08x faster                                  |
| genshi_text     | 22.1 ms                                                | 21.0 ms: 1.05x faster                                  |
| mako            | 9.85 ms                                                | 9.92 ms: 1.01x slower                                  |
| django_template | 32.5 ms                                                | 34.0 ms: 1.05x slower                                  |
| Geometric mean  | (ref)                                                  | 1.02x faster                                           |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230218-linux-x86_64-python-main-3.12.0a5+-61f1e67 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| generators              | 72.2 ms                                                | 30.5 ms: 2.37x faster                                  |
| json_dumps              | 12.7 ms                                                | 9.58 ms: 1.32x faster                                  |
| coroutines              | 26.1 ms                                                | 22.9 ms: 1.14x faster                                  |
| deltablue               | 3.64 ms                                                | 3.21 ms: 1.14x faster                                  |
| unpickle_pure_python    | 225 us                                                 | 198 us: 1.14x faster                                   |
| json_loads              | 26.2 us                                                | 23.7 us: 1.11x faster                                  |
| scimark_sparse_mat_mult | 4.40 ms                                                | 3.98 ms: 1.10x faster                                  |
| richards                | 46.2 ms                                                | 42.0 ms: 1.10x faster                                  |
| json                    | 4.95 ms                                                | 4.54 ms: 1.09x faster                                  |
| go                      | 143 ms                                                 | 133 ms: 1.08x faster                                   |
| fannkuch                | 388 ms                                                 | 360 ms: 1.08x faster                                   |
| genshi_xml              | 52.1 ms                                                | 48.3 ms: 1.08x faster                                  |
| scimark_fft             | 329 ms                                                 | 305 ms: 1.08x faster                                   |
| pickle_pure_python      | 304 us                                                 | 283 us: 1.07x faster                                   |
| xml_etree_parse         | 158 ms                                                 | 149 ms: 1.06x faster                                   |
| nqueens                 | 85.0 ms                                                | 80.0 ms: 1.06x faster                                  |
| scimark_sor             | 115 ms                                                 | 109 ms: 1.06x faster                                   |
| mdp                     | 2.62 sec                                               | 2.48 sec: 1.06x faster                                 |
| sympy_str               | 287 ms                                                 | 273 ms: 1.05x faster                                   |
| pidigits                | 199 ms                                                 | 189 ms: 1.05x faster                                   |
| genshi_text             | 22.1 ms                                                | 21.0 ms: 1.05x faster                                  |
| logging_silent          | 98.5 ns                                                | 93.9 ns: 1.05x faster                                  |
| pycparser               | 1.17 sec                                               | 1.12 sec: 1.05x faster                                 |
| sympy_integrate         | 20.9 ms                                                | 19.9 ms: 1.05x faster                                  |
| logging_simple          | 6.06 us                                                | 5.80 us: 1.05x faster                                  |
| regex_compile           | 136 ms                                                 | 130 ms: 1.05x faster                                   |
| coverage                | 101 ms                                                 | 96.3 ms: 1.04x faster                                  |
| float                   | 76.3 ms                                                | 73.1 ms: 1.04x faster                                  |
| chaos                   | 68.6 ms                                                | 65.7 ms: 1.04x faster                                  |
| pyflate                 | 417 ms                                                 | 400 ms: 1.04x faster                                   |
| deepcopy_memo           | 36.4 us                                                | 34.9 us: 1.04x faster                                  |
| sympy_sum               | 166 ms                                                 | 159 ms: 1.04x faster                                   |
| 2to3                    | 257 ms                                                 | 247 ms: 1.04x faster                                   |
| sympy_expand            | 472 ms                                                 | 454 ms: 1.04x faster                                   |
| sqlglot_optimize        | 53.0 ms                                                | 51.0 ms: 1.04x faster                                  |
| aiohttp                 | 1.05 ms                                                | 1.01 ms: 1.04x faster                                  |
| deepcopy                | 344 us                                                 | 332 us: 1.04x faster                                   |
| hexiom                  | 6.35 ms                                                | 6.13 ms: 1.04x faster                                  |
| sqlglot_normalize       | 108 ms                                                 | 104 ms: 1.03x faster                                   |
| spectral_norm           | 99.9 ms                                                | 96.6 ms: 1.03x faster                                  |
| html5lib                | 63.2 ms                                                | 61.1 ms: 1.03x faster                                  |
| pprint_pformat          | 1.44 sec                                               | 1.40 sec: 1.03x faster                                 |
| scimark_monte_carlo     | 68.3 ms                                                | 66.4 ms: 1.03x faster                                  |
| gunicorn                | 1.12 ms                                                | 1.09 ms: 1.03x faster                                  |
| xml_etree_iterparse     | 103 ms                                                 | 100 ms: 1.03x faster                                   |
| telco                   | 6.62 ms                                                | 6.46 ms: 1.03x faster                                  |
| bench_thread_pool       | 810 us                                                 | 790 us: 1.03x faster                                   |
| docutils                | 2.60 sec                                               | 2.54 sec: 1.02x faster                                 |
| nbody                   | 95.0 ms                                                | 92.9 ms: 1.02x faster                                  |
| logging_format          | 6.62 us                                                | 6.47 us: 1.02x faster                                  |
| meteor_contest          | 105 ms                                                 | 102 ms: 1.02x faster                                   |
| raytrace                | 290 ms                                                 | 285 ms: 1.02x faster                                   |
| unpack_sequence         | 43.4 ns                                                | 42.7 ns: 1.02x faster                                  |
| tornado_http            | 96.6 ms                                                | 95.2 ms: 1.02x faster                                  |
| dulwich_log             | 63.9 ms                                                | 62.9 ms: 1.02x faster                                  |
| regex_v8                | 22.3 ms                                                | 22.0 ms: 1.01x faster                                  |
| pprint_safe_repr        | 691 ms                                                 | 682 ms: 1.01x faster                                   |
| sqlalchemy_declarative  | 139 ms                                                 | 137 ms: 1.01x faster                                   |
| crypto_pyaes            | 73.9 ms                                                | 73.2 ms: 1.01x faster                                  |
| regex_effbot            | 3.36 ms                                                | 3.38 ms: 1.01x slower                                  |
| mako                    | 9.85 ms                                                | 9.92 ms: 1.01x slower                                  |
| pathlib                 | 18.2 ms                                                | 18.3 ms: 1.01x slower                                  |
| async_tree_io           | 1.31 sec                                               | 1.32 sec: 1.01x slower                                 |
| chameleon               | 6.41 ms                                                | 6.49 ms: 1.01x slower                                  |
| thrift                  | 752 us                                                 | 766 us: 1.02x slower                                   |
| unpickle_list           | 4.95 us                                                | 5.06 us: 1.02x slower                                  |
| pickle_list             | 4.17 us                                                | 4.29 us: 1.03x slower                                  |
| xml_etree_process       | 53.8 ms                                                | 55.4 ms: 1.03x slower                                  |
| pickle                  | 9.79 us                                                | 10.1 us: 1.03x slower                                  |
| pickle_dict             | 31.4 us                                                | 32.5 us: 1.04x slower                                  |
| async_tree_memoization  | 625 ms                                                 | 649 ms: 1.04x slower                                   |
| sqlite_synth            | 2.49 us                                                | 2.59 us: 1.04x slower                                  |
| sqlglot_transpile       | 1.66 ms                                                | 1.73 ms: 1.04x slower                                  |
| django_template         | 32.5 ms                                                | 34.0 ms: 1.05x slower                                  |
| sqlglot_parse           | 1.37 ms                                                | 1.44 ms: 1.05x slower                                  |
| xml_etree_generate      | 76.2 ms                                                | 81.2 ms: 1.06x slower                                  |
| python_startup          | 8.36 ms                                                | 9.00 ms: 1.08x slower                                  |
| regex_dna               | 203 ms                                                 | 220 ms: 1.08x slower                                   |
| python_startup_no_site  | 5.96 ms                                                | 6.52 ms: 1.09x slower                                  |
| async_generators        | 359 ms                                                 | 411 ms: 1.14x slower                                   |
| Geometric mean          | (ref)                                                  | 1.03x faster                                           |

Benchmark hidden because not significant (7): scimark_lu, async_tree_none, async_tree_cpu_io_mixed, deepcopy_reduce, bench_mp_pool, sqlalchemy_imperative, unpickle
Ignored benchmarks (3) of public/results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, mypy, pylint
Ignored benchmarks (6) of public/results/bm-20230218-3.12.0a5+-61f1e67/bm-20230218-linux-x86_64-python-main-3.12.0a5+-61f1e67.json: asyncio_tcp, create_gc_cycles, dask, djangocms, gc_traversal, mypy2
