# Lesson 7.03: Methods

## Learning Objectives

Students will be able to...

* Define and identify: **method**, **`__str__`**, **`__add__`**, **operator overloading**.
* Create a class with an `__init__` method.
* Understand and use the `self` argument.
* Instantiate a class with an argument.

## Materials/Preparation

* [7.03 Slide Deck](https://github.com/Areson/2nd-semester-introduction-to-computer-science/raw/master/units/7_unit/slidedecks/Intro%20Python%207.03%20TEALS.pptx)
* [Do Now][]
* [Lab - Kangaroo Class][] ([docx][]) ([pdf][])
* [Associated Reading](https://tealsk12.github.io/2nd-semester-introduction-to-computer-science/readings.md#associatedreadings/7.3)
* Read through the do now, lesson, and lab so that you are familiar with the requirements and can assist students.

## Pacing Guide

| **Duration**   | **Description** |
| ---------- | ----------- |
| 5 Minutes  | Do Now      |
| 10 Minutes | Lesson      |
| 35 Minutes | Lab         |
| 5 Minutes | Debrief  |

## Instructor's Notes

### 1. Do Now

* Display the Do Now on the board.
* Students will find that when they try to print the two different Time objects, it produces output that's not particularly useful or readable.
* Students will also discover that adding objects doesn't work...yet!

### 2. Lesson

#### Instruction - Method

* a function inside of a class.
* The first argument is always `self`.

#### Discussion

* Ask students what method we have already seen and used previously. (`init`)
* Ask students how they would distinguish between the two time variables.

#### Instruction - `__str__`

* Need a method called `__str__`.
* This will get called when you print an object.
* it returns a string that is easy to read and understand.

#### Activity

* Have the students practice writing `__str__` for the `Time` class for 5 minutes.
* Have a student write up their string method on the board.

#### Instruction `__add__`

* A method that gets called when the plus sign is used between two `Time` objects.
* In this case it takes as parameters `self` and another `Time` object and returns a `Time` object that is the sum of both.
* Overwriting add is called **operator overloading** because you are re-writing the code used to make the + work.

#### Demonstration

* Work together with students to come up with the add time algorithm.

### 3. Lab

* Have students finish up the time adding method.
* Have students work on kangaroo lab.

### 4. Debrief

* Go over students' questions and demonstrate some students' successfully completed labs.
* Review what a method is, as well as what specific methods were used in today's lab.

## Accommodation/Differentiation

Students that are moving quickly should work on the bonus assignment in the lab or assist a partner that is struggling.

[Do Now]:do_now.md
[Lab - Kangaroo Class]:lab.md
[pdf]: https://github.com/Areson/2nd-semester-introduction-to-computer-science/raw/master/units/7_unit/03_lesson/lab.pdf
[docx]: https://github.com/Areson/2nd-semester-introduction-to-computer-science/raw/master/units/7_unit/03_lesson/lab.docx
