# tpy

```
usage: tpy [-h] [-s SESSION] [-w WINDOW] {cmd,cmd_prev,pytest,python} ...

Runs command in tmux

positional arguments:
  {cmd,cmd_prev,pytest,python}

optional arguments:
  -h, --help            Usage info
  -s SESSION, --session SESSION
                        tmux session to use
  -w WINDOW, --window WINDOW
                        tmux window to use


usage: tpy cmd command

Runs arbitrary command

positional arguments:
  command  Command to execute



usage: tpy cmd_prev [-t TIMES_UP] [-r]

Runs previous command

optional arguments:
  -t TIMES_UP, --times_up TIMES_UP
                        Number of times to press cursor up
  -r, --reset           Resets window before execution, kills running programs



usage: tpy pytest [--executable EXECUTABLE] [-k KEYWORD] [-m MARK] [--pdb]
                  [--ipdb] [-mf MAXFAIL]
                  file_or_dir

Runs pytest on file or directory

positional arguments:
  file_or_dir

optional arguments:
  --executable EXECUTABLE
                        pytest executable
  -k KEYWORD, --keyword KEYWORD
                        Only run tests matching given substring expression
  -m MARK, --mark MARK  Only run tests matching mark expression
  --pdb                 Enables pdb
  --ipdb                Enables ipdb
  -mf MAXFAIL, --maxfail MAXFAIL
                        Maximum failures



usage: tpy python [--executable EXECUTABLE] [--pdb] [--ipdb] [-i] file

Executes file with python

positional arguments:
  file

optional arguments:
  --executable EXECUTABLE
                        Python executable
  --pdb                 Enables pdb
  --ipdb                Enables ipdb
  -i, --interactive     Enables interactive mode
```