# Annotation

## Inline Comments

**Don't overuse Inline Comments.**

Inline comments are comments that accompany code statements. Line comments and code must be separated by at least two Spaces. Comments begin with ``//`` and a space.

If the result is obvious, then it should not be added.

## Documentation String

You need to write it in the following format:

```PHP
/**
 * Description Here
 * @type0 content0
 * @type1 content1
 * ...
 */
```

For information on how to fill in "type", please go to [phpDoc](https://www.phpdoc.org/docs/latest/index.html).

## Block Comments

Block Comments are typically used when large amounts of newline text need to be written, such as complex business descriptions and complex internal implementations.

With the exception of the first and last line, the content of every Block comment should begin with '*' and a space.

e.g:

```PHP
/*
* From fairest creatures we desire increase,
* That thereby beauty's rose might never die,
* But as the riper should by time decease,
*/
```

