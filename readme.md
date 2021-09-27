# MinUnit
## A minimal unit testing framework for C

### Only 3 SLOC!!

```c
#define mu_assert(message, test) do { if (!(test)) return message; } while (0)
#define mu_run_test(test) do { char *message = test(); tests_run++; if (message) return message; } while (0)
extern int tests_run;
```

[Source](https://jera.com/techinfo/jtns/jtn002)
