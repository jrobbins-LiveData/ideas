Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509 | bm-20221024-darwin-arm64-python-dfb5d272e6b99c2c70c6-3.12.0a0-dfb5d27 |
|----------------|:-------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 181 ms                                                              | 185 ms: 1.02x slower                                                  |
| docutils       | 1.46 sec                                                            | 1.47 sec: 1.01x slower                                                |
| html5lib       | 34.7 ms                                                             | 36.5 ms: 1.05x slower                                                 |
| Geometric mean | (ref)                                                               | 1.02x slower                                                          |

Benchmark hidden because not significant (2): chameleon, tornado_http

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509 | bm-20221024-darwin-arm64-python-dfb5d272e6b99c2c70c6-3.12.0a0-dfb5d27 |
|----------------|:-------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 51.7 ms                                                             | 56.2 ms: 1.09x slower                                                 |
| nbody          | 65.2 ms                                                             | 64.6 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                               | 1.03x slower                                                          |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509 | bm-20221024-darwin-arm64-python-dfb5d272e6b99c2c70c6-3.12.0a0-dfb5d27 |
|----------------|:-------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 76.3 ms                                                             | 76.1 ms: 1.00x faster                                                 |
| regex_dna      | 151 ms                                                              | 152 ms: 1.01x slower                                                  |
| regex_effbot   | 2.63 ms                                                             | 2.74 ms: 1.04x slower                                                 |
| regex_v8       | 16.5 ms                                                             | 16.4 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                               | 1.01x slower                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509 | bm-20221024-darwin-arm64-python-dfb5d272e6b99c2c70c6-3.12.0a0-dfb5d27 |
|----------------------|:-------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 7.67 ms                                                             | 6.13 ms: 1.25x faster                                                 |
| json_loads           | 16.1 us                                                             | 16.2 us: 1.00x slower                                                 |
| pickle               | 7.21 us                                                             | 7.54 us: 1.05x slower                                                 |
| pickle_dict          | 17.9 us                                                             | 18.0 us: 1.01x slower                                                 |
| pickle_list          | 2.86 us                                                             | 2.88 us: 1.01x slower                                                 |
| pickle_pure_python   | 200 us                                                              | 208 us: 1.04x slower                                                  |
| unpickle_list        | 2.64 us                                                             | 2.53 us: 1.04x faster                                                 |
| unpickle_pure_python | 159 us                                                              | 162 us: 1.02x slower                                                  |
| xml_etree_parse      | 99.6 ms                                                             | 91.0 ms: 1.09x faster                                                 |
| xml_etree_iterparse  | 65.6 ms                                                             | 64.9 ms: 1.01x faster                                                 |
| xml_etree_generate   | 48.4 ms                                                             | 47.3 ms: 1.02x faster                                                 |
| xml_etree_process    | 35.1 ms                                                             | 34.9 ms: 1.01x faster                                                 |
| Geometric mean       | (ref)                                                               | 1.02x faster                                                          |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509 | bm-20221024-darwin-arm64-python-dfb5d272e6b99c2c70c6-3.12.0a0-dfb5d27 |
|------------------------|:-------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 7.24 ms                                                             | 7.21 ms: 1.00x faster                                                 |
| Geometric mean         | (ref)                                                               | 1.00x faster                                                          |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509 | bm-20221024-darwin-arm64-python-dfb5d272e6b99c2c70c6-3.12.0a0-dfb5d27 |
|-----------------|:-------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 21.1 ms                                                             | 21.7 ms: 1.03x slower                                                 |
| genshi_xml      | 30.5 ms                                                             | 30.2 ms: 1.01x faster                                                 |
| mako            | 8.40 ms                                                             | 8.13 ms: 1.03x faster                                                 |
| Geometric mean  | (ref)                                                               | 1.00x faster                                                          |

Benchmark hidden because not significant (1): genshi_text

All benchmarks:
===============

