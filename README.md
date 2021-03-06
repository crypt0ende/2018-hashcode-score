# Hash Code 2018 Score Calculator

**TL;DR** Compute score for Hash Code 2018 Qualification Round.

`score.py` was tested successfully on our final submission.

i.e. we obtained the same scores with `score.py` as those given by the official Judge System.

## Usage

`python3 score.py res/a_example.in res/a_example.out`

```
INFO:root:parsing rides
INFO:root:opening a_example.in
INFO:root:3 4 2 3 2 10
INFO:root:done parsing rides
INFO:root:parsing a_example.out
score: 10
```

`python3 score.py res/b_should_be_easy.in res/b_should_be_easy.out`

```
INFO:root:parsing rides
INFO:root:opening b_should_be_easy.in
INFO:root:800 1000 100 300 25 25000
INFO:root:done parsing rides
INFO:root:parsing b_should_be_easy.out
score: 176,877
```

`python3 score.py res/b_should_be_easy.in res/b_should_be_easy.out --score`

```
INFO:root:parsing rides
INFO:root:opening b_should_be_easy.in
INFO:root:800 1000 100 300 25 25000
INFO:root:done parsing rides
INFO:root:parsing b_should_be_easy.out
score: 176,877 = 169,677 + 7,200 (bonus)
```

## Unit Tests

see `test_score.py`

## Output File Checks

The following checks are performed on the output file when the `--check` option is set

check
- [x] ride ids are correct
- [x] rides are assigned only once
- [x] number of cars
- [x] number of steps in the simulation
- [x] simulation with unit tests

### Example

`./score.py res/b_should_be_easy.in res/b_should_be_easy.out --check`

```
INFO:root:parsing rides
INFO:root:opening res/b_should_be_easy.in
INFO:root:800 1000 100 300 25 25000
INFO:root:done parsing rides
INFO:root:parsing res/b_should_be_easy.out
INFO:root:checking vehicles
INFO:root:vehicles: OK
INFO:root:checking ride ids
INFO:root:ride ids: OK
```

## Our Team & Qualification Round

<https://hashcode.withgoogle.com/hashcode_2018.html>

Team: MetaModHell

Members (listed alphabetically): Karbok, PicoJr

Score: 46,048,775

Rank: 628th World, 81st France

### Submissions

| Input            |  Score     |
|:-----------------|-----------:|
| A-example        | 10         |
| B-should be easy | 176,877    |
| C-no hurry       | 13,052,303 |
| D-metropolis     | 11,353,640 |
| E-high bonus     | 21,465,945 |
