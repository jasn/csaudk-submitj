Balanced parenthesis checking
=============================

**Task ID: `"dyck"`**

**Last updated: 3 October 2017, 9:40**

In this problem, the input to your program is an array of N characters,
each of which is either `(`, `)`, `[` or `]`,
and your program must return `true` if the parentheses are properly matched,
and `false` if they are not.

For example, the following arrays of parentheses are properly matched:

```
  ( ( ) ( ) ) [ ]
  [ ( ( ( ) ) [ ] ) ]
  [ [ ] ] ( )
  [ [ ] [ [ ] ] ]
  ( ) [ ( [ ] ) ] [ ]
```

The following array is NOT properly matched since the round parentheses are not aligned:

```
  ( [ ] (
```

The following array is NOT properly matched since the square parentheses do not face each other:

```
  ( ] [ )
```

The following array is NOT properly matched since the round parenthesis matches a square parenthesis:

```
  ( [ ] ]
```

The following array is NOT properly matched since the round parenthesis intersect the square parentheses:

```
  ( [ ) ]
```

**Concretely,** you should use the skeleton
<a href="https://github.com/Mortal/csaudk-submitj/raw/master/tasks/dyck/Dyck.java">
`Dyck.java`</a>
and the
<a href="https://github.com/Mortal/csaudk-submitj/raw/master/Submit.java">
`Submit` program</a>
inside BlueJ (right click and choose "Save link as").
You must implement the method `checkParentheses` in `Dyck`
which takes an `ArrayList<Character>` and returns a `boolean`.

You may assume that the input only contains the characters `'('`, `')'`, `'['`, `']'`,
so you do not have to check if there are any other kinds of characters in the input.

**Hint:** Use a stack containing the open parentheses.

**Scoring:**

  * 1 point for correct algorithm
