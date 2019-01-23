```
cabal build
# will fail
ghc Use.hs 
# also fails
ghc -package-db dist/package.conf.inplace Use.hs
# comment out `lib irritant` in `test.cabal`.
cabal build
# succeeds
ghc -package-db dist/package.conf.inplace Use.hs
```

