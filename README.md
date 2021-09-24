[![Go Report Card](https://goreportcard.com/badge/github.com/LixvYang/Monkey)](https://goreportcard.com/report/github.com/LixvYang/Monkey)
[![license](https://img.shields.io/github/license/lixvyang/monkey.svg)](https://img.shields.io/badge/LICENSE-MIT-brightgreen.svg)
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/lixvyang/monkey)

- [Monkey](#monkey)
    - [My changes](#my-changes)
  - [Installation](#installation)
- [1 Usage](#1-usage)
- [2 Syntax](#2-syntax)
  - [2.1 Definitions](#21-definitions)
- [LIXIN](#lixin)

# Monkey
Thanks powerful book 《Write an Interpreter in Go》 I complete an interpreter for Monkey programminglanguage.

If you are favorite this repository,Click a :star: in the upper right corner please.

### My changes

The original repository has a high degree of scalability.I did it:
- Add built-in function.
- Add single-line && multi-line comment.
- Add postfix operators(i++...)

## Installation
You can install binary release at right-> **Init Monkey language state** for init realase.

Or, you can install from source like so:

```
#clone this repo
git clone https://github.com/lixvyang/monkey

cd monkey
go install
go build
```

# 1 Usage
```
❯ ./monkey
Hello ! This is the Monkey programming language!
Feel free to type in commands
>> let fib = fn(x){if(x<2){return x;}else{return fib(x-1) + fib(x-2);}};
>> fib(30)
832040
```
# 2 Syntax

## 2.1 Definitions
Variables are defined using the `let` keyword, with each line ending with `;`.
```js
let a = 3;
```
Variables may be integers, floats, strings, or arrays/hashes.

Variables may be updated without the need for `let`, for example this works as you would expect:
```
    let world = "Earth";
    world = "world";
    puts( "Hello, " + world + "!\n");
```


# LIXIN