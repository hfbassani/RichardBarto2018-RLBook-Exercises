### *Exercise 3.3:*

**Give a table analogous to that in Example 3.3, but for p(s 0 , r |s, a). It
should have columns for s, a, s 0 , r, and p(s 0 , r |s, a), and a row for every 4-tuple for which
p(s 0 , r |s, a) > 0.**

---
Resposta 1:

```

|     s    |    a     |    s'       | p(s',r|s,a) |
|----------|----------|-------------|-------------|
| high | search | high | r_{search} | alpha       |
| high | search | low  | r_{search} | 1-alpha     |
| low  | search | high | -3         | 1-beta      |
| low  | search | low  | r_{search} | beta        |
| high | search | high | r_{wait}   | 1           |
| low  | search | low  | r_{wait}   | 1           |
| low  | search | high | 0          | 1           |

```
