# Python questions for interview

1. What is PyPy?
2. What is a difference between tuples and lists?
3. What is the result of `1 / 2`?
4. What is the result of `2 * '5'`?
5. Explain these statements:

    ```python
    word = 'String in Python'
    print word[4], word[0:2], word[2:4], word[:2], word[2:], word[0:]
    print word[:], word[-1], word[:-1]
    ```
6. What is the result of 'ю' + u'я'?
7. Explain this statement:

    ```python
    a = '''123'''
    ```
8. Write the lambda, that returns the summ of a and b.
9. Explain following clause:

    ```python
    @capitalize
    def get_dotted(txt):
        return txt + '.'
    ```
10. Explain following clause:

    ```python
    def six():
        for i in (1, 2, 3, 4, 5, 6):
            yield i
    ```
11. Explain this:

    ```python
    def func(a, *b): print b
    ```
12. Is this code right?:

    ```python
    def func(arg1='', arg2):
        return '%s-%s' % (arg1, arg2)
    ```
13. What can you tell about `range()` vs. `xrange()`?
14. What is a sequence type `set`?
15. What disadvantage has an implementation of threads in CPython (module threading)?
16. What is a clause `if __name__ =='__main__':` used for?
17. What is WSGI?
18. What is middleware?
19. What are prepared statements?
20. What is XSS and how do you prevent it?
21. What is replication, partitioning, sharding?
22. What is the difference between WHERE and HAVING sql statements?
23. What is the name of postgresql's command line client?
24. What is inside of pg_hba.conf (in common)?
