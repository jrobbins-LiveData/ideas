
# Results vs. 3.11.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: bb396ee
- commit date: 2023-03-11
- overall geometric mean: 1.03x faster \*

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230311-linux-x86_64-python-main-3.12.0a6+-bb396ee |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 257 ms                                                 | 250 ms: 1.03x faster                                   |
| chameleon      | 6.41 ms                                                | 6.37 ms: 1.01x faster                                  |
| docutils       | 2.60 sec                                               | 2.55 sec: 1.02x faster                                 |
| html5lib       | 63.2 ms                                                | 61.6 ms: 1.03x faster                                  |
| tornado_http   | 96.6 ms                                                | 91.2 ms: 1.06x faster                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230311-linux-x86_64-python-main-3.12.0a6+-bb396ee |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pidigits       | 199 ms                                                 | 192 ms: 1.04x faster                                   |
| nbody          | 95.0 ms                                                | 92.1 ms: 1.03x faster                                  |
| float          | 76.3 ms                                                | 74.1 ms: 1.03x faster                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230311-linux-x86_64-python-main-3.12.0a6+-bb396ee |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_v8       | 22.3 ms                                                | 21.7 ms: 1.03x faster                                  |
| regex_compile  | 136 ms                                                 | 134 ms: 1.02x faster                                   |
| regex_dna      | 203 ms                                                 | 205 ms: 1.01x slower                                   |
| regex_effbot   | 3.36 ms                                                | 3.66 ms: 1.09x slower                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230311-linux-x86_64-python-main-3.12.0a6+-bb396ee |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_dumps           | 12.7 ms                                                | 9.48 ms: 1.34x faster                                  |
| unpickle_pure_python | 225 us                                                 | 201 us: 1.12x faster                                   |
| json_loads           | 26.2 us                                                | 24.0 us: 1.09x faster                                  |
| xml_etree_parse      | 158 ms                                                 | 147 ms: 1.07x faster                                   |
| pickle_pure_python   | 304 us                                                 | 287 us: 1.06x faster                                   |
| xml_etree_iterparse  | 103 ms                                                 | 101 ms: 1.02x faster                                   |
| pickle_dict          | 31.4 us                                                | 31.3 us: 1.00x faster                                  |
| unpickle_list        | 4.95 us                                                | 4.98 us: 1.00x slower                                  |
| pickle_list          | 4.17 us                                                | 4.24 us: 1.02x slower                                  |
| xml_etree_process    | 53.8 ms                                                | 55.8 ms: 1.04x slower                                  |
| xml_etree_generate   | 76.2 ms                                                | 80.6 ms: 1.06x slower                                  |
| pickle               | 9.79 us                                                | 10.4 us: 1.07x slower                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                           |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230311-linux-x86_64-python-main-3.12.0a6+-bb396ee |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 8.36 ms                                                | 8.96 ms: 1.07x slower                                  |
| python_startup_no_site | 5.96 ms                                                | 6.50 ms: 1.09x slower                                  |
| Geometric mean         | (ref)                                                  | 1.08x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230311-linux-x86_64-python-main-3.12.0a6+-bb396ee |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| genshi_xml      | 52.1 ms                                                | 48.2 ms: 1.08x faster                                  |
| genshi_text     | 22.1 ms                                                | 21.8 ms: 1.01x faster                                  |
| django_template | 32.5 ms                                                | 32.9 ms: 1.01x slower                                  |
| mako            | 9.85 ms                                                | 10.1 ms: 1.03x slower                                  |
| Geometric mean  | (ref)                                                  | 1.01x faster                                           |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230311-linux-x86_64-python-main-3.12.0a6+-bb396ee |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| generators              | 72.2 ms                                                | 30.3 ms: 2.38x faster                                  |
| json_dumps              | 12.7 ms                                                | 9.48 ms: 1.34x faster                                  |
| coroutines              | 26.1 ms                                                | 22.7 ms: 1.15x faster                                  |
| deltablue               | 3.64 ms                                                | 3.22 ms: 1.13x faster                                  |
| unpickle_pure_python    | 225 us                                                 | 201 us: 1.12x faster                                   |
| fannkuch                | 388 ms                                                 | 355 ms: 1.09x faster                                   |
| json_loads              | 26.2 us                                                | 24.0 us: 1.09x faster                                  |
| json                    | 4.95 ms                                                | 4.57 ms: 1.08x faster                                  |
| genshi_xml              | 52.1 ms                                                | 48.2 ms: 1.08x faster                                  |
| scimark_sor             | 115 ms                                                 | 107 ms: 1.08x faster                                   |
| richards                | 46.2 ms                                                | 42.9 ms: 1.08x faster                                  |
| xml_etree_parse         | 158 ms                                                 | 147 ms: 1.07x faster                                   |
| spectral_norm           | 99.9 ms                                                | 93.3 ms: 1.07x faster                                  |
| go                      | 143 ms                                                 | 135 ms: 1.06x faster                                   |
| pickle_pure_python      | 304 us                                                 | 287 us: 1.06x faster                                   |
| tornado_http            | 96.6 ms                                                | 91.2 ms: 1.06x faster                                  |
| logging_simple          | 6.06 us                                                | 5.77 us: 1.05x faster                                  |
| scimark_fft             | 329 ms                                                 | 313 ms: 1.05x faster                                   |
| unpack_sequence         | 43.4 ns                                                | 41.3 ns: 1.05x faster                                  |
| deepcopy_memo           | 36.4 us                                                | 34.8 us: 1.05x faster                                  |
| pycparser               | 1.17 sec                                               | 1.13 sec: 1.04x faster                                 |
| logging_format          | 6.62 us                                                | 6.36 us: 1.04x faster                                  |
| sqlglot_optimize        | 53.0 ms                                                | 51.0 ms: 1.04x faster                                  |
| pprint_pformat          | 1.44 sec                                               | 1.39 sec: 1.04x faster                                 |
| aiohttp                 | 1.05 ms                                                | 1.01 ms: 1.04x faster                                  |
| pidigits                | 199 ms                                                 | 192 ms: 1.04x faster                                   |
| pyflate                 | 417 ms                                                 | 403 ms: 1.03x faster                                   |
| logging_silent          | 98.5 ns                                                | 95.2 ns: 1.03x faster                                  |
| gunicorn                | 1.12 ms                                                | 1.09 ms: 1.03x faster                                  |
| coverage                | 101 ms                                                 | 97.3 ms: 1.03x faster                                  |
| nbody                   | 95.0 ms                                                | 92.1 ms: 1.03x faster                                  |
| float                   | 76.3 ms                                                | 74.1 ms: 1.03x faster                                  |
| hexiom                  | 6.35 ms                                                | 6.17 ms: 1.03x faster                                  |
| mdp                     | 2.62 sec                                               | 2.55 sec: 1.03x faster                                 |
| 2to3                    | 257 ms                                                 | 250 ms: 1.03x faster                                   |
| scimark_monte_carlo     | 68.3 ms                                                | 66.5 ms: 1.03x faster                                  |
| regex_v8                | 22.3 ms                                                | 21.7 ms: 1.03x faster                                  |
| sqlglot_normalize       | 108 ms                                                 | 105 ms: 1.03x faster                                   |
| bench_thread_pool       | 810 us                                                 | 789 us: 1.03x faster                                   |
| html5lib                | 63.2 ms                                                | 61.6 ms: 1.03x faster                                  |
| pathlib                 | 18.2 ms                                                | 17.7 ms: 1.02x faster                                  |
| sympy_expand            | 472 ms                                                 | 461 ms: 1.02x faster                                   |
| deepcopy                | 344 us                                                 | 336 us: 1.02x faster                                   |
| raytrace                | 290 ms                                                 | 284 ms: 1.02x faster                                   |
| telco                   | 6.62 ms                                                | 6.49 ms: 1.02x faster                                  |
| nqueens                 | 85.0 ms                                                | 83.3 ms: 1.02x faster                                  |
| sqlalchemy_imperative   | 18.0 ms                                                | 17.7 ms: 1.02x faster                                  |
| async_tree_io           | 1.31 sec                                               | 1.28 sec: 1.02x faster                                 |
| async_tree_cpu_io_mixed | 752 ms                                                 | 738 ms: 1.02x faster                                   |
| sympy_integrate         | 20.9 ms                                                | 20.5 ms: 1.02x faster                                  |
| async_tree_none         | 529 ms                                                 | 520 ms: 1.02x faster                                   |
| docutils                | 2.60 sec                                               | 2.55 sec: 1.02x faster                                 |
| xml_etree_iterparse     | 103 ms                                                 | 101 ms: 1.02x faster                                   |
| pprint_safe_repr        | 691 ms                                                 | 680 ms: 1.02x faster                                   |
| regex_compile           | 136 ms                                                 | 134 ms: 1.02x faster                                   |
| genshi_text             | 22.1 ms                                                | 21.8 ms: 1.01x faster                                  |
| chaos                   | 68.6 ms                                                | 67.8 ms: 1.01x faster                                  |
| sympy_str               | 287 ms                                                 | 284 ms: 1.01x faster                                   |
| chameleon               | 6.41 ms                                                | 6.37 ms: 1.01x faster                                  |
| pickle_dict             | 31.4 us                                                | 31.3 us: 1.00x faster                                  |
| dulwich_log             | 63.9 ms                                                | 63.7 ms: 1.00x faster                                  |
| sympy_sum               | 166 ms                                                 | 167 ms: 1.00x slower                                   |
| unpickle_list           | 4.95 us                                                | 4.98 us: 1.00x slower                                  |
| sqlalchemy_declarative  | 139 ms                                                 | 140 ms: 1.01x slower                                   |
| deepcopy_reduce         | 2.97 us                                                | 3.00 us: 1.01x slower                                  |
| regex_dna               | 203 ms                                                 | 205 ms: 1.01x slower                                   |
| meteor_contest          | 105 ms                                                 | 106 ms: 1.01x slower                                   |
| django_template         | 32.5 ms                                                | 32.9 ms: 1.01x slower                                  |
| pickle_list             | 4.17 us                                                | 4.24 us: 1.02x slower                                  |
| mako                    | 9.85 ms                                                | 10.1 ms: 1.03x slower                                  |
| sqlglot_transpile       | 1.66 ms                                                | 1.72 ms: 1.04x slower                                  |
| sqlglot_parse           | 1.37 ms                                                | 1.42 ms: 1.04x slower                                  |
| xml_etree_process       | 53.8 ms                                                | 55.8 ms: 1.04x slower                                  |
| async_tree_memoization  | 625 ms                                                 | 649 ms: 1.04x slower                                   |
| thrift                  | 752 us                                                 | 782 us: 1.04x slower                                   |
| scimark_sparse_mat_mult | 4.40 ms                                                | 4.59 ms: 1.04x slower                                  |
| sqlite_synth            | 2.49 us                                                | 2.63 us: 1.06x slower                                  |
| xml_etree_generate      | 76.2 ms                                                | 80.6 ms: 1.06x slower                                  |
| scimark_lu              | 107 ms                                                 | 114 ms: 1.06x slower                                   |
| pickle                  | 9.79 us                                                | 10.4 us: 1.07x slower                                  |
| python_startup          | 8.36 ms                                                | 8.96 ms: 1.07x slower                                  |
| python_startup_no_site  | 5.96 ms                                                | 6.50 ms: 1.09x slower                                  |
| regex_effbot            | 3.36 ms                                                | 3.66 ms: 1.09x slower                                  |
| async_generators        | 359 ms                                                 | 415 ms: 1.16x slower                                   |
| Geometric mean          | (ref)                                                  | 1.03x faster                                           |

Benchmark hidden because not significant (3): bench_mp_pool, crypto_pyaes, unpickle
Ignored benchmarks (3) of public/results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, mypy, pylint
Ignored benchmarks (7) of public/results/bm-20230311-3.12.0a6+-bb396ee/bm-20230311-linux-x86_64-python-main-3.12.0a6+-bb396ee.json: asyncio_tcp, comprehensions, create_gc_cycles, dask, djangocms, gc_traversal, mypy2