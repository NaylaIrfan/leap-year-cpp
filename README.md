# leap-year-cpp

# Leap Year Checker (C++)

A beginner-friendly C++ program that checks whether a year entered by the user is a leap year or not.

## About

The program reads a year and uses the leap year rules to decide whether it is a leap year. It prints the result on the screen.

## Leap Year Rules

A year is a leap year if either of these is true:

1. It is divisible by **400** (for example, 2000).
2. It is divisible by **4** but **not** by 100 (for example, 2024).

| Year | Divisible by 4 | Divisible by 100 | Divisible by 400 | Leap year? |
|------|----------------|------------------|------------------|------------|
| 2024 | Yes | No | No | Yes |
| 1900 | Yes | Yes | No | No |
| 2000 | Yes | Yes | Yes | Yes |
| 2023 | No | No | No | No |

## Examples

```
Enter a year: 2024
2024 is a leap year.
```

```
Enter a year: 1900
1900 is not a leap year.
```

```
Enter a year: 2000
2000 is a leap year.
```

## How It Works

1. Read the year using `cin`.
2. Check the condition `(year % 400 == 0) || (year % 4 == 0 && year % 100 != 0)`.
3. If the condition is true, print that it is a leap year.
4. Otherwise, print that it is not a leap year.

## Things to Note

- The `%` (modulus) operator gives the remainder. A remainder of 0 means the number divides exactly.
- Checking only "divisible by 4" is not enough, because years like 1900 are divisible by 4 but are not leap years.

## Concepts Used

- Data types (`int`)
- Input and output (`cin`, `cout`)
- `if` / `else` conditions
- Modulus operator (`%`)
- Logical operators (`&&`, `||`)

## How to Run

Make sure a C++ compiler such as `g++` is installed.

```bash
# Compile
g++ leap_year.cpp -o leap_year

# Run (Linux / macOS)
./leap_year

# Run (Windows)
leap_year.exe
```

## Project Structure

```
leap-year-cpp/
├── README.md
└── leap_year.cpp
```

## Author

NAYLA IRFAN
B.Tech CSE
## License

This project is free to use for learning purposes.
