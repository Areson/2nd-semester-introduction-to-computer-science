# Lesson 4.01: Looping Basics

## Learning Objectives

Students will be able to...

* Define and identify: **for loop**, **item**, **iteration**, **scope**.
* Loop through (traverse) the items in a list.
* Be aware of the scope of variables during iteration.

## Materials/Preparation

* [4.01 Slide Deck](https://github.com/Areson/2nd-semester-introduction-to-computer-science/raw/master/units/4_unit/slidedecks/Intro%20Python%204.01%20TEALS.pptx)
* [Do Now][]
* [Lab - de_vowel][] ([docx][]) ([pdf][])
* [Associated Reading](https://tealsk12.github.io/2nd-semester-introduction-to-computer-science/readings.md#associatedreadings/4.1)
* Read through the Do Now, lesson, and lab so that you are familiar with the requirements and can assist students.

## Pacing Guide

| **Duration** | **Description** |
| ----------   | -----------     |
| 10 Minutes   | Do Now          |
| 10 Minutes   | Lesson          |
| 30 Minutes   | Lab             |
| 5 Minutes    | Debrief         |

## Instructor's Notes

### 1. Do Now

* Display the Do Now on the board.
* Students will work through how to use a `for` loop to efficiently complete a repeated action.

### 2. Lesson

* Go over Part 1 of the Do Now. Ask the students what would happen if the list got much larger?
* If they say they would write down a lot of code, ask how readable that might be, or how long would it take to write, or the greater potential for bugs due to typos.
* Go over Part 2 of the Do Now. Ask the students what happened.
* Introduce the **for loop** as a way to deal with issues associated with Part 1 of the Do Now.

#### Optional video explanation of `for` loops and `while` loops using mnemonics

[![Loop Mnemonics](https://img.youtube.com/vi/KosrKNJK9Sw/0.jpg)](https://youtu.be/KosrKNJK9Sw)

Note: This video is great for introducing mnemonics to loops but it does include While loops and mentions Jupyter notebooks at the end of it. We recommend ending the video around the 6:54 mark, prior to the statement at the end about Jupyter notebooks.

* From the code in the Do Now: `for num in list_of_numbers:`
* Emphasize that the body of the `for` loop is the indented part
* **Iteration**: body of the loop is repeated with different values of the list. Note how the body of the loop is repeated but `num` changes. Consider drawing this out on the board.
* Remind students of the concept of **scope**, showing how `num` changes value with each iteration of the loop.
* Go over Part 3 (many students likely didn't have time to finish). Ask students to write the first line of the loop on the board. Have students brainstorm what the body should be. Come to a group consensus and run the code.  

### 3. Lab

* De-vowel Lab: Students will create a function that will take in a sentence and return that sentence without vowels.

### 4. Debrief

* Talk about any issues or challenges the students had with this lab. If there is time, call students up to the board to shown and demonstrate their code/solutions.

## Accommodation/Differentiation

If there is time, go over the bonus question. Explain how a counter is often defined outside a loop, then used to keep track of the count of things inside the loop. Discuss the concept of the counter's scope (counter gets updated in the loop, but doesn't reset automatically at each iteration). Counters can be used with any loop, and are often used with `while` loops.

There's a good example of code re-use here, also showing the wide variety of possible solutions to any coding problem. A very short `count_vowels()` function can be completed using nothing but the completed `de_vowel()` function, with no new loops or counters:

```python
    def count_vowels(any_string):
        return len(any_string) - len(de_vowel(any_string))
```

[Do Now]: do_now.md
[Lab - de_vowel]: lab.md
[pdf]: https://github.com/Areson/2nd-semester-introduction-to-computer-science/raw/master/units/4_unit/01_lesson/lab.pdf
[docx]: https://github.com/Areson/2nd-semester-introduction-to-computer-science/raw/master/units/4_unit/01_lesson/lab.docx
