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
* [Day 14](#day14)
* [Day 15](#day15)
* [Day 16](#day16)
* [Day 17](#day17)
* [Day 18](#day18)
* [Day 19](#day19)
* [Day 20](#day20)
* [Day 21](#day21)
* [Day 22](#day22)
* [Day 23](#day23)
* [Day 24](#day24)
* [Day 25](#day25)
* [Day 26](#day26)
* [Day 27](#day27)
* [Day 28](#day28)
* [Day 29](#day29)
* [Day 30](#day30)


<a id="day0"></a>
### Day 0: January 29, 2020

**Today's Progress:** I started a small lib for holidays and working days calculations.

**Thoughts:** I learned about [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) and I started to applying it in this project.

**Link to work:** [workingless project](https://github.com/pity7736/workingless)

<a id="day1"></a>
### Day 1: January 30, 2020

**Today's Progress:** I refactorized holidays calculations.

**Thoughts:** I like tests more and more!

**Link to work:** [refactor](https://github.com/pity7736/workingless/commit/310f3a7447f45d34d6cfe862da014a8b8fa787b3)

<a id="day2"></a>
### Day 2: January 31, 2020

**Today's Progress:** Added `is_holiday` function.

**Thoughts:** I hope add another country, maybe Mexico, very soon.

**Link to work:** [commit](https://github.com/pity7736/workingless/commit/e44b0cd7b67001fe1d469e9967b857ca6fa09554)


<a id="day3"></a>
### Day 3: February 1, 2020

**Today's Progress:** Initial documentation

**Thoughts:** Learning more about sphinx and documentation in general.

**Link to work:** [workingless project](https://github.com/pity7736/workingless)

<a id="day4"></a>
### Day 4: February 2, 2020

**Today's Progress:** I started multi country feature.

**Thoughts:** I need to find a way to do multi country very flexible.

**Link to work:** [workingless project](https://github.com/pity7736/workingless)

<a id="day5"></a>
### Day 5: February 3, 2020

**Today's Progress:** I refactorized `HolidayCalculator` class and its `calculate` method. I applied strategy design pattern.

**Thoughts:** I need to practice more and more until achieve a good architecture.

**Link to work:** [workingless project](https://github.com/pity7736/workingless)

<a id="day6"></a>
### Day 6: February 4, 2020

**Today's Progress:** I haven't much time and I not wrote code but I was thinking about next steps in architecture.

**Thoughts:** The architecture is changing.

**Link to work:** [workingless project](https://github.com/pity7736/workingless)

<a id="day7"></a>
### Day 7: February 5, 2020

**Today's Progress:** Today I was thinking how make easy to add more countries.

**Thoughts:** It's hard for me to make a decision about the architecture.

**Link to work:** [workingless project](https://github.com/pity7736/workingless)

<a id="day8"></a>
### Day 8: February 7, 2020

**Today's Progress:** I added Mexico. Removed api module and moved function to `CountryBase` class as methods.

**Thoughts:** I like how the project looks but I need some feedback, so I will release 0.1.0 version this weekend and share the project with some friends.

**Link to work:** [commit](https://github.com/pity7736/workingless/commit/0639f3efa9ea1e9f7c16aceed1ebd22437f91c04)

<a id="day9"></a>
### Day 9: February 8, 2020

**Today's Progress:** Added some documentation and readme updated.

**Thoughts:** Writing documentation makes me change some classes name.

**Link to work:** [commit](https://github.com/pity7736/workingless/commit/47024c9544014f26b692023831e2bc2e9ef97a35)

<a id="day10"></a>
### Day 10: February 10, 2020

**Today's Progress:** I added `get_next_working_day` and `is_working_day` methods.

**Thoughts:** I renamed countries by using [ISO 3166](https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)

**Link to work:** [workingless project](https://github.com/pity7736/workingless)

<a id="day11"></a>
### Day 11: February 11, 2020

**Today's Progress:** I released version 0.1.1!

**Thoughts:** I made a mistake. I uploaded version 0.1.0 to pypi but I didn't commit the changes. For thar teason the version released is 0.1.1.

**Link to work:** [workingless project](https://github.com/pity7736/workingless)


<a id="day12"></a>
### Day 12: February 12, 2020

**Today's Progress:** Added `NDayHolidayCalculator`

**Thoughts:** It was not simple add new holiday calculator, so I think that I'm going to refactor it.

**Link to work:** [workingless project](https://github.com/pity7736/workingless)


<a id="day13"></a>
### Day 13: February 13, 2020

**Today's Progress:** I changed relationships and removed `Holiday` and `HolidaCalulator` classes.

**Thoughts:** I think that now is much simpler to add another holiday calculator.

**Link to work:** [workingless project](https://github.com/pity7736/workingless)

<a id="day14"></a>
### Day 14: February 14, 2020

**Today's Progress:** I added some tests for calulators

**Thoughts:** When I did the tests I realized that the calculators isn't specific for holidays, so I renamed them.

**Link to work:** [workingless project](https://github.com/pity7736/workingless)

<a id="day15"></a>
### Day 15: February 15, 2020

**Today's Progress:** I updated documentation and integrated CI with circle ci.

**Thoughts:** It's easy the first step to do CI with circle. I think that I'm going to upload each new version with circle.

**Link to work:** [workingless project](https://github.com/pity7736/workingless)

<a id="day16"></a>
### Day 16: February 16, 2020

**Today's Progress:** I tested the lib with different python versions by using circle. Also, a was preparing a talk about asyncIO for the office team.

**Thoughts:** It's really nice to use CI like circle.

**Link to work:** [workingless project](https://github.com/pity7736/workingless)

<a id="day17"></a>
### Day 17: February 17, 2020

**Today's Progress:** I added `EveryNYearsCalculator` and get holidays for Mexico. Version 0.2.0 released!

**Thoughts:** I need to be more carefully when I release a new version, I forgot update the readme!

**Link to work:** [workingless project](https://github.com/pity7736/workingless)

<a id="day18"></a>
### Day 18: February 18, 2020

**Today's Progress:** I didn't code today but I was learning more about concurrency.

**Thoughts:** I saw some advantages and disadvantages about threading and multiproccesing. It's so interesting.

**Link to work:**
  - [Raymond Hettinger keynote](https://www.youtube.com/watch?v=9zinZmE3Ogk)
  - [AsyncIO real python](https://realpython.com/async-io-python/)

<a id="day19"></a>
### Day 19: February 19, 2020

**Today's Progress:** I was readin extreme programming book today.

**Thoughts:** It's a very interesting book. I hope to implement in my work.

<a id="day20"></a>
### Day 20: February 20, 2020

**Today's Progress:** I was reading XP book. Also, I was reviewing and remembering the gideon code. I'll be working on it tomorrow.

**Thoughts:** I liked the XP values, principles and practices. I had already done some of them but I think that I need to do all of them and do it more frequently.

**Link to work:** [gideon project](https://github.com/pity7736/gideon)

<a id="day21"></a>
### Day 21: February 23, 2020

**Today's Progress:** I was preparing a asyncio talk.

**Thoughts:** It's interesting what I'm learning meanwhile I prepare the talk.

<a id="day22"></a>
### Day 22: February 24, 2020

**Today's Progress:** I was preparing a asyncio talk.

**Thoughts:** I think that I want to give the talk in python Bogotá meeting.

**Link to work:** [talk exercises](https://github.com/pity7736/asyncio-talk)

<a id="day23"></a>
### Day 23: February 26, 2020

**Today's Progress:** I was reading XP book and I still preparing a asyncio talk.

**Thoughts:** I thinking about what XP practices to implement in my teamwork.

**Link to work:** [talk exercises](https://github.com/pity7736/asyncio-talk)

<a id="day24"></a>
### Day 24: February 27, 2020

**Today's Progress:** I still preparing a asyncio talk.

**Thoughts:** I'm so slow. 

**Link to work:** [talk exercises](https://github.com/pity7736/asyncio-talk)

<a id="day25"></a>
### Day 25: February 28, 2020

**Today's Progress:** Last day preparing talk

**Thoughts:** ...

**Link to work:** [talk exercises](https://github.com/pity7736/asyncio-talk)


<a id="day26"></a>
### Day 26: March 1, 2020

**Today's Progress:** I was reading a XP book.

**Thoughts:** 


<a id="day27"></a>
### Day 27: March 2, 2020

**Today's Progress:** I was reading a XP book.

**Thoughts:** I was thinking about what project is the next for this callenge.

<a id="day28"></a>
### Day 28: March 3, 2020

**Today's Progress:** Today I was watching videos about TDD. In fact, I bought a video of cleancoders (Uncle Bob Martin) about it.

**Thoughts:** I did decide to write a personal accounting application with pluggable DB engine.

<a id="day29"></a>
### Day 29: March 4, 2020

**Today's Progress:** Today I was watching the second episode of chicago vs london from cleancoders.

**Thoughts:** It's interesting the way that acceptance tests prove the architecture and unit test drive the architecture.

<a id="day30"></a>
### Day 30: March 5, 2020

**Today's Progress:** Today I was watching the third episode of chicago vs london from cleancoders.

**Thoughts:** I like the london way but I think the tests mock so much.
