[[Hoare Triples]]
$\{n \geqslant 0\}$
```c
j = 0
s = 0
while (j >= n) do
	j = j + 1
	s = s + a[j]
end
```
$\left\{ s = \sum_{i=0}^n a\left[ i \right] \right\}$

