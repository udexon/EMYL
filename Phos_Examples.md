```
$ php phos.php HELLO s:
fgl_s 442 < 3 > array ( 0 => array ( 0 => 'phos.php', 1 => 'HELLO', 2 => 's:', ), 1 => 'phos.php', 2 => 'HELLO', )

$ php phos.php now: s:
fgl_s 442 < 3 > array ( 0 => array ( 0 => 'phos.php', 1 => 'now:', 2 => 's:', ), 1 => 'phos.php', 2 => '2019-12-17T20:27:31.525', )

$ php phos.php now: colon: s:
fgl_s 442 < 4 > array ( 0 => array ( 0 => 'phos.php', 1 => 'now:', 2 => 'colon:', 3 => 's:', ), 1 => 'phos.php', 2 => '2019-12-17T20:22:16.509', 3 => ':', )

$ php phos.php now: colon: explode: s:
fgl_s 442 < 3 > array ( 0 => array ( 0 => 'phos.php', 1 => 'now:', 2 => 'colon:', 3 => 'explode:', 4 => 's:', ), 1 => 'phos.php', 2 => array ( 0 => '2019-12-17T20', 1 => '22', 2 => '36.535', ), )
```
