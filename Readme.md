Minimal repro for `clojure -X` misreporting FileNotFoundException. 

```sh
bash-3.2$ clojure -X main/-main
finished loading main
Namespace could not be loaded: main
```

This behavior differs from -M

```sh
bash-3.2$ clojure -M -m main
finished loading main
Execution error (FileNotFoundException) at main/-main (main.clj:4).
null

Full report at:
/var/folders/fk/l27d_8g52450jh4m7_dhqkr00000gn/T/clojure-16350436886037263655.edn
```