| Benchmark               | bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509 | bm-20221024-darwin-arm64-python-dfb5d272e6b99c2c70c6-3.12.0a0-dfb5d27 |
|-------------------------|:-------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3                    | 181 ms                                                              | 185 ms: 1.02x slower                                                  |
| async_generators        | 195 ms                                                              | 199 ms: 1.02x slower                                                  |
| async_tree_none         | 281 ms                                                              | 287 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed | 528 ms                                                              | 544 ms: 1.03x slower                                                  |
| async_tree_io           | 696 ms                                                              | 736 ms: 1.06x slower                                                  |
| async_tree_memoization  | 317 ms                                                              | 325 ms: 1.03x slower                                                  |
| chaos                   | 49.3 ms                                                             | 50.3 ms: 1.02x slower                                                 |
| bench_thread_pool       | 457 us                                                              | 452 us: 1.01x faster                                                  |
| coroutines              | 17.8 ms                                                             | 18.9 ms: 1.07x slower                                                 |
| coverage                | 58.4 ms                                                             | 53.1 ms: 1.10x faster                                                 |
| crypto_pyaes            | 51.7 ms                                                             | 51.3 ms: 1.01x faster                                                 |
| deepcopy                | 222 us                                                              | 239 us: 1.08x slower                                                  |
| deepcopy_reduce         | 1.90 us                                                             | 2.05 us: 1.08x slower                                                 |
| deepcopy_memo           | 26.2 us                                                             | 29.0 us: 1.11x slower                                                 |
| deltablue               | 2.82 ms                                                             | 2.74 ms: 1.03x faster                                                 |
| django_template         | 21.1 ms                                                             | 21.7 ms: 1.03x slower                                                 |
| docutils                | 1.46 sec                                                            | 1.47 sec: 1.01x slower                                                |
| dulwich_log             | 29.1 ms                                                             | 29.4 ms: 1.01x slower                                                 |
| fannkuch                | 262 ms                                                              | 268 ms: 1.02x slower                                                  |
| float                   | 51.7 ms                                                             | 56.2 ms: 1.09x slower                                                 |
| generators              | 28.4 ms                                                             | 29.3 ms: 1.03x slower                                                 |
| genshi_xml              | 30.5 ms                                                             | 30.2 ms: 1.01x faster                                                 |
| go                      | 109 ms                                                              | 119 ms: 1.09x slower                                                  |
| hexiom                  | 4.73 ms                                                             | 4.92 ms: 1.04x slower                                                 |
| html5lib                | 34.7 ms                                                             | 36.5 ms: 1.05x slower                                                 |
| json_dumps              | 7.67 ms                                                             | 6.13 ms: 1.25x faster                                                 |
| json_loads              | 16.1 us                                                             | 16.2 us: 1.00x slower                                                 |
| logging_format          | 3.73 us                                                             | 3.97 us: 1.06x slower                                                 |
| logging_silent          | 67.4 ns                                                             | 65.8 ns: 1.02x faster                                                 |
| logging_simple          | 3.47 us                                                             | 3.66 us: 1.06x slower                                                 |
| mako                    | 8.40 ms                                                             | 8.13 ms: 1.03x faster                                                 |
| mdp                     | 1.54 sec                                                            | 1.52 sec: 1.01x faster                                                |
| meteor_contest          | 73.9 ms                                                             | 76.8 ms: 1.04x slower                                                 |
| nbody                   | 65.2 ms                                                             | 64.6 ms: 1.01x faster                                                 |
| nqueens                 | 59.5 ms                                                             | 60.3 ms: 1.01x slower                                                 |
| pickle                  | 7.21 us                                                             | 7.54 us: 1.05x slower                                                 |
| pickle_dict             | 17.9 us                                                             | 18.0 us: 1.01x slower                                                 |
| pickle_list             | 2.86 us                                                             | 2.88 us: 1.01x slower                                                 |
| pickle_pure_python      | 200 us                                                              | 208 us: 1.04x slower                                                  |
| pprint_safe_repr        | 467 ms                                                              | 488 ms: 1.04x slower                                                  |
| pprint_pformat          | 953 ms                                                              | 996 ms: 1.05x slower                                                  |
| pycparser               | 694 ms                                                              | 703 ms: 1.01x slower                                                  |
| pyflate                 | 313 ms                                                              | 355 ms: 1.14x slower                                                  |
| python_startup_no_site  | 7.24 ms                                                             | 7.21 ms: 1.00x faster                                                 |
| raytrace                | 207 ms                                                              | 227 ms: 1.10x slower                                                  |
| regex_compile           | 76.3 ms                                                             | 76.1 ms: 1.00x faster                                                 |
| regex_dna               | 151 ms                                                              | 152 ms: 1.01x slower                                                  |
| regex_effbot            | 2.63 ms                                                             | 2.74 ms: 1.04x slower                                                 |
| regex_v8                | 16.5 ms                                                             | 16.4 ms: 1.01x faster                                                 |
| richards                | 32.7 ms                                                             | 33.5 ms: 1.03x slower                                                 |
| scimark_fft             | 201 ms                                                              | 196 ms: 1.02x faster                                                  |
| scimark_lu              | 72.2 ms                                                             | 71.9 ms: 1.00x faster                                                 |
| scimark_monte_carlo     | 46.9 ms                                                             | 55.4 ms: 1.18x slower                                                 |
| scimark_sor             | 83.3 ms                                                             | 101 ms: 1.21x slower                                                  |
| scimark_sparse_mat_mult | 3.20 ms                                                             | 2.77 ms: 1.16x faster                                                 |
| spectral_norm           | 72.7 ms                                                             | 72.6 ms: 1.00x faster                                                 |
| sqlglot_parse           | 948 us                                                              | 1.00 ms: 1.06x slower                                                 |
| sqlglot_transpile       | 1.11 ms                                                             | 1.17 ms: 1.05x slower                                                 |
| sqlglot_optimize        | 31.3 ms                                                             | 31.8 ms: 1.02x slower                                                 |
| sqlglot_normalize       | 171 ms                                                              | 173 ms: 1.01x slower                                                  |
| sqlite_synth            | 1.29 us                                                             | 1.45 us: 1.12x slower                                                 |
| sympy_expand            | 242 ms                                                              | 247 ms: 1.02x slower                                                  |
| sympy_integrate         | 11.5 ms                                                             | 11.6 ms: 1.01x slower                                                 |
| sympy_sum               | 85.5 ms                                                             | 86.1 ms: 1.01x slower                                                 |
| sympy_str               | 151 ms                                                              | 154 ms: 1.02x slower                                                  |
| telco                   | 3.39 ms                                                             | 3.37 ms: 1.01x faster                                                 |
| thrift                  | 429 us                                                              | 441 us: 1.03x slower                                                  |
| unpack_sequence         | 33.1 ns                                                             | 33.2 ns: 1.00x slower                                                 |
| unpickle_list           | 2.64 us                                                             | 2.53 us: 1.04x faster                                                 |
| unpickle_pure_python    | 159 us                                                              | 162 us: 1.02x slower                                                  |
| xml_etree_parse         | 99.6 ms                                                             | 91.0 ms: 1.09x faster                                                 |
| xml_etree_iterparse     | 65.6 ms                                                             | 64.9 ms: 1.01x faster                                                 |
| xml_etree_generate      | 48.4 ms                                                             | 47.3 ms: 1.02x faster                                                 |
| xml_etree_process       | 35.1 ms                                                             | 34.9 ms: 1.01x faster                                                 |
| Geometric mean          | (ref)                                                               | 1.02x slower                                                          |

Benchmark hidden because not significant (11): chameleon, bench_mp_pool, genshi_text, json, mypy, pathlib, pidigits, pylint, python_startup, tornado_http, unpickle
Ignored benchmarks (5) of ../ideas/results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509.json: aiohttp, flaskblogging, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative
