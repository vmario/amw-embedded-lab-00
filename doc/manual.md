---
title: "Instrukcja laboratorium systemów wbudowanych"
subtitle: "Ćwiczenie 0: Pobieranie ćwiczenia i obsługa IDE"
author: [Mariusz Chilmon <<mariusz.chilmon@ctm.gdynia.pl>>]
lang: "pl"
titlepage: yes
titlepage-logo: "logo.jpg"
colorlinks: yes
header-includes: |
  \usepackage{awesomebox}
...

> When the terrain disagrees with the map, trust the terrain.
>
> — _Swiss army proverb_

# Środowisko programistyczne

\begin{description}
\item[Płytka ewaluacyjna]
ATB 1.05A firmy Atnel z mikrokontrolerem ATmega z rodziny AVR. Producentem mikrokontrolerów AVR jest firma Microchip Technologies, która w 2016 r.~przejęła pierwotnego producenta — firmę Atmel.
\item[Kompilator]
AVR Toolchain v3.7 bazujący na kompilatorze GCC.
\item[Programator]
AVRDUDE v7.1.
\item[IDE]
Visual Studio Code (nie mylić z Visual Studio) z wtyczką \textit{C/C++} umożliwiającą nawigowanie po kodzie C i C++ oraz automatyczne uzupełnianie kodu w tych językach.
\item[Katalog roboczy]
\lstinline{Embedded} w katalogu \lstinline{Dokumenty}. Kody źródłowe ćwiczeń należy umieszczać w~\lstinline{Embedded/Core}. W \lstinline{Embedded/Datasheets} umieszczone są noty katalogowe mikrokontrolerów oraz dokumentacja płytki ewaluacyjnej.
\end{description}

# Pobieranie kodu i instrukcji do ćwiczenia

1. Wyczyść zawartość katalogu `Embedded/Core`.
1. Uruchom Visual Studio Code.
1. Wciśnij _Ctrl + Shift + P_ i wpisz polecenie _git clone_.
1. Sklonuj repozytorium Git [https://github.com/vmario/amw-embedded-labXX.git](https://github.com/vmario/amw-embedded-labXX.git), gdzie _XX_ to numer ćwiczenia.
1. Wybierz katalog `Embedded/Code` do zapisania projektu.

# Kompilacja programu

1. Wybierz odpowiedni model mikrokontrolera w prawym dolnym rogu okna programu.
1. Wciśnij _Ctrl + Shift + B_ i wybierz zadanie _all_.

\notebox{Jeżeli zbudowałeś program dla niewłaściwego mikrokontrolera, wyczyść pliki wynikowe zadaniem \textit{clean}.}

# Wgrywanie wsadu

1. Wciśnij _Ctrl + Shift + B_ i wybierz zadanie _program_.

\notebox{Zadanie \textit{program} przebudowuje też program wynikowy, jeżeli zostały wprowadzone jakieś zmiany w plikach źródłowych. Zatem, jeżeli chcesz skompilować program i od razu go wgrać, możesz pominąć zadanie \textit{all}.}

# Opis skonfigurowanych zadań

\begin{description}
\item[all]
Buduje program.
\item[clean]
Czyści wszystkie pliki wynikowe (usuwa efekt kompilacji).
\item[erase]
Czyści pamięć mikrokontrolera.
\item[program]
Buduje program i wgrywa go do mikrokontrolera.
\end{description}
