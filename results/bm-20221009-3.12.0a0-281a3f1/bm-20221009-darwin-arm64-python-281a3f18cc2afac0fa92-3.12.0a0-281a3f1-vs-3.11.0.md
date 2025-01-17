Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509 | bm-20221009-darwin-arm64-python-281a3f18cc2afac0fa92-3.12.0a0-281a3f1 |
|----------------|:-------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 181 ms                                                              | 186 ms: 1.02x slower                                                  |
| docutils       | 1.46 sec                                                            | 1.47 sec: 1.01x slower                                                |
| html5lib       | 34.7 ms                                                             | 36.6 ms: 1.06x slower                                                 |
| Geometric mean | (ref)                                                               | 1.01x slower                                                          |

Benchmark hidden because not significant (2): chameleon, tornado_http

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509 | bm-20221009-darwin-arm64-python-281a3f18cc2afac0fa92-3.12.0a0-281a3f1 |
|----------------|:-------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 51.7 ms                                                             | 56.1 ms: 1.09x slower                                                 |
| nbody          | 65.2 ms                                                             | 64.3 ms: 1.02x faster                                                 |
| Geometric mean | (ref)                                                               | 1.02x slower                                                          |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509 | bm-20221009-darwin-arm64-python-281a3f18cc2afac0fa92-3.12.0a0-281a3f1 |
|----------------|:-------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 76.3 ms                                                             | 76.5 ms: 1.00x slower                                                 |
| regex_effbot   | 2.63 ms                                                             | 2.68 ms: 1.02x slower                                                 |
| regex_v8       | 16.5 ms                                                             | 16.3 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                               | 1.00x slower                                                          |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509 | bm-20221009-darwin-arm64-python-281a3f18cc2afac0fa92-3.12.0a0-281a3f1 |
|----------------------|:-------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 7.67 ms                                                             | 6.17 ms: 1.24x faster                                                 |
| json_loads           | 16.1 us                                                             | 16.3 us: 1.01x slower                                                 |
| pickle               | 7.21 us                                                             | 7.56 us: 1.05x slower                                                 |
| pickle_dict          | 17.9 us                                                             | 18.0 us: 1.01x slower                                                 |
| pickle_list          | 2.86 us                                                             | 2.91 us: 1.02x slower                                                 |
| pickle_pure_python   | 200 us                                                              | 208 us: 1.04x slower                                                  |
| unpickle             | 9.68 us                                                             | 9.78 us: 1.01x slower                                                 |
| unpickle_list        | 2.64 us                                                             | 2.54 us: 1.04x faster                                                 |
| unpickle_pure_python | 159 us                                                              | 162 us: 1.02x slower                                                  |
| xml_etree_parse      | 99.6 ms                                                             | 90.0 ms: 1.11x faster                                                 |
| xml_etree_iterparse  | 65.6 ms                                                             | 64.6 ms: 1.01x faster                                                 |
| xml_etree_generate   | 48.4 ms                                                             | 47.1 ms: 1.03x faster                                                 |
| xml_etree_process    | 35.1 ms                                                             | 34.9 ms: 1.01x faster                                                 |
| Geometric mean       | (ref)                                                               | 1.02x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509 | bm-20221009-darwin-arm64-python-281a3f18cc2afac0fa92-3.12.0a0-281a3f1 |
|------------------------|:-------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 9.19 ms                                                             | 9.38 ms: 1.02x slower                                                 |
| python_startup_no_site | 7.24 ms                                                             | 7.41 ms: 1.02x slower                                                 |
| Geometric mean         | (ref)                                                               | 1.02x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509 | bm-20221009-darwin-arm64-python-281a3f18cc2afac0fa92-3.12.0a0-281a3f1 |
|-----------------|:-------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 21.1 ms                                                             | 21.7 ms: 1.03x slower                                                 |
| genshi_xml      | 30.5 ms                                                             | 30.1 ms: 1.01x faster                                                 |
| mako            | 8.40 ms                                                             | 8.11 ms: 1.04x faster                                                 |
| Geometric mean  | (ref)                                                               | 1.00x faster                                                          |

Benchmark hidden because not significant (1): genshi_text

All benchmarks:
===============

