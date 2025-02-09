summary: Cvičenie 01
id: cvicenie-01
categories: cvicenie
tags: beginner
status: Published
authors: Milan Mladoniczky
feedback link: https://github.com/interes-group/pevs-DSA-BIAX10031/issues

# Cvičenie 01

<!-- ------------------------ -->

## Úvod

Toto cvičenie je zamerané na precvičenie základných konceptov programovania v jazyku C++. Budete pracovať s rôznymi
dátovými typmi, štandardným vstupom a výstupom, dynamickou alokáciou pamäte, poľami, reťazcami,
konštantami a vlastnými funkciami. Cieľom je posilniť ich pochopenie týchto konceptov a pripraviť ich na riešenie
zložitejších problémov.

### Obsah

- štandardný vstup a výstup
- práca s dynamicky alokovanými poliami
- práca s dátovým typom string

> aside negative
> Ak používate ako vývojové prostredie lokálny a editor a následnú kompiláciu cez terminál. Použite príkaz:
> ```shell
> g++ -o program -Wall -Wextra main.cpp
> ```

Pre vypracovanie týchto úloh odporúčam mať funkčné lokálne vývojové prostredie (VS Code, CLion a pod.) a kompilátor
jazyka C++.

> aside negative
> Nezabudnite každú alokovanú pamäť uvoľniť volaním operátorom `delete <premenná>`! Je dôležité si po sebe vždy
> upratať.

Riešenia na jednotlivé úlohy budú uverejnené neskôr.

<!-- ------------------------ -->

## Úloha 1.1

Napíšte program, zdrojový kód, v jazyku C++ použitím štandardu C++17, ktorý realizuje nasledovnú činnosť.

Program načíta celé číslo `n` zo štandardného vstupu a následne načíta `n` celých čísel. Vypočíta ich súčet a priemer (
zaokrúhlený nadol na celé číslo) a vypíše ich na štandardný výstup.

### Príklady vstupov / výstupov programu

#### Vstup

```text
6
5 10 20 30 40 50
```

#### Výstup

```text
Súčet: 150 
Priemer: 30
```

<!-- ------------------------ -->

## Úloha 1.2

Napíšte program, zdrojový kód, v jazyku C++ použitím štandardu C++17, ktorý realizuje nasledovnú činnosť.

Program načíta celé číslo `n`, ktoré predstavuje počet prvkov v poli. Následne alokuje dynamické pole veľkosti `n`,
načíta `n` celých čísel a následne vypíše všetky párne čísla v poradí, v akom boli zadané.

### Príklady vstupov / výstupov programu

#### Vstup

```text
7
6 1 2 3 4 5 6
```

#### Výstup

```text
2 4 6
```

<!-- ------------------------ -->

## Úloha 1.3

Napíšte program, zdrojový kód, v jazyku C++ použitím štandardu C++17, ktorý realizuje nasledovnú činnosť.

Program načíta celé číslo `n` zo štandardného vstupu, ktoré predstavuje počet riadkov a stĺpcov štvorcovej matice.
Následne alokuje dynamickú dvojrozmernú maticu veľkosti `n x n` a načíta do nej celé čísla po riadkoch (t.j. načíta `n`
čísel prvého riadku, potom ďalší atď.). Program potom transponuje túto maticu (vymení riadky za stĺpce) a vypíše
transponovanú maticu na štandardný výstup.

### Príklady vstupov / výstupov programu

#### Vstup

```text
3
3 1 2
3 4 5
6 7 8
```

#### Výstup

```text
3 3 6
1 4 7
2 5 8
```

<!-- ------------------------ -->

## Úloha 1.4

Napíšte program v jazyku C++ použitím štandardu C++17, ktorý realizuje nasledovnú činnosť.

Program načíta reťazec zo štandardného vstupu a zistí, či je tento reťazec palindróm (t.j. číta sa rovnako spredu aj
zozadu). Implementujte funkciu `bool je_palindrom(const std::string& text)`, ktorá vráti hodnotu `true`, ak je reťazec
palindróm, inak vráti `false`. V programe použite vhodné konštanty tam, kde je to potrebné.

### Príklady vstupov / výstupov programu

#### Príklad 1

- Vstup: `radar`
- Výstup: `Reťazec 'radar' je palindróm.`

#### Príklad 2

- Vstup: `programovanie`
- Výstup: `Reťazec 'programovanie' nie je palindróm.`

<!-- ------------------------ -->

## Úloha 1.5

Napíšte program v jazyku C++ použitím štandardu C++17, ktorý realizuje nasledovnú činnosť.

Program načíta dva reťazce zo štandardného vstupu a zistí, či sú tieto reťazce anagramy (t.j. obsahujú rovnaké znaky v
rovnakom počte, ale v rôznom poradí). Implementujte funkciu
`bool su_anagramy(const std::string& prvy, const std::string& druhy)`, ktorá vráti hodnotu `true`, ak sú reťazce
anagramy, inak vráti `false`. V programe použite vhodné konštanty tam, kde je to potrebné.

### Príklady vstupov / výstupov programu

#### Príklad 1

- Vstup: `listen silent`
- Výstup: `Reťazce 'listen' a 'silent' sú anagramy.`

#### Príklad 2

- Vstup: `hello world`
- Výstup: `Reťazce 'hello' a 'world' nie sú anagramy.`

## ✨ Úloha 1.6

Napíšte program v jazyku C++ použitím štandardu C++17, ktorý realizuje nasledovnú činnosť.

Program načíta celé číslo `n` zo štandardného vstupu, ktoré predstavuje počet prvkov v poli. Následne alokuje dynamické
pole veľkosti `n` a načíta do neho `n` celých čísel. Program potom nájde najdlhšiu postupnosť po sebe idúcich prvkov,
ktoré sú v neklesajúcom poradí (každý nasledujúci prvok je rovnaký alebo väčší ako predchádzajúci), a vypíše dĺžku tejto
postupnosti.

### Príklady vstupov / výstupov programu

#### Vstup

```text
11
10 5 3 4 4 5 6 2 2 2 3
```

#### Výstup

```text
Najdlhšia neklesajúca postupnosť má dĺžku: 4
```
