
# Results vs. 3.10.4

- fork: brandtbucher
- ref: no_superinstructions
- machine: linux-x86_64
- commit hash: b633237
- commit date: 2023-01-14
- overall geometric mean: 1.29x faster \*

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230114-linux-x86_64-brandtbucher-no_superinstructions-3.12.0a4+-b633237 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 332 ms                                                 | 255 ms: 1.30x faster                                                         |
| chameleon      | 8.86 ms                                                | 6.49 ms: 1.37x faster                                                        |
| docutils       | 3.18 sec                                               | 2.50 sec: 1.27x faster                                                       |
| html5lib       | 85.8 ms                                                | 60.6 ms: 1.41x faster                                                        |
| tornado_http   | 128 ms                                                 | 94.9 ms: 1.35x faster                                                        |
| Geometric mean | (ref)                                                  | 1.34x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230114-linux-x86_64-brandtbucher-no_superinstructions-3.12.0a4+-b633237 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 108 ms                                                 | 72.2 ms: 1.49x faster                                                        |
| nbody          | 136 ms                                                 | 94.2 ms: 1.45x faster                                                        |
| pidigits       | 190 ms                                                 | 193 ms: 1.01x slower                                                         |
| Geometric mean | (ref)                                                  | 1.29x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230114-linux-x86_64-brandtbucher-no_superinstructions-3.12.0a4+-b633237 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 174 ms                                                 | 133 ms: 1.31x faster                                                         |
| regex_dna      | 214 ms                                                 | 207 ms: 1.03x faster                                                         |
| regex_effbot   | 3.21 ms                                                | 3.54 ms: 1.10x slower                                                        |
| regex_v8       | 25.0 ms                                                | 21.2 ms: 1.18x faster                                                        |
| Geometric mean | (ref)                                                  | 1.10x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230114-linux-x86_64-brandtbucher-no_superinstructions-3.12.0a4+-b633237 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.5 ms                                                | 9.38 ms: 1.44x faster                                                        |
| json_loads           | 28.9 us                                                | 24.1 us: 1.20x faster                                                        |
| pickle               | 10.1 us                                                | 10.0 us: 1.01x faster                                                        |
| pickle_dict          | 28.3 us                                                | 29.5 us: 1.04x slower                                                        |
| pickle_list          | 4.50 us                                                | 4.02 us: 1.12x faster                                                        |
| pickle_pure_python   | 453 us                                                 | 287 us: 1.58x faster                                                         |
| unpickle             | 14.3 us                                                | 12.9 us: 1.11x faster                                                        |
| unpickle_list        | 4.99 us                                                | 4.91 us: 1.02x faster                                                        |
| unpickle_pure_python | 297 us                                                 | 201 us: 1.48x faster                                                         |
| xml_etree_parse      | 163 ms                                                 | 148 ms: 1.10x faster                                                         |
| xml_etree_iterparse  | 110 ms                                                 | 105 ms: 1.05x faster                                                         |
| xml_etree_generate   | 93.3 ms                                                | 77.0 ms: 1.21x faster                                                        |
| xml_etree_process    | 74.5 ms                                                | 53.7 ms: 1.39x faster                                                        |
| Geometric mean       | (ref)                                                  | 1.19x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230114-linux-x86_64-brandtbucher-no_superinstructions-3.12.0a4+-b633237 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 13.9 ms                                                | 8.74 ms: 1.59x faster                                                        |
| python_startup_no_site | 5.76 ms                                                | 6.30 ms: 1.09x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.21x faster                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230114-linux-x86_64-brandtbucher-no_superinstructions-3.12.0a4+-b633237 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| django_template | 46.3 ms                                                | 32.7 ms: 1.41x faster                                                        |
| genshi_text     | 30.6 ms                                                | 20.5 ms: 1.49x faster                                                        |
| genshi_xml      | 63.6 ms                                                | 47.1 ms: 1.35x faster                                                        |
| mako            | 14.3 ms                                                | 9.89 ms: 1.44x faster                                                        |
| Geometric mean  | (ref)                                                  | 1.42x faster                                                                 |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230114-linux-x86_64-brandtbucher-no_superinstructions-3.12.0a4+-b633237 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3                    | 332 ms                                                 | 255 ms: 1.30x faster                                                         |
| aiohttp                 | 1.34 ms                                                | 1.00 ms: 1.33x faster                                                        |
| async_generators        | 428 ms                                                 | 356 ms: 1.20x faster                                                         |
| async_tree_none         | 713 ms                                                 | 530 ms: 1.34x faster                                                         |
| async_tree_cpu_io_mixed | 949 ms                                                 | 749 ms: 1.27x faster                                                         |
| async_tree_io           | 1.78 sec                                               | 1.32 sec: 1.34x faster                                                       |
| async_tree_memoization  | 854 ms                                                 | 658 ms: 1.30x faster                                                         |
| chameleon               | 8.86 ms                                                | 6.49 ms: 1.37x faster                                                        |
| chaos                   | 104 ms                                                 | 70.4 ms: 1.48x faster                                                        |
| bench_thread_pool       | 943 us                                                 | 784 us: 1.20x faster                                                         |
| coroutines              | 31.7 ms                                                | 25.0 ms: 1.26x faster                                                        |
| coverage                | 75.3 ms                                                | 96.2 ms: 1.28x slower                                                        |
| crypto_pyaes            | 118 ms                                                 | 77.7 ms: 1.51x faster                                                        |
| deepcopy                | 429 us                                                 | 336 us: 1.28x faster                                                         |
| deepcopy_reduce         | 3.75 us                                                | 2.95 us: 1.27x faster                                                        |
| deepcopy_memo           | 50.0 us                                                | 36.1 us: 1.38x faster                                                        |
| deltablue               | 7.39 ms                                                | 3.23 ms: 2.29x faster                                                        |
| django_template         | 46.3 ms                                                | 32.7 ms: 1.41x faster                                                        |
| docutils                | 3.18 sec                                               | 2.50 sec: 1.27x faster                                                       |
| dulwich_log             | 75.5 ms                                                | 62.4 ms: 1.21x faster                                                        |
| fannkuch                | 477 ms                                                 | 374 ms: 1.27x faster                                                         |
| float                   | 108 ms                                                 | 72.2 ms: 1.49x faster                                                        |
| generators              | 75.8 ms                                                | 74.6 ms: 1.02x faster                                                        |
| genshi_text             | 30.6 ms                                                | 20.5 ms: 1.49x faster                                                        |
| genshi_xml              | 63.6 ms                                                | 47.1 ms: 1.35x faster                                                        |
| go                      | 226 ms                                                 | 137 ms: 1.66x faster                                                         |
| gunicorn                | 1.43 ms                                                | 1.08 ms: 1.32x faster                                                        |
| hexiom                  | 9.42 ms                                                | 6.18 ms: 1.52x faster                                                        |
| html5lib                | 85.8 ms                                                | 60.6 ms: 1.41x faster                                                        |
| json                    | 5.35 ms                                                | 4.71 ms: 1.14x faster                                                        |
| json_dumps              | 13.5 ms                                                | 9.38 ms: 1.44x faster                                                        |
| json_loads              | 28.9 us                                                | 24.1 us: 1.20x faster                                                        |
| logging_format          | 8.92 us                                                | 6.52 us: 1.37x faster                                                        |
| logging_silent          | 173 ns                                                 | 91.7 ns: 1.89x faster                                                        |
| logging_simple          | 8.06 us                                                | 5.82 us: 1.38x faster                                                        |
| mako                    | 14.3 ms                                                | 9.89 ms: 1.44x faster                                                        |
| mdp                     | 2.82 sec                                               | 2.61 sec: 1.08x faster                                                       |
| meteor_contest          | 114 ms                                                 | 104 ms: 1.10x faster                                                         |
| mypy                    | 1.01 sec                                               | 821 ms: 1.24x faster                                                         |
| nbody                   | 136 ms                                                 | 94.2 ms: 1.45x faster                                                        |
| nqueens                 | 99.3 ms                                                | 79.4 ms: 1.25x faster                                                        |
| pathlib                 | 20.0 ms                                                | 18.2 ms: 1.10x faster                                                        |
| pickle                  | 10.1 us                                                | 10.0 us: 1.01x faster                                                        |
| pickle_dict             | 28.3 us                                                | 29.5 us: 1.04x slower                                                        |
| pickle_list             | 4.50 us                                                | 4.02 us: 1.12x faster                                                        |
| pickle_pure_python      | 453 us                                                 | 287 us: 1.58x faster                                                         |
| pidigits                | 190 ms                                                 | 193 ms: 1.01x slower                                                         |
| pprint_safe_repr        | 943 ms                                                 | 676 ms: 1.39x faster                                                         |
| pprint_pformat          | 1.97 sec                                               | 1.38 sec: 1.43x faster                                                       |
| pycparser               | 1.51 sec                                               | 1.11 sec: 1.36x faster                                                       |
| pyflate                 | 675 ms                                                 | 398 ms: 1.70x faster                                                         |
| python_startup          | 13.9 ms                                                | 8.74 ms: 1.59x faster                                                        |
| python_startup_no_site  | 5.76 ms                                                | 6.30 ms: 1.09x slower                                                        |
| raytrace                | 461 ms                                                 | 288 ms: 1.60x faster                                                         |
| regex_compile           | 174 ms                                                 | 133 ms: 1.31x faster                                                         |
| regex_dna               | 214 ms                                                 | 207 ms: 1.03x faster                                                         |
| regex_effbot            | 3.21 ms                                                | 3.54 ms: 1.10x slower                                                        |
| regex_v8                | 25.0 ms                                                | 21.2 ms: 1.18x faster                                                        |
| richards                | 71.4 ms                                                | 44.0 ms: 1.62x faster                                                        |
| scimark_fft             | 414 ms                                                 | 317 ms: 1.31x faster                                                         |
| scimark_lu              | 158 ms                                                 | 106 ms: 1.49x faster                                                         |
| scimark_monte_carlo     | 105 ms                                                 | 66.1 ms: 1.58x faster                                                        |
| scimark_sor             | 193 ms                                                 | 107 ms: 1.80x faster                                                         |
| scimark_sparse_mat_mult | 5.48 ms                                                | 4.13 ms: 1.33x faster                                                        |
| spectral_norm           | 148 ms                                                 | 98.0 ms: 1.51x faster                                                        |
| sqlglot_parse           | 2.04 ms                                                | 1.40 ms: 1.45x faster                                                        |
| sqlglot_transpile       | 2.42 ms                                                | 1.70 ms: 1.42x faster                                                        |
| sqlglot_optimize        | 65.3 ms                                                | 51.4 ms: 1.27x faster                                                        |
| sqlglot_normalize       | 135 ms                                                 | 106 ms: 1.28x faster                                                         |
| sqlite_synth            | 2.90 us                                                | 2.58 us: 1.13x faster                                                        |
| sympy_expand            | 537 ms                                                 | 466 ms: 1.15x faster                                                         |
| sympy_integrate         | 23.9 ms                                                | 20.5 ms: 1.17x faster                                                        |
| sympy_sum               | 183 ms                                                 | 165 ms: 1.11x faster                                                         |
| sympy_str               | 324 ms                                                 | 288 ms: 1.13x faster                                                         |
| telco                   | 6.68 ms                                                | 6.43 ms: 1.04x faster                                                        |
| thrift                  | 1.03 ms                                                | 750 us: 1.37x faster                                                         |
| tornado_http            | 128 ms                                                 | 94.9 ms: 1.35x faster                                                        |
| unpack_sequence         | 59.5 ns                                                | 49.0 ns: 1.21x faster                                                        |
| unpickle                | 14.3 us                                                | 12.9 us: 1.11x faster                                                        |
| unpickle_list           | 4.99 us                                                | 4.91 us: 1.02x faster                                                        |
| unpickle_pure_python    | 297 us                                                 | 201 us: 1.48x faster                                                         |
| xml_etree_parse         | 163 ms                                                 | 148 ms: 1.10x faster                                                         |
| xml_etree_iterparse     | 110 ms                                                 | 105 ms: 1.05x faster                                                         |
| xml_etree_generate      | 93.3 ms                                                | 77.0 ms: 1.21x faster                                                        |
| xml_etree_process       | 74.5 ms                                                | 53.7 ms: 1.39x faster                                                        |
| Geometric mean          | (ref)                                                  | 1.29x faster                                                                 |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (4) of public/results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, pylint, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of public/results/bm-20230114-3.12.0a4+-b633237/bm-20230114-linux-x86_64-brandtbucher-no_superinstructions-3.12.0a4+-b633237.json: asyncio_tcp, create_gc_cycles, dask, djangocms, gc_traversal
