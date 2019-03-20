# argparse

```
import argparse

parser = argparse.ArgumentParser(description='A description shown in help.')
```
Add some arguments:
```
parser.add_argument('first_arg', help='This is shown in help')
```
Parse the arguments:
```
args = parser.parse_args()
```

## Possible arguments for `add_argument`
```
add_argument(name or flags...[, action][, nargs][, const][, default][, type][, choices][, required][, help][, metavar][, dest])
```
Define how a single command-line argument should be parsed. In short:

* `name or flags` - Either a name or a list of option strings, e.g. foo or -f, --foo.
* `action` - The basic type of action to be taken when this argument is encountered at the command line.
* `nargs` - The number of command-line arguments that should be consumed.
* `const` - A constant value required by some action and nargs selections.
* `default` - The value produced if the argument is absent from the command line.
* `type` - The type to which the command-line argument should be converted.
* `choices` - A container of the allowable values for the argument.
* `required` - Whether or not the command-line option may be omitted (optionals only).
* `help` - A brief description of what the argument does.
* `metavar` - A name for the argument in usage messages.
* `dest` - The name of the attribute to be added to the object returned by parse_args().

(From https://docs.python.org/3/library/argparse.html)


