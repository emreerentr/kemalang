VERSION 1.0

syntax:
com arg1 arg2 arg3

if some arguments are not used, then replace the space with \0, for example, if you're not using arg3:
com arg1 arg2 \0

there are no variable declarations, only 4 declared variables a, b, c, d

commands:
  main commands:
    print format \0 \0         prints the value in variable a
    read format \0 \0          reads to variable a
    exit status \0 \0          exits with status status
    equate dest src            sets dest to src
  note that there are two formats, int (format = 1) and char (format = 2) and that there are 2 status: 0 (EXIT_SUCCESS in C) and 1 (EXIT_FAILURE in C)
  other:
    arithmetic:
      add dest_arg1 arg2 \0
      subt dest_arg1 arg2 \0 
      mul dest_arg1 arg2 \0
      div dest_arg1 arg2 \0
      mod dest_arg1 arg2 \0
    logic:
      or dest_arg1 arg2 \0
      xor dest_arg1 arg2 \0
      and dest_arg1 arg2 \0

basically, it has a similar syntax to assembly
  
