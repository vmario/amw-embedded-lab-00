---
title: "Ćwiczenie XX: Szablon"
subtitle: "Instrukcja laboratorium"
footer-left: "Instrukcja laboratorium"
author: [Mariusz Chilmon <<mariusz.chilmon@ctm.gdynia.pl>>]
lang: "pl"
titlepage: yes
titlepage-logo: "logo.png"
logo-width: "70mm"
colorlinks: yes
header-includes: |
  \usepackage{algorithm}
  \usepackage{algpseudocode}
  \usepackage{awesomebox}
  \usepackage{ellipsis}
  \usepackage{lcd}
  \LCDcolors[MidnightBlue]{MidnightBlue!10}{MidnightBlue!80}
  \usepackage[raster]{tcolorbox}
  \usepackage{tikz}
  \usetikzlibrary{positioning}
  \usepackage{xfrac}
...

\lstset{language=[11]C++}

> Blah, blah.
>
> — _X Y_

# Cel ćwiczenia

Celem ćwiczenia jest zapoznanie się z:

* foo,
* bar.

# Uruchomienie programu wyjściowego

1. Podłącz płytkę _LCD Keypad Shield_ do _Arduino Uno_.
1. Pole \textLCD[0]{3}+XYZ+.

# Zadanie podstawowe

Opis.

## Wymagania funkcjonalne

1. Foo.
1. Bar.

## Modyfikacja programu

### Foo

Foo.

### Bar

Bar.

# Zadanie rozszerzone

## Wymagania funkcjonalne

## Modyfikacja programu

# Szablony

\begin{center}
\LCD{2}{16}
    |0123456789012345|
    |0123456789012345|
\captionof{figure}{Wyjściowy stan wyświetlacza}
\end{center}

\awesomebox[purple]{2pt}{\faMicrochip}{purple}{}
\awesomebox[violet]{2pt}{\faBook}{violet}{}
\awesomebox[teal]{2pt}{\faCode}{teal}{}
\awesomebox[gray]{2pt}{\faMonument}{gray}{}

\begin{equation}
a = \frac{b}{c}
\end{equation}

```
cout << "Hello, world!" << endl;
```

\begin{algorithm}
\caption{Tytuł}
\begin{algorithmic}
\If {$a \neq b$}
    \State \Return A\_B
\ElsIf {$c = d$}
    \State $e \gets f$
    \State \Return C\_D
\Else
    \State \dots
\EndIf
\end{algorithmic}
\end{algorithm}
