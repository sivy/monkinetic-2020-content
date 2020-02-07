date: 2002-10-13
slug: multi-level-break
title: Multi-level 'break'
---
Miscellaneous h4xx0r note: PHP has a mutli-level `` break `` which I had not seen before in a language. Used normally, break will exit the current loop (while, for, etc). Using the optional integer argument:
>  `` break n ``
will break you out of as many nested loops as specified. For example:

<pre> 10 /* Using the optional argument. */
 11 $i = 0;
 12 while ( ++$i ) {
 13     switch ( $i ) {
 14     case 5:
 15         echo "At 5<br/>";
 16         break 1;  /* Exit only the switch. */
 17     case 10:
 18         echo "At 10; quitting<br/>\n";
 19         break 2;  /* Exit the switch and the while. */
 20     default:
 21         break;
 22     }
 23 } </pre>

Found [here](http://phpbuilder.com/manual/control-structures.break.php).