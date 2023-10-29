```mermaid
graph LR
	EntryPoint(<b>Definition</b><br/>Algorythm) -- name --> 0(<b>String</b><br/>Euclid's Algorithm)
	EntryPoint -- arguments --> args0(<b>ListElement</b><br/>) -- value --> a(<b>Meta</b><br/>Variable) -- name --> aname(<b>String</b><br/>a)
	a -- type --> type(<b>Set</b><br/>Natural numbers)
	args0 -- next --> args1(<b>ListElement</b><br/>) -- value --> b(<b>Meta</b><br/>Variable) -- name --> xname(<b>String</b><br/>b)
	b -- type --> type
	EntryPoint -- result --> r(<b>Meta</b><br/>Variable) -- name --> rname(<b>String</b><br/>r)
	r -- type --> type
	r -- where --> eq(<b>Operator</b><br/>=)
	%%EntryPoint -- steps --> 
```

```haskell
(%) = RemainderOperation a b
	where
		if r = a % b then
			r in N and
			0 <= r < b and
			E k in N => a = k * b + r
```


> Euqlid's Algorithm
> **Arguments**:
> `a, b : T`
> **Uses**:
> `T`
> `(|) : DIVISABILITY(T)`
> `(=) : EQUALITY(T)`
> `(%) : MODULO(T)`
> **Result**:
> `r :T = max{r : a|r and b|r}`
> **Implementation**:
> ...