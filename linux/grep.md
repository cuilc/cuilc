
#grep multiple word at one time 
grep -n --color=auto -E 'word1|word2|word3' target.file -n show line num

-E regular expression
--color=auto show color to which matched word
-Cnum show 
-Anum show more NUM lines AFTER the matched line
-Bnum show more NUM lines BEFORE the matched line

