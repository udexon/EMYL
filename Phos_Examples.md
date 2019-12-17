### Phos Smashlet (Stack Machine Shell) Examples

Stack machine is perhaps one of the most ubiquitous but yet under-exposed systems in computer systems. They exist everywhere from the proprietary stack engine in microproessors to the interpreter engine in almost all modern high level programming languages, e.g. PHP, Java, JavaScript, Python etc.

The Forth programming language is perhaps the oldest, well developed and most popular stack machine focused programming language. We have extended the Forth programming language to create ___Phos stack machine shell___ that can be implemented in any known high level programming language.

#### Phos JavaScript

1. Open http://phos.epizy.com/smashlet/?i=1

2. Open Developer Console.

<img src="https://github.com/udexon/EMYL/blob/master/Phos_now_JavaScript.png" width=300>

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

```
$ java -cp '.:../../libs/*' com.udexon.smashlet.Phos 1 sstr: esp:
 1

$ java -cp '.:../libs/*' com.udexon.smashlet.Phos 1 2 + now: sstr: esp:
 3 2019-12-17T20:38:37.906005 
 
$ java -cp '.:../libs/*' com.udexon.smashlet.Phos 1 2 + now: colon: explode: sstr: esp:
 3 ["2019-12-17T20","38","18.131809"]  
```
