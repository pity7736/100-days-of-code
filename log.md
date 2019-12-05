# 100 Days Of Code - Log

* [Day 0](#day0)
* [Day 1](#day1)
* [Day 2](#day2)
* [Day 3](#day3)
* [Day 4](#day4)
* [Day 5](#day5)
* [Day 6](#day6)
* [Day 7](#day7)
* [Day 8](#day8)
* [Day 9](#day9)
* [Day 10](#day10)
* [Day 11](#day11)
* [Day 12](#day12)
* [Day 13](#day13)

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


<a id="day7"></a>
### Day 7: November 18, 2019

**Today's Progress:**

* Created `DBClient`.
* Renamed environment variables for connection.
* QuerySet now uses `DBClient`.

**Thoughts:**

* I think that I wrong importing cython files. I need to check this installing gideon in other project (like [Odin](https://github.com/pity7736/odin)).

**Link to work:** [gideon](https://github.com/pity7736/gideon)

<a id="day8"></a>
### Day 8: November 19, 2019

**Today's Progress:**

* Better connection pool implementation.
* Added `run_insert` method to `DBClient`.

**Thoughts:**

* I'll check if I need to implement `asyncio.Lock` when acquire connection from `ConnectionPool`.

**Link to work:** [gideon](https://github.com/pity7736/gideon)

<a id="day9"></a>
### Day 9: November 20, 2019

**Today's Progress:**

* Criteria in `filter` is not longer mandatory.
* `filter` in `QuerySet` without side effects.
* Refactorized `get` method. Now it return a new instance of `QuerySet` and is no longer a coroutine.
* Removed `criteria` and `fields` params from `QuerySet`.
* Added `create` method to `Model`. It's just a shortcut to:
```python
    obj = Model(field1=value1, field2=value2)
    await obj.save()
```

**Thoughts:**

* I could not implement `_clone` method in `QuerySet` due to the visibility of the attributes. However, I'll find a way to do it.

**Link to work:** [gideon](https://github.com/pity7736/gideon)

<a id="day10"></a>
### Day 10: November 21, 2019

**Today's Progress:**

* Now `all` method return a new instance of `QuerySet` and is no longer a coroutine.


**Thoughts:**

* I was thinking how to convert `QuerySet` instances to sql. It's not easy. Actually, it's really hard to find a way to make it flexible enough. I think that I need a `SQLCompiler` and `Èxecutor` classes. For now, I don't know!

**Link to work:** [gideon](https://github.com/pity7736/gideon)

<a id="day11"></a>
### Day 11: December 2, 2019

**Today's Progress:**

* Update Model instances with `save` method.


**Thoughts:**

* I think I need to add more features before to make the `SQLCompiler`.

**Link to work:** [gideon](https://github.com/pity7736/gideon)

<a id="day12"></a>
### Day 12: December 3, 2019

**Today's Progress:**

* Refactorized some tests and fixtures.
* Created `movement` fixture.
* The `update_fields` parameter was added to the` save` method that allows only specific fields to be updated.
* Created CHANGELOG file.
* New v0.0.0a6 version uploaded to pypi.


**Thoughts:**

* I'll start type documentation soon.

**Link to work:** [gideon](https://github.com/pity7736/gideon)

<a id="day13"></a>
### Day 13: December 4, 2019

**Today's Progress:**

* Set the `Field` name automatically when this is `None`.
* Created `CharChoicesField` and removed chocies parameter from `Field`. (Not in master)

**Thoughts:**

* I should have done auto field name before.
* I don't decide if merge to master the `CharChoicesField`.  What will be better? The difference would be that choices is removed from all fields types.
```python
    field1 = CharField(choices=ChoicesEnum)
    field2 = CharChoicesField(choices=ChoicesEnum)
```

**Link to work:** [gideon](https://github.com/pity7736/gideon)

