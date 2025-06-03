### Multi Line Expression Output CC


```
The result of 5 + 3 is:
8
```

---

### ✅ Version 1: Using a hardcoded value (`8`)

```c
#include <stdio.h>

int main() {
    printf("The result of 5 + 3 is:\n8");
    return 0;
}
```

#### How it works:

* `printf()` prints the full string inside quotes.
* `\n` is an **escape sequence** that inserts a newline.
* So it prints:

  * `The result of 5 + 3 is:` on the first line.
  * Then `8` on the next line.

#### Limitation:

* The number `8` is **hardcoded**—it doesn't actually compute `5 + 3`.

---

### ✅ Version 2: Computes the result of `5 + 3`

```c
#include <stdio.h>

int main() {
    printf("The result of 5 + 3 is:\n%d", 5 + 3);
    return 0;
}
```

#### How it works:

* `%d` is a **format specifier** used to print an integer.
* `5 + 3` is calculated by the compiler at runtime.
* The result (`8`) replaces `%d` when printing.
* `\n` again makes a line break after the first part.

#### Output:

```
The result of 5 + 3 is:
8
```


