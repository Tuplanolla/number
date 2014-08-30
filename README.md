# Number

## 1   Explanation

This script numbers sections in a Markdown document.

### 1.1   Note

It also removes said numbers.

### 1.2   Another Note

You can use it on any other document that uses `#`s to denote headings too.

## 2   Purpose

Sometimes you might not want to install and
configure a complete Markdown system just to number a few sections.

## 3   Usage

The `example` file shows how it works.

### 3.1   Synopsis

There are two scripts

	number [depth] [separator]
	denumber [depth] [separator]

that process the sections beyond a certain `depth` and
use a `separator` between their numbers and titles.

### 3.2   Defaults

If the parameters are omitted, then
`depth` is assumed to be `0` and
`separator` to be `   ` (a nonbreaking space surrounded by spaces).

### 3.3   Errors

Orphaned sections are given the number `0`.

## 4   Other Things

### 4.1   Author

This project was written by Sampsa "Tuplanolla" Kiiskinen on 2014-08-31.

### 4.2   License

It is licensed under the GNU General Public License version 3 or later.

### 4.3   Implementation

The code is written in Ruby and works like a shell script.

#### 4.3.1   Remark

It is trivial.

## 5   Hint

The script was used to number these sections automatically.

	cat README.md | ./number 1
