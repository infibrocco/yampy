![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/infibrocco/parsematic/python-package.yml)
![GitHub License](https://img.shields.io/github/license/infibrocco/parsematic)
![GitHub repo size](https://img.shields.io/github/repo-size/infibrocco/parsematic)
![LOc](https://sloc.xyz/github/infibrocco/parsematic/)
![GitHub Repo stars](https://img.shields.io/github/stars/infibrocco/parsematic)


# Parsematic

This is a basic math parser that can parse mathematical expressions.

## Features

Parses a variety of mathematical expressions, including:

- Integers `(0, 1, 5, -7)`, Floats `(3.14159, 2.7, 0.5)`

- Basic arithmetic operations `(+, -, \*, /, \*\*, //, %)`

- Comparison operators `(==, !=, <, >, <=, >=)`

- Parentheses for grouping

- Mathematical functions `(sin, cos, tan, abs, sqrt, log, fact, gcd, lcm, xor, int, float, min, max)`

## Usage

First, install it with:

```
pip install parsematic
```

Import the MathParser class:

```Python
from math_parser import MathParser
```

Create a MathParser instance:

```Python
parser = MathParser()
```

Use the parse() method to parse and evaluate an expression:

```Python
result = parser.parse("2 + 3 * (4 - 1)")
print(result) # Output: 11
```

Or, use it from the command line

```Python
python -m parsematic "2 + 3 * (4 - 1)"
```

Supported Operators:

- Arithmetic operators: `+, -, \_, / (true division), // (floor division), \*\* (exponentiation), % (modulo)`
- Comparison operators: `==, !=, <, >, <=, >=`
- Supported Functions
  `sin, cos, tan, abs, sqrt, log,
fact (factorial),
gcd (greatest common divisor),
lcm (least common multiple),
xor (bitwise exclusive or),
int, float (type conversions),
min, max`

## Error Handling

The parser will raise exceptions for invalid syntax or unsupported operations.

Additional Notes
The parser does not currently support variables or user-defined functions.

## Contributing

Pull requests are welcome!
