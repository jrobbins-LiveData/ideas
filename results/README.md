# Benchmark results

<!-- START table -->
## linux x86_64
| date | fork | ref | version | hash | vs. 3.10.4: | vs. 3.11.0: | vs. base: |
| --- | --- | --- | --- | --- | ---: | ---: | ---: |
| [2022-03-23](bm-20220323-3.10.4-9d38120) | python | v3.10.4 | 3.10.4 | 9d38120 |  | [1.26x slower](bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120-vs-3.11.0.md) |  |
| [2022-12-06](bm-20221206-3.10.9-1dd9be6) | python | 1dd9be6584 | 3.10.9 | 1dd9be6 | [1.00x slower](bm-20221206-3.10.9-1dd9be6/bm-20221206-linux-x86_64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.10.4.md) | [1.26x slower](bm-20221206-3.10.9-1dd9be6/bm-20221206-linux-x86_64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.11.0.md) |  |
| [2021-10-05](bm-20211005-3.11.0a1-7c12e48) | python | 7c12e4835e | 3.11.0a1 | 7c12e48 | [1.12x faster](bm-20211005-3.11.0a1-7c12e48/bm-20211005-linux-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.10.4.md) | [1.12x slower](bm-20211005-3.11.0a1-7c12e48/bm-20211005-linux-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48-vs-3.11.0.md) |  |
| [2021-11-05](bm-20211105-3.11.0a2-e2b4e4b) | python | e2b4e4bab9 | 3.11.0a2 | e2b4e4b | [1.15x faster](bm-20211105-3.11.0a2-e2b4e4b/bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.10.4.md) | [1.09x slower](bm-20211105-3.11.0a2-e2b4e4b/bm-20211105-linux-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.11.0.md) |  |
| [2021-12-08](bm-20211208-3.11.0a3-2e91dba) | python | main | 3.11.0a3 | 2e91dba | [1.20x faster \*](bm-20211208-3.11.0a3-2e91dba/bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba-vs-3.10.4.md) | [1.06x slower \*](bm-20211208-3.11.0a3-2e91dba/bm-20211208-linux-x86_64-python-main-3.11.0a3-2e91dba-vs-3.11.0.md) |  |
| [2022-01-13](bm-20220113-3.11.0a4-9471106) | python | main | 3.11.0a4 | 9471106 | [1.22x faster \*](bm-20220113-3.11.0a4-9471106/bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106-vs-3.10.4.md) | [1.04x slower \*](bm-20220113-3.11.0a4-9471106/bm-20220113-linux-x86_64-python-main-3.11.0a4-9471106-vs-3.11.0.md) |  |
| [2022-02-03](bm-20220203-3.11.0a5-c4e4b91) | python | main | 3.11.0a5 | c4e4b91 | [1.22x faster \*](bm-20220203-3.11.0a5-c4e4b91/bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91-vs-3.10.4.md) | [1.04x slower \*](bm-20220203-3.11.0a5-c4e4b91/bm-20220203-linux-x86_64-python-main-3.11.0a5-c4e4b91-vs-3.11.0.md) |  |
| [2022-03-07](bm-20220307-3.11.0a6-3ddfa55) | python | main | 3.11.0a6 | 3ddfa55 | [1.20x faster \*](bm-20220307-3.11.0a6-3ddfa55/bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55-vs-3.10.4.md) | [1.06x slower \*](bm-20220307-3.11.0a6-3ddfa55/bm-20220307-linux-x86_64-python-main-3.11.0a6-3ddfa55-vs-3.11.0.md) |  |
| [2022-04-05](bm-20220405-3.11.0a7-2e49bd0) | python | main | 3.11.0a7 | 2e49bd0 | [1.24x faster \*](bm-20220405-3.11.0a7-2e49bd0/bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0-vs-3.10.4.md) | [1.02x slower \*](bm-20220405-3.11.0a7-2e49bd0/bm-20220405-linux-x86_64-python-main-3.11.0a7-2e49bd0-vs-3.11.0.md) |  |
| [2022-05-06](bm-20220506-3.11.0b1-8d32a5c) | python | main | 3.11.0b1 | 8d32a5c | [1.29x faster \*](bm-20220506-3.11.0b1-8d32a5c/bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c-vs-3.10.4.md) | [1.01x faster \*](bm-20220506-3.11.0b1-8d32a5c/bm-20220506-linux-x86_64-python-main-3.11.0b1-8d32a5c-vs-3.11.0.md) |  |
| [2022-05-30](bm-20220530-3.11.0b2-72f00f4) | python | main | 3.11.0b2 | 72f00f4 | [1.29x faster \*](bm-20220530-3.11.0b2-72f00f4/bm-20220530-linux-x86_64-python-main-3.11.0b2-72f00f4-vs-3.10.4.md) | [1.02x faster \*](bm-20220530-3.11.0b2-72f00f4/bm-20220530-linux-x86_64-python-main-3.11.0b2-72f00f4-vs-3.11.0.md) |  |
| [2022-06-01](bm-20220601-3.11.0b3-eb0004c) | python | main | 3.11.0b3 | eb0004c | [1.30x faster \*](bm-20220601-3.11.0b3-eb0004c/bm-20220601-linux-x86_64-python-main-3.11.0b3-eb0004c-vs-3.10.4.md) | [1.02x faster \*](bm-20220601-3.11.0b3-eb0004c/bm-20220601-linux-x86_64-python-main-3.11.0b3-eb0004c-vs-3.11.0.md) |  |
| [2022-07-11](bm-20220711-3.11.0b4-5a7e1e0) | python | 5a7e1e0a92 | 3.11.0b4 | 5a7e1e0 | [1.28x faster](bm-20220711-3.11.0b4-5a7e1e0/bm-20220711-linux-x86_64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0-vs-3.10.4.md) | [1.01x faster](bm-20220711-3.11.0b4-5a7e1e0/bm-20220711-linux-x86_64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0-vs-3.11.0.md) |  |
| [2022-07-25](bm-20220725-3.11.0b5-0771d71) | python | 0771d71eea | 3.11.0b5 | 0771d71 | [1.27x faster](bm-20220725-3.11.0b5-0771d71/bm-20220725-linux-x86_64-python-0771d71eea30316020a8-3.11.0b5-0771d71-vs-3.10.4.md) | [1.01x faster](bm-20220725-3.11.0b5-0771d71/bm-20220725-linux-x86_64-python-0771d71eea30316020a8-3.11.0b5-0771d71-vs-3.11.0.md) |  |
| [2022-08-05](bm-20220805-3.11.0rc1-41cb071) | python | 41cb07120b | 3.11.0rc1 | 41cb071 | [1.27x faster](bm-20220805-3.11.0rc1-41cb071/bm-20220805-linux-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.10.4.md) | [1.00x faster](bm-20220805-3.11.0rc1-41cb071/bm-20220805-linux-x86_64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.11.0.md) |  |
| [2022-09-11](bm-20220911-3.11.0rc2-ed7c3ff) | python | ed7c3ff156 | 3.11.0rc2 | ed7c3ff | [1.26x faster](bm-20220911-3.11.0rc2-ed7c3ff/bm-20220911-linux-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.10.4.md) | [1.00x slower](bm-20220911-3.11.0rc2-ed7c3ff/bm-20220911-linux-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.11.0.md) |  |
| [2022-10-24](bm-20221024-3.11.0-deaf509) | python | v3.11.0 | 3.11.0 | deaf509 | [1.26x faster](bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509-vs-3.10.4.md) |  |  |
| [2022-12-06](bm-20221206-3.11.1-a7a450f) | python | a7a450f84a | 3.11.1 | a7a450f | [1.25x faster](bm-20221206-3.11.1-a7a450f/bm-20221206-linux-x86_64-python-a7a450f84a0874216031-3.11.1-a7a450f-vs-3.10.4.md) | [1.00x slower](bm-20221206-3.11.1-a7a450f/bm-20221206-linux-x86_64-python-a7a450f84a0874216031-3.11.1-a7a450f-vs-3.11.0.md) |  |
| [2022-06-11](bm-20220611-3.12.0a1+-733e15f) | python | main | 3.12.0a1+ | 733e15f | [1.31x faster \*](bm-20220611-3.12.0a1+-733e15f/bm-20220611-linux-x86_64-python-main-3.12.0a1+-733e15f-vs-3.10.4.md) | [1.03x faster \*](bm-20220611-3.12.0a1+-733e15f/bm-20220611-linux-x86_64-python-main-3.12.0a1+-733e15f-vs-3.11.0.md) |  |
| [2022-06-26](bm-20220626-3.12.0a1+-38612a0) | python | main | 3.12.0a1+ | 38612a0 | [1.32x faster \*](bm-20220626-3.12.0a1+-38612a0/bm-20220626-linux-x86_64-python-main-3.12.0a1+-38612a0-vs-3.10.4.md) | [1.04x faster \*](bm-20220626-3.12.0a1+-38612a0/bm-20220626-linux-x86_64-python-main-3.12.0a1+-38612a0-vs-3.11.0.md) |  |
| [2022-07-02](bm-20220702-3.12.0a1+-7db1d2e) | python | main | 3.12.0a1+ | 7db1d2e | [1.32x faster \*](bm-20220702-3.12.0a1+-7db1d2e/bm-20220702-linux-x86_64-python-main-3.12.0a1+-7db1d2e-vs-3.10.4.md) | [1.04x faster \*](bm-20220702-3.12.0a1+-7db1d2e/bm-20220702-linux-x86_64-python-main-3.12.0a1+-7db1d2e-vs-3.11.0.md) |  |
| [2022-07-10](bm-20220710-3.12.0a1+-264b3dd) | python | main | 3.12.0a1+ | 264b3dd | [1.31x faster \*](bm-20220710-3.12.0a1+-264b3dd/bm-20220710-linux-x86_64-python-main-3.12.0a1+-264b3dd-vs-3.10.4.md) | [1.03x faster \*](bm-20220710-3.12.0a1+-264b3dd/bm-20220710-linux-x86_64-python-main-3.12.0a1+-264b3dd-vs-3.11.0.md) |  |
| [2022-07-17](bm-20220717-3.12.0a1+-c20186c) | python | main | 3.12.0a1+ | c20186c | [1.32x faster \*](bm-20220717-3.12.0a1+-c20186c/bm-20220717-linux-x86_64-python-main-3.12.0a1+-c20186c-vs-3.10.4.md) | [1.04x faster \*](bm-20220717-3.12.0a1+-c20186c/bm-20220717-linux-x86_64-python-main-3.12.0a1+-c20186c-vs-3.11.0.md) |  |
| [2022-08-06](bm-20220806-3.12.0a1+-330f1d5) | python | main | 3.12.0a1+ | 330f1d5 | [1.32x faster \*](bm-20220806-3.12.0a1+-330f1d5/bm-20220806-linux-x86_64-python-main-3.12.0a1+-330f1d5-vs-3.10.4.md) | [1.04x faster \*](bm-20220806-3.12.0a1+-330f1d5/bm-20220806-linux-x86_64-python-main-3.12.0a1+-330f1d5-vs-3.11.0.md) |  |
| [2022-08-13](bm-20220813-3.12.0a1+-32ac98e) | python | main | 3.12.0a1+ | 32ac98e | [1.32x faster \*](bm-20220813-3.12.0a1+-32ac98e/bm-20220813-linux-x86_64-python-main-3.12.0a1+-32ac98e-vs-3.10.4.md) | [1.04x faster \*](bm-20220813-3.12.0a1+-32ac98e/bm-20220813-linux-x86_64-python-main-3.12.0a1+-32ac98e-vs-3.11.0.md) |  |
| [2022-10-02](bm-20221002-3.12.0a1+-8baef8a) | python | main | 3.12.0a1+ | 8baef8a | [1.32x faster \*](bm-20221002-3.12.0a1+-8baef8a/bm-20221002-linux-x86_64-python-main-3.12.0a1+-8baef8a-vs-3.10.4.md) | [1.04x faster \*](bm-20221002-3.12.0a1+-8baef8a/bm-20221002-linux-x86_64-python-main-3.12.0a1+-8baef8a-vs-3.11.0.md) |  |
| [2022-10-09](bm-20221009-3.12.0a1+-2d2e01a) | python | main | 3.12.0a1+ | 2d2e01a | [1.30x faster \*](bm-20221009-3.12.0a1+-2d2e01a/bm-20221009-linux-x86_64-python-main-3.12.0a1+-2d2e01a-vs-3.10.4.md) | [1.02x faster \*](bm-20221009-3.12.0a1+-2d2e01a/bm-20221009-linux-x86_64-python-main-3.12.0a1+-2d2e01a-vs-3.11.0.md) |  |
| [2022-10-15](bm-20221015-3.12.0a1+-660f102) | python | main | 3.12.0a1+ | 660f102 | [1.30x faster \*](bm-20221015-3.12.0a1+-660f102/bm-20221015-linux-x86_64-python-main-3.12.0a1+-660f102-vs-3.10.4.md) | [1.03x faster \*](bm-20221015-3.12.0a1+-660f102/bm-20221015-linux-x86_64-python-main-3.12.0a1+-660f102-vs-3.11.0.md) |  |
| [2022-10-19](bm-20221019-3.12.0a1+-5055300) | python | main | 3.12.0a1+ | 5055300 | [1.30x faster \*](bm-20221019-3.12.0a1+-5055300/bm-20221019-linux-x86_64-python-main-3.12.0a1+-5055300-vs-3.10.4.md) | [1.03x faster \*](bm-20221019-3.12.0a1+-5055300/bm-20221019-linux-x86_64-python-main-3.12.0a1+-5055300-vs-3.11.0.md) |  |
| [2022-10-22](bm-20221022-3.12.0a1+-f58631b) | python | main | 3.12.0a1+ | f58631b | [1.30x faster \*](bm-20221022-3.12.0a1+-f58631b/bm-20221022-linux-x86_64-python-main-3.12.0a1+-f58631b-vs-3.10.4.md) | [1.03x faster \*](bm-20221022-3.12.0a1+-f58631b/bm-20221022-linux-x86_64-python-main-3.12.0a1+-f58631b-vs-3.11.0.md) |  |
| [2022-10-29](bm-20221029-3.12.0a2+-fc94d55) | python | main | 3.12.0a2+ | fc94d55 | [1.30x faster \*](bm-20221029-3.12.0a2+-fc94d55/bm-20221029-linux-x86_64-python-main-3.12.0a2+-fc94d55-vs-3.10.4.md) | [1.03x faster \*](bm-20221029-3.12.0a2+-fc94d55/bm-20221029-linux-x86_64-python-main-3.12.0a2+-fc94d55-vs-3.11.0.md) |  |
| [2022-11-12](bm-20221112-3.12.0a2+-57be545) | python | main | 3.12.0a2+ | 57be545 | [1.31x faster \*](bm-20221112-3.12.0a2+-57be545/bm-20221112-linux-x86_64-python-main-3.12.0a2+-57be545-vs-3.10.4.md) | [1.03x faster \*](bm-20221112-3.12.0a2+-57be545/bm-20221112-linux-x86_64-python-main-3.12.0a2+-57be545-vs-3.11.0.md) |  |
| [2022-11-21](bm-20221121-3.12.0a2+-cdde29d) | python | cdde29dde9 | 3.12.0a2+ | cdde29d | [1.31x faster](bm-20221121-3.12.0a2+-cdde29d/bm-20221121-linux-x86_64-python-cdde29dde90947df9bac-3.12.0a2+-cdde29d-vs-3.10.4.md) | [1.03x faster](bm-20221121-3.12.0a2+-cdde29d/bm-20221121-linux-x86_64-python-cdde29dde90947df9bac-3.12.0a2+-cdde29d-vs-3.11.0.md) |  |
| [2022-11-28](bm-20221128-3.12.0a2+-594de16) | python | 594de165bf | 3.12.0a2+ | 594de16 | [1.30x faster](bm-20221128-3.12.0a2+-594de16/bm-20221128-linux-x86_64-python-594de165bf2f21d6b28e-3.12.0a2+-594de16-vs-3.10.4.md) | [1.03x faster](bm-20221128-3.12.0a2+-594de16/bm-20221128-linux-x86_64-python-594de165bf2f21d6b28e-3.12.0a2+-594de16-vs-3.11.0.md) |  |
| [2022-12-05](bm-20221205-3.12.0a2+-e3a3863) | python | e3a3863cb9 | 3.12.0a2+ | e3a3863 | [1.30x faster](bm-20221205-3.12.0a2+-e3a3863/bm-20221205-linux-x86_64-python-e3a3863cb9561705d3dd-3.12.0a2+-e3a3863-vs-3.10.4.md) | [1.03x faster](bm-20221205-3.12.0a2+-e3a3863/bm-20221205-linux-x86_64-python-e3a3863cb9561705d3dd-3.12.0a2+-e3a3863-vs-3.11.0.md) |  |
| [2022-11-19](bm-20221119-3.12.0a3+-b0e1f9c) | python | main | 3.12.0a3+ | b0e1f9c | [1.31x faster \*](bm-20221119-3.12.0a3+-b0e1f9c/bm-20221119-linux-x86_64-python-main-3.12.0a3+-b0e1f9c-vs-3.10.4.md) | [1.03x faster \*](bm-20221119-3.12.0a3+-b0e1f9c/bm-20221119-linux-x86_64-python-main-3.12.0a3+-b0e1f9c-vs-3.11.0.md) |  |
| [2022-12-11](bm-20221211-3.12.0a3+-70be5e4) | python | 70be5e42f6 | 3.12.0a3+ | 70be5e4 | [1.30x faster](bm-20221211-3.12.0a3+-70be5e4/bm-20221211-linux-x86_64-python-70be5e42f6e288de32e0-3.12.0a3+-70be5e4-vs-3.10.4.md) | [1.03x faster](bm-20221211-3.12.0a3+-70be5e4/bm-20221211-linux-x86_64-python-70be5e42f6e288de32e0-3.12.0a3+-70be5e4-vs-3.11.0.md) |  |
| [2022-12-19](bm-20221219-3.12.0a3+-702a5bc) | python | 702a5bc463 | 3.12.0a3+ | 702a5bc | [1.31x faster](bm-20221219-3.12.0a3+-702a5bc/bm-20221219-linux-x86_64-python-702a5bc4637c82dc011e-3.12.0a3+-702a5bc-vs-3.10.4.md) | [1.04x faster](bm-20221219-3.12.0a3+-702a5bc/bm-20221219-linux-x86_64-python-702a5bc4637c82dc011e-3.12.0a3+-702a5bc-vs-3.11.0.md) |  |

