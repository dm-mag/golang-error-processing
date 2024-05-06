# golang-error-processing
my golang error processing

```
func eie(err error) {
  if err != nil {
    log.Fatal(err)
  }
}
func eie2[K any](r K, e error) K {
  eie(e)
  return r
}
.....
data = eie2(os.ReadFile(os.Args[1]))
```
