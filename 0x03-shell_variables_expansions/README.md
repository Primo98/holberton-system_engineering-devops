#!bins/bash
_08 / February / 2022_

__Learning about variables and expansions___


"The following commands that make up the executable Scripts; __WRITE THEM WITHOUT THE FIRST AND LAST PARENTHESES!__"


0-alias (alias ls="rm *")

_Create a script that creates an alias._

_1. Name: ls
_2. Value: rm *

1-hello_you (echo "hello $USER")

_Create a script that prints hello user, where user is the current Linux user._

10-love_exponent_breath (echo $(($BREATH**LOVE)))

_Write a script that displays the result of BREATH to the power LOVE_

_BREATH and LOVE are environment variables_
_The script should display the result, followed by a new line_

11-binary_to_decimal (echo $((2#$BINARY)))

_Write a script that converts a number from base 2 to base 10._

_The number in base 2 is stored in the environment variable BINARY_
_The script should display the number in base 10, followed by a new line_

12-combinations (echo {a..z}{a..z} | tr ' ' '\n' | grep -v oo)

_Create a script that prints all possible combinations of two letters, except oo._

_Letters are lower cases, from a to z_
_One combination per line_
_The output should be alpha ordered, starting with aa_
_Do not print oo_
_Your script file should contain maximum 64 characters_

13-print_float (printf "%0.2f\n" $NUM)

_Write a script that prints a number with two decimal places, followed by a new line._

_1. The number will be stored in the environment variable NUM._

2-path (PATH=$PATH:/action)

_Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program._

3-paths (echo $PATH | tr ":" "\n" | wc -l)

_Create a script that counts the number of directories in the PATH._

4-global_variables (ls -l | printenv)

_Create a script that lists environment variables._

5-local_variables (set)

_Create a script that lists all local variables and environment variables, and functions._

6-create_local_variable (export BEST="School")

_Create a script that creates a new local variable._

_1. Name: BEST_
_2. Value: School_

7-create_global_variable (export BEST="School")

_Create a script that creates a new global variable._

_Name: BEST_
_Value: School_

8-true_knowledge (echo $(($TRUEKNOWLEDGE+128)))

_Write a script that prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line._

9-divide_and_rule (echo $(($POWER/$DIVIDE)))

_Write a script that prints the result of POWER divided by DIVIDE, followed by a new line._

_1. POWER and DIVIDE are environment variables_

100-decimal_to_hexadecimal (printf "%x\n" $DECIMAL)

_Write a script that converts a number from base 10 to base 16._

_The number in base 10 is stored in the environment variable DECIMAL_
_The script should display the number in base 16, followed by a new line_

101-rot13 (tr 'A-Za-z' 'N-ZA-Mn-za-m')

_Write a script that encodes and decodes text using the rot13 encryption. Assume ASCII._

102-odd (paste -d" " - - | cut -d " " -f 1)

_Write a script that prints every other line from the input, starting with the first line._

103-water_and_stir (printf "%o\n" $(( (5#$(echo $WATER | tr '[water]' '[01234]')) + (5#$(echo $STIR | tr '[stir.]' '[01234]')) )) | tr '[01234567]' '[bestchol]')

_Write a shell script that adds the two numbers stored in the environment variables WATER and STIR and prints the result.

_WATER is in base water_
_STIR is in base stir._
_The result should be in base bestchol_