## darwin arm64
| date | fork | ref | version | hash | vs. 3.10.4: | vs. 3.11.0: | vs. base: |
| --- | --- | --- | --- | --- | ---: | ---: | ---: |
| [2022-03-23](bm-20220323-3.10.4-9d38120) | python | v3.10.4 | 3.10.4 | 9d38120 |  | [1.22x slower](bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120-vs-3.11.0.md) |  |
| [2022-12-06](bm-20221206-3.10.9-1dd9be6) | python | 1dd9be6584 | 3.10.9 | 1dd9be6 | [1.00x slower](bm-20221206-3.10.9-1dd9be6/bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.10.4.md) | [1.22x slower](bm-20221206-3.10.9-1dd9be6/bm-20221206-darwin-arm64-python-1dd9be6584413fbfa823-3.10.9-1dd9be6-vs-3.11.0.md) |  |
| [2021-11-05](bm-20211105-3.11.0a2-e2b4e4b) | python | e2b4e4bab9 | 3.11.0a2 | e2b4e4b | [1.15x faster](bm-20211105-3.11.0a2-e2b4e4b/bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.10.4.md) | [1.05x slower](bm-20211105-3.11.0a2-e2b4e4b/bm-20211105-darwin-arm64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b-vs-3.11.0.md) |  |
| [2021-12-08](bm-20211208-3.11.0a3-2e91dba) | python | 2e91dba437 | 3.11.0a3 | 2e91dba | [1.15x faster](bm-20211208-3.11.0a3-2e91dba/bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba-vs-3.10.4.md) | [1.06x slower](bm-20211208-3.11.0a3-2e91dba/bm-20211208-darwin-arm64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba-vs-3.11.0.md) |  |
| [2022-01-13](bm-20220113-3.11.0a4-9471106) | python | 9471106fd5 | 3.11.0a4 | 9471106 | [1.17x faster](bm-20220113-3.11.0a4-9471106/bm-20220113-darwin-arm64-python-9471106fd5b47418ffd2-3.11.0a4-9471106-vs-3.10.4.md) | [1.04x slower](bm-20220113-3.11.0a4-9471106/bm-20220113-darwin-arm64-python-9471106fd5b47418ffd2-3.11.0a4-9471106-vs-3.11.0.md) |  |
| [2022-02-03](bm-20220203-3.11.0a5-c4e4b91) | python | c4e4b91557 | 3.11.0a5 | c4e4b91 | [1.09x faster](bm-20220203-3.11.0a5-c4e4b91/bm-20220203-darwin-arm64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91-vs-3.10.4.md) | [1.12x slower](bm-20220203-3.11.0a5-c4e4b91/bm-20220203-darwin-arm64-python-c4e4b91557f18f881f39-3.11.0a5-c4e4b91-vs-3.11.0.md) |  |
| [2022-03-07](bm-20220307-3.11.0a6-3ddfa55) | python | 3ddfa55df4 | 3.11.0a6 | 3ddfa55 | [1.17x faster](bm-20220307-3.11.0a6-3ddfa55/bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55-vs-3.10.4.md) | [1.04x slower](bm-20220307-3.11.0a6-3ddfa55/bm-20220307-darwin-arm64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55-vs-3.11.0.md) |  |
| [2022-04-05](bm-20220405-3.11.0a7-2e49bd0) | python | 2e49bd06c5 | 3.11.0a7 | 2e49bd0 | [1.22x faster](bm-20220405-3.11.0a7-2e49bd0/bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0-vs-3.10.4.md) | [1.01x slower](bm-20220405-3.11.0a7-2e49bd0/bm-20220405-darwin-arm64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0-vs-3.11.0.md) |  |
| [2022-05-06](bm-20220506-3.11.0b1-8d32a5c) | python | 8d32a5c8c4 | 3.11.0b1 | 8d32a5c | [1.21x faster](bm-20220506-3.11.0b1-8d32a5c/bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.10.4.md) | [1.01x slower](bm-20220506-3.11.0b1-8d32a5c/bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c-vs-3.11.0.md) |  |
| [2022-05-30](bm-20220530-3.11.0b2-72f00f4) | python | 72f00f420a | 3.11.0b2 | 72f00f4 | [1.21x faster](bm-20220530-3.11.0b2-72f00f4/bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4-vs-3.10.4.md) | [1.01x slower](bm-20220530-3.11.0b2-72f00f4/bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4-vs-3.11.0.md) |  |
| [2022-06-01](bm-20220601-3.11.0b3-eb0004c) | python | eb0004c271 | 3.11.0b3 | eb0004c | [1.21x faster](bm-20220601-3.11.0b3-eb0004c/bm-20220601-darwin-arm64-python-eb0004c27163ec089201-3.11.0b3-eb0004c-vs-3.10.4.md) | [1.01x slower](bm-20220601-3.11.0b3-eb0004c/bm-20220601-darwin-arm64-python-eb0004c27163ec089201-3.11.0b3-eb0004c-vs-3.11.0.md) |  |
| [2022-07-11](bm-20220711-3.11.0b4-5a7e1e0) | python | 5a7e1e0a92 | 3.11.0b4 | 5a7e1e0 | [1.23x faster](bm-20220711-3.11.0b4-5a7e1e0/bm-20220711-darwin-arm64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0-vs-3.10.4.md) | [1.01x faster](bm-20220711-3.11.0b4-5a7e1e0/bm-20220711-darwin-arm64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0-vs-3.11.0.md) |  |
| [2022-07-25](bm-20220725-3.11.0b5-0771d71) | python | 0771d71eea | 3.11.0b5 | 0771d71 | [1.23x faster](bm-20220725-3.11.0b5-0771d71/bm-20220725-darwin-arm64-python-0771d71eea30316020a8-3.11.0b5-0771d71-vs-3.10.4.md) | [1.01x faster](bm-20220725-3.11.0b5-0771d71/bm-20220725-darwin-arm64-python-0771d71eea30316020a8-3.11.0b5-0771d71-vs-3.11.0.md) |  |
| [2022-08-05](bm-20220805-3.11.0rc1-41cb071) | python | 41cb07120b | 3.11.0rc1 | 41cb071 | [1.23x faster](bm-20220805-3.11.0rc1-41cb071/bm-20220805-darwin-arm64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.10.4.md) | [1.01x faster](bm-20220805-3.11.0rc1-41cb071/bm-20220805-darwin-arm64-python-41cb07120b7792eac641-3.11.0rc1-41cb071-vs-3.11.0.md) |  |
| [2022-09-11](bm-20220911-3.11.0rc2-ed7c3ff) | python | ed7c3ff156 | 3.11.0rc2 | ed7c3ff | [1.22x faster](bm-20220911-3.11.0rc2-ed7c3ff/bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.10.4.md) | [1.00x faster](bm-20220911-3.11.0rc2-ed7c3ff/bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff-vs-3.11.0.md) |  |
| [2022-10-24](bm-20221024-3.11.0-deaf509) | python | deaf509e8f | 3.11.0 | deaf509 | [1.22x faster](bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-deaf509e8fc6e0363bd6-3.11.0-deaf509-vs-3.10.4.md) |  |  |
| [2022-12-06](bm-20221206-3.11.1-a7a450f) | python | a7a450f84a | 3.11.1 | a7a450f | [1.22x faster](bm-20221206-3.11.1-a7a450f/bm-20221206-darwin-arm64-python-a7a450f84a0874216031-3.11.1-a7a450f-vs-3.10.4.md) | [1.00x faster](bm-20221206-3.11.1-a7a450f/bm-20221206-darwin-arm64-python-a7a450f84a0874216031-3.11.1-a7a450f-vs-3.11.0.md) |  |
| [2022-09-04](bm-20220904-3.12.0a0-a0ad63e) | python | a0ad63e70e | 3.12.0a0 | a0ad63e | [1.21x faster](bm-20220904-3.12.0a0-a0ad63e/bm-20220904-darwin-arm64-python-a0ad63e70e3682cdf7e8-3.12.0a0-a0ad63e-vs-3.10.4.md) | [1.01x slower](bm-20220904-3.12.0a0-a0ad63e/bm-20220904-darwin-arm64-python-a0ad63e70e3682cdf7e8-3.12.0a0-a0ad63e-vs-3.11.0.md) |  |
| [2022-09-12](bm-20220912-3.12.0a0-1756ffd) | python | 1756ffd66a | 3.12.0a0 | 1756ffd | [1.20x faster](bm-20220912-3.12.0a0-1756ffd/bm-20220912-darwin-arm64-python-1756ffd66a38755cd45d-3.12.0a0-1756ffd-vs-3.10.4.md) | [1.02x slower](bm-20220912-3.12.0a0-1756ffd/bm-20220912-darwin-arm64-python-1756ffd66a38755cd45d-3.12.0a0-1756ffd-vs-3.11.0.md) |  |
| [2022-09-19](bm-20220919-3.12.0a0-5b3a256) | python | 5b3a2569f4 | 3.12.0a0 | 5b3a256 | [1.20x faster](bm-20220919-3.12.0a0-5b3a256/bm-20220919-darwin-arm64-python-5b3a2569f4b4dfb58a8f-3.12.0a0-5b3a256-vs-3.10.4.md) | [1.02x slower](bm-20220919-3.12.0a0-5b3a256/bm-20220919-darwin-arm64-python-5b3a2569f4b4dfb58a8f-3.12.0a0-5b3a256-vs-3.11.0.md) |  |
| [2022-09-26](bm-20220926-3.12.0a0-2b428a1) | python | 2b428a1fae | 3.12.0a0 | 2b428a1 | [1.20x faster](bm-20220926-3.12.0a0-2b428a1/bm-20220926-darwin-arm64-python-2b428a1faed88f148ede-3.12.0a0-2b428a1-vs-3.10.4.md) | [1.02x slower](bm-20220926-3.12.0a0-2b428a1/bm-20220926-darwin-arm64-python-2b428a1faed88f148ede-3.12.0a0-2b428a1-vs-3.11.0.md) |  |
| [2022-10-02](bm-20221002-3.12.0a0-14d4f68) | python | 14d4f68ebb | 3.12.0a0 | 14d4f68 | [1.20x faster](bm-20221002-3.12.0a0-14d4f68/bm-20221002-darwin-arm64-python-14d4f68ebb495fe7ccba-3.12.0a0-14d4f68-vs-3.10.4.md) | [1.02x slower](bm-20221002-3.12.0a0-14d4f68/bm-20221002-darwin-arm64-python-14d4f68ebb495fe7ccba-3.12.0a0-14d4f68-vs-3.11.0.md) |  |
| [2022-10-09](bm-20221009-3.12.0a0-281a3f1) | python | 281a3f18cc | 3.12.0a0 | 281a3f1 | [1.20x faster](bm-20221009-3.12.0a0-281a3f1/bm-20221009-darwin-arm64-python-281a3f18cc2afac0fa92-3.12.0a0-281a3f1-vs-3.10.4.md) | [1.02x slower](bm-20221009-3.12.0a0-281a3f1/bm-20221009-darwin-arm64-python-281a3f18cc2afac0fa92-3.12.0a0-281a3f1-vs-3.11.0.md) |  |
| [2022-10-16](bm-20221016-3.12.0a0-bb38b39) | python | bb38b39b33 | 3.12.0a0 | bb38b39 | [1.20x faster](bm-20221016-3.12.0a0-bb38b39/bm-20221016-darwin-arm64-python-bb38b39b339191c5fc00-3.12.0a0-bb38b39-vs-3.10.4.md) | [1.02x slower](bm-20221016-3.12.0a0-bb38b39/bm-20221016-darwin-arm64-python-bb38b39b339191c5fc00-3.12.0a0-bb38b39-vs-3.11.0.md) |  |
| [2022-10-24](bm-20221024-3.12.0a0-dfb5d27) | python | dfb5d272e6 | 3.12.0a0 | dfb5d27 | [1.20x faster](bm-20221024-3.12.0a0-dfb5d27/bm-20221024-darwin-arm64-python-dfb5d272e6b99c2c70c6-3.12.0a0-dfb5d27-vs-3.10.4.md) | [1.02x slower](bm-20221024-3.12.0a0-dfb5d27/bm-20221024-darwin-arm64-python-dfb5d272e6b99c2c70c6-3.12.0a0-dfb5d27-vs-3.11.0.md) |  |
| [2022-10-31](bm-20221031-3.12.0a1+-29f98b4) | python | 29f98b46b7 | 3.12.0a1+ | 29f98b4 | [1.20x faster](bm-20221031-3.12.0a1+-29f98b4/bm-20221031-darwin-arm64-python-29f98b46b77ee528477b-3.12.0a1+-29f98b4-vs-3.10.4.md) | [1.02x slower](bm-20221031-3.12.0a1+-29f98b4/bm-20221031-darwin-arm64-python-29f98b46b77ee528477b-3.12.0a1+-29f98b4-vs-3.11.0.md) |  |
| [2022-11-06](bm-20221106-3.12.0a1+-728e42f) | python | 728e42fcf5 | 3.12.0a1+ | 728e42f | [1.17x faster](bm-20221106-3.12.0a1+-728e42f/bm-20221106-darwin-arm64-python-728e42fcf51cbb2108ca-3.12.0a1+-728e42f-vs-3.10.4.md) | [1.04x slower](bm-20221106-3.12.0a1+-728e42f/bm-20221106-darwin-arm64-python-728e42fcf51cbb2108ca-3.12.0a1+-728e42f-vs-3.11.0.md) |  |
| [2022-11-13](bm-20221113-3.12.0a1+-367f552) | python | 367f552129 | 3.12.0a1+ | 367f552 | [1.19x faster](bm-20221113-3.12.0a1+-367f552/bm-20221113-darwin-arm64-python-367f552129341796d75f-3.12.0a1+-367f552-vs-3.10.4.md) | [1.03x slower](bm-20221113-3.12.0a1+-367f552/bm-20221113-darwin-arm64-python-367f552129341796d75f-3.12.0a1+-367f552-vs-3.11.0.md) |  |
| [2022-11-21](bm-20221121-3.12.0a2+-cdde29d) | python | cdde29dde9 | 3.12.0a2+ | cdde29d | [1.19x faster](bm-20221121-3.12.0a2+-cdde29d/bm-20221121-darwin-arm64-python-cdde29dde90947df9bac-3.12.0a2+-cdde29d-vs-3.10.4.md) | [1.03x slower](bm-20221121-3.12.0a2+-cdde29d/bm-20221121-darwin-arm64-python-cdde29dde90947df9bac-3.12.0a2+-cdde29d-vs-3.11.0.md) |  |
| [2022-11-28](bm-20221128-3.12.0a2+-594de16) | python | 594de165bf | 3.12.0a2+ | 594de16 | [1.19x faster](bm-20221128-3.12.0a2+-594de16/bm-20221128-darwin-arm64-python-594de165bf2f21d6b28e-3.12.0a2+-594de16-vs-3.10.4.md) | [1.03x slower](bm-20221128-3.12.0a2+-594de16/bm-20221128-darwin-arm64-python-594de165bf2f21d6b28e-3.12.0a2+-594de16-vs-3.11.0.md) |  |
| [2022-12-05](bm-20221205-3.12.0a2+-e3a3863) | python | e3a3863cb9 | 3.12.0a2+ | e3a3863 | [1.18x faster](bm-20221205-3.12.0a2+-e3a3863/bm-20221205-darwin-arm64-python-e3a3863cb9561705d3dd-3.12.0a2+-e3a3863-vs-3.10.4.md) | [1.04x slower](bm-20221205-3.12.0a2+-e3a3863/bm-20221205-darwin-arm64-python-e3a3863cb9561705d3dd-3.12.0a2+-e3a3863-vs-3.11.0.md) |  |
| [2022-12-11](bm-20221211-3.12.0a3+-70be5e4) | python | 70be5e42f6 | 3.12.0a3+ | 70be5e4 | [1.24x faster](bm-20221211-3.12.0a3+-70be5e4/bm-20221211-darwin-arm64-python-70be5e42f6e288de32e0-3.12.0a3+-70be5e4-vs-3.10.4.md) | [1.02x faster](bm-20221211-3.12.0a3+-70be5e4/bm-20221211-darwin-arm64-python-70be5e42f6e288de32e0-3.12.0a3+-70be5e4-vs-3.11.0.md) |  |


<!-- END table -->