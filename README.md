This is the sample code to accompany the book *Parallel and Concurrent Programming in Haskell* (Simon Marlow, O'Reilly 2013).

To build the code on your system, you need either:

* [Stack](http://haskellstack.org)
* [A Minimal GHC installation](https://www.haskell.org/downloads)
* [The Haskell Platform](https://www.haskell.org/downloads#platform)

## Building with Stack

```
stack build
```

will build all the executables and install them in a platform-specific
subdirectory under `.stack-work/install`.

## Building with Cabal new-build

```
cabal new-build
```

## Building with Cabal

```
cabal sandbox init
cabal install --only-dependencies
cabal configure
cabal build
```
## 추천하는 GHC 버전 8.8.4
 - 요구하는 base 라이브러리의 버전 범위(>=4.5 && <4.14)
 - GHC 8.8.4에서 4.13 base 라이브러리 사용
   
```
ghcup install ghc 8.8.4
ghcup set ghc 8.8.4
cabal clean
cabal build
```
