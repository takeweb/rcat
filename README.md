# rcat

* cat command witten by rust

## Installation

```
cargo install --path .
```

## Uninstallation

```
cargo uninstall rcat
```

## Example for args one file
```
% rcat tests/inputs/fox.txt

The quick brown fox jumps over the lazy dog.
```

## Example for args some file
```
% rcat tests/inputs/*.txt

The quick brown fox jumps over the lazy dog.
Don't worry, spiders,
I keep house
casually.
The bustle in a house
The morning after death
Is solemnest of industries
Enacted upon earth,—

The sweeping up the heart,
And putting love away
We shall not want to use again
Until eternity.
```

## Example for args standard input
```
% rcat < tests/inputs/fox.txt

The quick brown fox jumps over the lazy dog.
```

## Example for args pipe standard input
```
cat tests/inputs/fox.txt | rcat

The quick brown fox jumps over the lazy dog.
```

## Example for args one file with -n
```
% rcat -n tests/inputs/spiders.txt

     1  Don't worry, spiders,
     2  I keep house
     3  casually.
```

## 引数あり(-b)で実行
```
% rcat -b tests/inputs/the-bustle.txt

     1  The bustle in a house
     2  The morning after death
     3  Is solemnest of industries
     4  Enacted upon earth,—

     5  The sweeping up the heart,
     6  And putting love away
     7  We shall not want to use again
     8  Until eternity.
```