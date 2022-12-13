# Linux ANSI Code

This package installs a library that defines a function to use human-readable [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code).

## Usage
Instead of writing this:
```bash
echo -e "\e[1;3;91mThis text is written in bold, bright red, italic letters on the command line.\e[0m"
```
You write this:
```bash
source /usr/local/lib/ansicode.sh
echo -e "$(ansi_code BOLD BRIGHT_RED ITALIC 'This text is written in bold, bright red, italic letters on the command line.')"
```

## Available Codes

### Text Decoration

* BOLD
* FAINT
* ITALIC
* UNDERLINE 
* BLINK
* FBLINK => fast blink
* REVERSE
* HIDE
* STRIKE
* DUNDERLINE => double underline
* OVERLINE
* NORMAL

### Font Color

* BLACK
* RED
* GREEN
* YELLOW 
* BLUE
* MAGENTA
* CYAN
* WHITE
* BRIGHT_BLACK
* BRIGHT_RED
* BRIGHT_GREEN
* BRIGHT_YELLOW
* BRIGHT_BLUE
* BRIGHT_MAGENTA
* BRIGHT_CYAN
* BRIGHT_WHITE
* COLOR_[X] => [X] is a number between 0 & 255
* COLOR_[X]\_[Y]\_[Z] => [X], [Y] and [Z] are numbers between 0 & 255
* COLOR_DEFAULT

### Background Color

* BLACK_BG
* RED_BG
* GREEN_BG
* YELLOW_BG
* BLUE_BG
* MAGENTA_BG
* CYAN_BG
* WHITE_BG
* BRIGHT_BLACK_BG
* BRIGHT_RED_BG
* BRIGHT_GREEN_BG
* BRIGHT_YELLOW_BG
* BRIGHT_BLUE_BG
* BRIGHT_MAGENTA_BG
* BRIGHT_CYAN_BG
* BRIGHT_WHITE_BG
* COLOR_BG_[X] => [X] is a number between 0 & 255
* COLOR_BG_[X]\_[Y]\_[Z] => [X], [Y] and [Z] are numbers between 0 & 255
* COLOR_BG_DEFAULT

### Miscellaneous

* CODE_[X] => Set to the ANSI escape code number [X]
