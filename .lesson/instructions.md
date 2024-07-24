# Assignment 1: Salutations

Create Python program called `saluations.py` that will print a friendly greeting.

Open the new `salutations.py` program and modify it to accept three optional arguments:

* `-g|--greeting`: A greeting, defaults to "Howdy"
* `-n|--name`: A name to greeting, defaults to "Stranger"
* `-e|--excited`: A flag to terminate the greeting with an exclamation point

The program should respond to `-h|--help` to print the following usage:

```
$ ./salutations.py -h
usage: salutations.py [-h] [-g str] [-n str] [-e]

Greetings and salutations

optional arguments:
  -h, --help            show this help message and exit
  -g str, --greeting str
                        The greeting (default: Howdy)
  -n str, --name str    Whom to greet (default: Stranger)
  -e, --excited         Include an exclamation point (default: False)
```

When run with no arguments, it should use the default values to print the following:

```
$ ./salutations.py
Howdy, Stranger.
```

The `-g|--greeting` option should cause it to use the provided greeting:

```
$ ./salutations.py -g Sup
Sup, Stranger.
```

The `-n|--name` option should cause it to use the provided name:

```
$ ./salutations.py -n Amanda
Howdy, Amanda.
```

The `-e|--excited` flag should cause the greeting to end with a bang:

```
$ ./salutations.py -e
Howdy, Stranger!
```

The program should accept any combination of the short or long names of the arguments:

```
$ ./salutations.py --greeting Sup --name Dude --excited
Sup, Dude!
```
