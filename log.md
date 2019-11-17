# 100 Days Of Code - Log

* [Day 0](#day0)
* [Day 1](#day1)
* [Day 2](#day2)
* [Day 3](#day3)
* [Day 4](#day4)
* [Day 5](#day5)
* [Day 6](#day6)

<a id="day0"></a>
### Day 0: November 9, 2019

**Today's Progress:** I updated status project and I planned the following steps.

**Thoughts:** Although I had not made commits since July, I was able to update quickly with status project.

**Link to work:** [gideon project](https://github.com/pity7736/gideon)


<a id="day1"></a>
### Day 1: November 10, 2019

**Today's Progress:** I learning about python descriptors.

**Thoughts:** Maybe I could use python descriptors to run field validators.


<a id="day2"></a>
### Day 2: November 11, 2019

**Today's Progress:**

* Updated requirements.
* Added choices as `Enum` to field.
* Added `to_python` method to `Field` and use it in `Model.__init__`.
* Added choices validation in setter.

**Thoughts:**

* I must be careful with OS upgrades. The virtualenv failed after upgrade and wasted my time. Maybe it could be for cython compilation.
* I was able to add the choices as `Enum` and continue using cython in the fields. Last time I wasn't

**Link to work:** [gideon project](https://github.com/pity7736/gideon)


<a id="day3"></a>
### Day 3: November 12, 2019

**Today's Progress:**

* Created `QuerySet` class
* Added `all`, `get` and `filter` methods to `QuerySet` and `Model` calls these methods.
* `filter` method return another `QuerySet` instance with the new filter criteria.

**Thoughts:**

* It was very easy to add `QuerySet` class and replace the methods thanks to the tests.
* Radon (lib to calculate a cyclomatic complexity number) and pytest-coverage don't work with cython files. I need to find a way to solve this.

**Link to work:** [queryset PR](https://github.com/pity7736/gideon/pull/1/files)

<a id="day4"></a>
### Day 4: November 13, 2019

**Today's Progress:**

* Added `only` method to `QuerySet`.
* Refactorized `_run_query` method.

**Thoughts:**

* I need to review `get` and `all` methods. Maybe they shouldn't be coroutines but functions.

**Link to work:** [PR](https://github.com/pity7736/gideon/pull/2/files)

<a id="day5"></a>
### Day 5: November 14, 2019

**Today's Progress:**

* Implemented dummy connection pool

**Thoughts:**

* The `__new__` method is not available in cython. I could not implement `ConnectionPool` as singleton.
* I'm going to create a  database client that uses the `ConnectionPool`.

**Link to work:** [gideon](https://github.com/pity7736/gideon/)

<a id="day6"></a>
### Day 6: November 16, 2019

**Today's Progress:**

* I was learning about concurrency.

**Thoughts:**

* The threading is more complicated than I thought.
* It's very common bugs in threading code and it's very difficult find them.
