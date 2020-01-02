### Measuring the Progress towards Technological Singularity using Homoiconic Programming

One of the biggest pitfalls in the debates about technological singularity is the lack of "hard" metrics (experiments, verifiable figures) for the progress towards singularity. This is highly unusual, in fact, completely unprecedented in the history of science and technology, where measurement is the foundation of everything.

This could be due to the fact that singularity is in fact an intractable problem. As such, only "established" people above and beyond academic scrutiny such as Ray Kurzweil would dare give a hard number, yet without verifiable theoretical foundations or experiments.

_As the Internet are full of toxic critics who by definition do not even care to read a single line of code before delivering judgement and condemnation, those of us who dare to attempt at measuring the progress towards singularity would just have to ignore them and seek out parties who are willing to engage in rational analysis and discussions._

In order to filter toxic critics, here is a simple test -- have a look at the following file:

http://phos.epizy.com/smashlet/pdo/fgl.js

This is the source code for "homoiconic transformation", a procedure to transform Forth like Reverse Polish Notation (homoiconic code) into a non-homoiconic host programming language, in this case, JavaScript. We call our implementation of the Reverse Polish Notation "Phos" to distinguish from traditional Forth.

We have demonstrated that it is possible to perform homoiconic transformation in many high level programming languages, as shown in the examples below:

https://github.com/udexon/Homoiconism/blob/master/Q23_Phos_Smashlet.md

We believe that Phos Stack Machine Shelll (Smashlet) can be ported to all known programming language, by translating the Phos engine code, as shown in the examples above. However, a rigourous mathematical proof itself (i.e. that Phos Smashlet can be ported to any known programming language) needs to be written in Forth like Reverse Polish Notation. As such, it will take time to develop the vocabulary (function database) to perform the proof.

We believe any programmer with half a year of programming experience is capable of rewriting Phos engine in a programming language of his (her) choice, as it merely consists of:
- parsing a space delimited string (Reverse Polish Notation) into a list of tokens
- pushing non-function tokens on to the stack,
- executing a function upon reading a function token and pushing the result(s) on to the stack

The Phos engine is a stack machine shell (smashlet), as it is a shell (capable of parsing space delimited string as input) running as a stack machine.

Prior to Phos stack machine shell (smashlet), Forth has been ported to various high level programming languages, besides running on almost all known microprocessor architectures, due to its simplicity and elegance. However, conventional Forth ports in high level programming languages (software Forth) concentrate on porting the full Forth vocabulary (making it difficult for beginners to learn) and not emphasizing on integrating with function libraries of the host programming language, which Phos aims to correct. As such, Phos has the potential to become a universal script that can be used to interface to all known programming languages. We believe this is a huge step towards technological singularity.

The major benefits of Phos smashlet are:
- A Forth like vocabulary (function database) spanning ALL known programming languages can be constructed
- Forth and Phos, being homoiconic, can be use to construct self evaluating metaprogram -- programs that generates other programs in the same programming language and analyse them. This is critical to achieve Artificial General Intelligence
- Forth and Phos can be generalized as mathematical notations. The learning of programming and mathematics can be simplified with a systematic "learn one word at a time" approach, yet another unprecedented breakthrough in the history of computing and mathematics.

Based on the above, the hard metrics towards singularity that we propose are:
- the number of Phos/Forth words mapping across all programming languages
- the number of programmers involved in homoiconic programming
- the level of sophistication in homoiconic programming, e.g. unification with mathematics, self evaluating code, etc.

To be consistent with the spirit of science, our theories are of course open to scrutiny and challenges. We welcome alternative theories to be compared to ours, using rational analysis of course, but not toxic unsubstantiated   criticism.

The weakest link in our theories is the adoption by new programmers. Of course the rate of adoption of new theories very much depends on how well the tutorials are written. This is an area which we welcome collaboration.

Our goals are:

1. To recruit 25 collaborators per quarter in 2020, achieving 100 collaborators by the end of 2020.

2. [ Datong Token ](https://github.com/udexon/DatongToken/blob/master/Datong_3_in_1.md) to achieve total of USD 10K transactions by end of 2020.

3. Port robotics and game engine to Phos by end of 2020.

4. Start work on computer algebra system by end of 2020. Find people to start work on this.

5. Start work on self evaluating code by end of 2020. Find people to start work on this.
