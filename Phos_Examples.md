### Phos Smashlet (Stack Machine Shell) Examples

Stack machine is perhaps one of the most ubiquitous but yet under-exposed systems in computer systems. They exist everywhere from the proprietary stack engine in microproessors to the interpreter engine in almost all modern high level programming languages, e.g. PHP, Java, JavaScript, Python etc.

The Forth programming language is perhaps the oldest, well developed and most popular stack machine focused programming language. We have extended the Forth programming language to create ___Phos stack machine shell___ that can be implemented in any known high level programming language.

Although many tutorials and reference materials for Forth exist, they are perhaps too focused on stack machine that programmers of modern programming language find them difficult to grasp. As such, this project is created specifically to introduce stack machine programming from the perspectives of modern programming languages to a wider audience, from six years olds to sixty years olds, quite literally, as we believe the Reverse Polish Notation that forms the foundation of Forth and Phos, is such a wonderful and elegant syntax that can serve as the unifying script to bridge programming languages as well as mathematics.

#### Phos Smashlet in JavaScript

This tutorial is written for both beginners as well as experts in mind. Such a combination is rather rare and is perhaps a proof of the elegance of the stack machine architecture as well as the Reverse Polish Notation. Beginners may skip sections marked with __[EXPERT]__.

1. Open http://phos.epizy.com/smashlet/?i=1 using a desktop browser.

2. Open the Developer Console.

Key in the following commands as shown in the screenshot below:

```
F("now:")
S
F("now: colon:")
S
F("now: colon: explode:")
S
```

<img src="https://github.com/udexon/EMYL/blob/master/Phos_now_JavaScript.png" width=300>

`S`, the data stack, is implemented as a global array in JavaScript. Entering `S` on its own in the developer console will print out the its contents. 

- `F("now:")` results in the current time to be _pushed on to the stack_. 
- `F("now: colon:")` pushes an additional colon `:` character on to the stack. 
- `F("now: colon: explode:")` splits the date time string using colon as the delimiter and pushes the results (an array containing parts separated by colon) on to the stack.

__[EXPERT]__ The source code for the above can be viewed at http://phos.epizy.com/smashlet/pdo/fgl.js

In summary, the operations of the stack machine are:
- push a non-function token to the stack
- execute a host programming language (JavaScript) function mapped by a function token

It is dues to this simplicity that the Phos stack machine shell (smashlet) can be implemented in any known host programming language, with around 20 lines of code for the core operations described above.


#### Phos Smashlet in Java

(upload to github ...)

```
$ java -cp '.:../../libs/*' com.udexon.smashlet.Phos 1 sstr: esp:
 1

$ java -cp '.:../libs/*' com.udexon.smashlet.Phos 1 2 + now: sstr: esp:
 3 2019-12-17T20:38:37.906005 
 
$ java -cp '.:../libs/*' com.udexon.smashlet.Phos 1 2 + now: colon: explode: sstr: esp:
 3 ["2019-12-17T20","38","18.131809"]  
```


#### Phos Smashlet in PHP

```
$ php phos.php HELLO s:
fgl_s 442 < 3 > array ( 
0 => array ( 0 => 'phos.php', 1 => 'HELLO', 2 => 's:', ), 
1 => 'phos.php', 
2 => 'HELLO', )

$ php phos.php now: s:
fgl_s 442 < 3 > array ( 0 => array ( 0 => 'phos.php', 1 => 'now:', 2 => 's:', ), 1 => 'phos.php', 2 => '2019-12-17T20:27:31.525', )

$ php phos.php now: colon: s:
fgl_s 442 < 4 > array ( 0 => array ( 0 => 'phos.php', 1 => 'now:', 2 => 'colon:', 3 => 's:', ), 1 => 'phos.php', 2 => '2019-12-17T20:22:16.509', 3 => ':', )

$ php phos.php now: colon: explode: s:
fgl_s 442 < 3 > array ( 0 => array ( 0 => 'phos.php', 1 => 'now:', 2 => 'colon:', 3 => 'explode:', 4 => 's:', ), 1 => 'phos.php', 2 => array ( 0 => '2019-12-17T20', 1 => '22', 2 => '36.535', ), )
```