| Benchmark               | bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509 | bm-20221009-darwin-arm64-python-281a3f18cc2afac0fa92-3.12.0a0-281a3f1 |
|-------------------------|:-------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3                    | 181 ms                                                              | 186 ms: 1.02x slower                                                  |
| async_generators        | 195 ms                                                              | 199 ms: 1.02x slower                                                  |
| async_tree_none         | 281 ms                                                              | 287 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed | 528 ms                                                              | 545 ms: 1.03x slower                                                  |
| async_tree_io           | 696 ms                                                              | 736 ms: 1.06x slower                                                  |
| async_tree_memoization  | 317 ms                                                              | 325 ms: 1.03x slower                                                  |
| chaos                   | 49.3 ms                                                             | 50.4 ms: 1.02x slower                                                 |
| bench_thread_pool       | 457 us                                                              | 452 us: 1.01x faster                                                  |
| coroutines              | 17.8 ms                                                             | 19.0 ms: 1.07x slower                                                 |
| coverage                | 58.4 ms                                                             | 53.4 ms: 1.09x faster                                                 |
| crypto_pyaes            | 51.7 ms                                                             | 51.8 ms: 1.00x slower                                                 |
| deepcopy                | 222 us                                                              | 239 us: 1.08x slower                                                  |
| deepcopy_reduce         | 1.90 us                                                             | 2.06 us: 1.09x slower                                                 |
| deepcopy_memo           | 26.2 us                                                             | 29.2 us: 1.12x slower                                                 |
| deltablue               | 2.82 ms                                                             | 2.74 ms: 1.03x faster                                                 |
| django_template         | 21.1 ms                                                             | 21.7 ms: 1.03x slower                                                 |
| docutils                | 1.46 sec                                                            | 1.47 sec: 1.01x slower                                                |
| dulwich_log             | 29.1 ms                                                             | 29.3 ms: 1.01x slower                                                 |
| fannkuch                | 262 ms                                                              | 269 ms: 1.03x slower                                                  |
| float                   | 51.7 ms                                                             | 56.1 ms: 1.09x slower                                                 |
| generators              | 28.4 ms                                                             | 29.0 ms: 1.02x slower                                                 |
| genshi_xml              | 30.5 ms                                                             | 30.1 ms: 1.01x faster                                                 |
| go                      | 109 ms                                                              | 120 ms: 1.09x slower                                                  |
| hexiom                  | 4.73 ms                                                             | 4.92 ms: 1.04x slower                                                 |
| html5lib                | 34.7 ms                                                             | 36.6 ms: 1.06x slower                                                 |
| json                    | 2.83 ms                                                             | 2.84 ms: 1.01x slower                                                 |
| json_dumps              | 7.67 ms                                                             | 6.17 ms: 1.24x faster                                                 |
| json_loads              | 16.1 us                                                             | 16.3 us: 1.01x slower                                                 |
| logging_format          | 3.73 us                                                             | 4.00 us: 1.07x slower                                                 |
| logging_silent          | 67.4 ns                                                             | 65.9 ns: 1.02x faster                                                 |
| logging_simple          | 3.47 us                                                             | 3.66 us: 1.06x slower                                                 |
| mako                    | 8.40 ms                                                             | 8.11 ms: 1.04x faster                                                 |
| mdp                     | 1.54 sec                                                            | 1.52 sec: 1.01x faster                                                |
| meteor_contest          | 73.9 ms                                                             | 76.2 ms: 1.03x slower                                                 |
| nbody                   | 65.2 ms                                                             | 64.3 ms: 1.02x faster                                                 |
| nqueens                 | 59.5 ms                                                             | 60.3 ms: 1.01x slower                                                 |
| pickle                  | 7.21 us                                                             | 7.56 us: 1.05x slower                                                 |
| pickle_dict             | 17.9 us                                                             | 18.0 us: 1.01x slower                                                 |
| pickle_list             | 2.86 us                                                             | 2.91 us: 1.02x slower                                                 |
| pickle_pure_python      | 200 us                                                              | 208 us: 1.04x slower                                                  |
| pprint_safe_repr        | 467 ms                                                              | 486 ms: 1.04x slower                                                  |
| pprint_pformat          | 953 ms                                                              | 992 ms: 1.04x slower                                                  |
| pycparser               | 694 ms                                                              | 706 ms: 1.02x slower                                                  |
| pyflate                 | 313 ms                                                              | 352 ms: 1.12x slower                                                  |
| python_startup          | 9.19 ms                                                             | 9.38 ms: 1.02x slower                                                 |
| python_startup_no_site  | 7.24 ms                                                             | 7.41 ms: 1.02x slower                                                 |
| raytrace                | 207 ms                                                              | 219 ms: 1.06x slower                                                  |
| regex_compile           | 76.3 ms                                                             | 76.5 ms: 1.00x slower                                                 |
| regex_effbot            | 2.63 ms                                                             | 2.68 ms: 1.02x slower                                                 |
| regex_v8                | 16.5 ms                                                             | 16.3 ms: 1.01x faster                                                 |
| richards                | 32.7 ms                                                             | 33.5 ms: 1.02x slower                                                 |
| scimark_fft             | 201 ms                                                              | 198 ms: 1.01x faster                                                  |
| scimark_lu              | 72.2 ms                                                             | 73.9 ms: 1.02x slower                                                 |
| scimark_monte_carlo     | 46.9 ms                                                             | 54.6 ms: 1.16x slower                                                 |
| scimark_sor             | 83.3 ms                                                             | 101 ms: 1.22x slower                                                  |
| scimark_sparse_mat_mult | 3.20 ms                                                             | 2.78 ms: 1.15x faster                                                 |
| spectral_norm           | 72.7 ms                                                             | 72.5 ms: 1.00x faster                                                 |
| sqlalchemy_declarative  | 62.4 ms                                                             | 61.0 ms: 1.02x faster                                                 |
| sqlalchemy_imperative   | 7.22 ms                                                             | 7.16 ms: 1.01x faster                                                 |
| sqlglot_parse           | 948 us                                                              | 1.01 ms: 1.06x slower                                                 |
| sqlglot_transpile       | 1.11 ms                                                             | 1.18 ms: 1.06x slower                                                 |
| sqlglot_optimize        | 31.3 ms                                                             | 31.7 ms: 1.01x slower                                                 |
| sqlglot_normalize       | 171 ms                                                              | 173 ms: 1.01x slower                                                  |
| sqlite_synth            | 1.29 us                                                             | 1.45 us: 1.12x slower                                                 |
| sympy_expand            | 242 ms                                                              | 246 ms: 1.01x slower                                                  |
| sympy_integrate         | 11.5 ms                                                             | 11.6 ms: 1.01x slower                                                 |
| sympy_sum               | 85.5 ms                                                             | 86.0 ms: 1.01x slower                                                 |
| sympy_str               | 151 ms                                                              | 153 ms: 1.01x slower                                                  |
| telco                   | 3.39 ms                                                             | 3.32 ms: 1.02x faster                                                 |
| thrift                  | 429 us                                                              | 438 us: 1.02x slower                                                  |
| unpack_sequence         | 33.1 ns                                                             | 33.5 ns: 1.01x slower                                                 |
| unpickle                | 9.68 us                                                             | 9.78 us: 1.01x slower                                                 |
| unpickle_list           | 2.64 us                                                             | 2.54 us: 1.04x faster                                                 |
| unpickle_pure_python    | 159 us                                                              | 162 us: 1.02x slower                                                  |
| xml_etree_parse         | 99.6 ms                                                             | 90.0 ms: 1.11x faster                                                 |
| xml_etree_iterparse     | 65.6 ms                                                             | 64.6 ms: 1.01x faster                                                 |
| xml_etree_generate      | 48.4 ms                                                             | 47.1 ms: 1.03x faster                                                 |
| xml_etree_process       | 35.1 ms                                                             | 34.9 ms: 1.01x faster                                                 |
| Geometric mean          | (ref)                                                               | 1.02x slower                                                          |

Benchmark hidden because not significant (9): chameleon, bench_mp_pool, genshi_text, mypy, pathlib, pidigits, pylint, regex_dna, tornado_http
Ignored benchmarks (3) of ../ideas/results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509.json: aiohttp, flaskblogging, gunicorn
