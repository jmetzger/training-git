# git checkout 

## Checkout (change to) existing branch 

```
git checkout feature/4711
```

## Checkout and create branch 

```
# Only possible once 
git checkout -b feature/4712
```

## Checkout branch auf Basis eines tags 

```
git checkout -b lookaround v1.0-prod
```

## Checkout branch auf Basis eines Commits 

```
git checkout -b lookaround 31bc 
```

## File aus einem Commit holen (oder HEAD) 

```
git checkout HEAD -- todo.txt
```
