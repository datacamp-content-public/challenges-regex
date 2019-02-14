---
title: example_python_challenges
output: html_document
---

## [MC] Choose the right answer

```yaml
type: MultipleChoiceChallenge
key: 115qFYuQ4pPlifqZze0QkDORLwVufanGIfC
```

`@assignment1`
Which command explicitly imports the `pyplot` subpackage from `matplotlib`?

`@assignment2`
Assuming `matplotlib.pyplot` is imported as `plt`, which command displays the current figure?

`@assignment3`
Assuming `matplotlib.pyplot` is imported as `plt`, which command clears the current figure?

`@options1`
- `import matplotlib as pyplot`
- `import pyplot from matplotlib`
- [`import matplotlib.pyplot as plt`]
- `from pyplot import plt`
- `import pyplot as plt`

`@options2`
- `matplotlib.pyplot.show()`
- `matplotlib.show()`
- `pyplot.show()`
- `plt.show`
- [`plt.show()`]

`@options3`
- `matplotlib.pyplot.clear()`
- `plt.clear()`
- `plt.clf`
- `plt.clear`
- [`plt.clf()`]

---

## concatenating lists

```yaml
type: BlanksChallenge
key: 8a565a9166
```

`@context`


`@code1`
```{python}
l1 = {{l1}}
l2 = {{l2}}
print(l1 {{_op}} l2)
```

`@pre_challenge_code`
```{python}
import dccpu.generators as g
```

`@variables`
```yaml
l1:
  - '!expr g.int_vector()'
l2:
  - '!expr g.int_vector()'
op:
  - '+'
```

`@distractors`
```yaml

```

---

## popping lists (2)

```yaml
type: OutputChallenge
key: 6258197972
```

`@context`


`@code1`
```{python}
l1 = {{$l1}}
p = l1.pop()
print(p)
```

`@code2`
```{python}
l1 = {{$l1}}
p = l1.pop({{n}})
print(p)
```

`@pre_challenge_code`
```{python}
import dccpu.generators as g
```

`@variables`
```yaml
l1:
  - '!expr g.int_vector(size=6)'
n:
  - '!expr g.rand_int(hi=5)'
```

---

## regex

```yaml
type: BlanksChallenge
key: 2ab52990f2
```

`@context`
#import re and split with it

`@code1`
```{python}
import __
```

`@code2`
```{python}
# faites de la phrase Ecrivons des regex! Ce sera très pratique. Espérons-le du moins. Pouvez vous trouver 4 phrases, ou alors tous les 22 mots? une string
my_string = "__"
```

`@code3`
```{python}
# trouvez une regex qui vous permettra de couper cette string à chaque fin de phrase
sentence_endings = r"___"
```

`@code4`
```{python}
# splittez
print(re.split(___, my_string))
```

`@pre_challenge_code`
```{python}

```

`@variables`
```yaml

```

`@distractors`
```yaml

```
