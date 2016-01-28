# interview-questions
Questions for technical interviews. It contains questions to test python and javascript knowledges.

I have used these questions for interviewing new employes.

## Javascript questions
[Download javascript.docx](https://github.com/lev-veshnyakov/interview-questions/blob/master/javascript.docx?raw=true)

1. How to check is the variable `var1` defined?
2. What does the `document.querySelectorAll` do?
3. How to add the string `"123"` to the local storage of the browser?
4. What is the difference between `jQuery(window).load(...)` and `jQuery(document).ready(...)`?
5. What is the difference between `jQuery('div')[0]` and `jQuery('div').eq(0)`?
6. How to prevent default action from the event handler?
7. What is the event capturing and the event bubbling?
8. What does this css selector 
`.someclass + .button ~ div:not([class^="container"]) > span:last-child` do?
9. Which css selector works faster and why?

    ```css
    .content-button
    .content  .button
    ```
10. What do you know about `display: flex`?
11. What is XSS?
12. What is CSRF?
13. What is the same origin policy?
14. What will the code below output to the console and why?

    ```css
    console.log(1 +  "2" + "2");
    console.log(1 +  +"2" + "2");
    console.log(1 +  -"1" + "2");
    console.log(+"1" +  "1" + "2");
    console.log( "A" - "B" + "2");
    console.log( "A" - "B" + 2);
    ```
15. What is the result of executing this code and why?

    ```css
    function test() {
       console.log(a);
       console.log(foo());
       var a = 1;
       function foo() {
          return 2;
       }
    }
    test();
    ```
16. Consider the following code.

    ```css
    var a;
    (function() {
        var a = b = 5;
    })();
    console.log(a, b);
    ```
What will be printed on the console?
17. What will happen if we add `'use strict'` to this code:

    ```css
    var a;
    (function() {
       'use strict'
        var a = b = 5;
    })();
    console.log(a, b);
    ```
18. What is the result of the following code? Explain your answer.

    ```css
    var name = 'Ivan';
    var obj = {
       name: 'John',
       prop: {
          name: 'Johan',
          getName: function() {
             return this.name;
          }
       }
    };
    console.log(obj.prop.getName());
    var test = obj.prop.getName;
    console.log(test());
    ```
19. Fix the previous question’s issue so that the last `console.log()` prints `'Johan'`.
20. Consider the following code.

    ```css
    var nodes = document.getElementsByTagName('button');
    for (var i = 0; i < nodes.length; i++) {
       nodes[i].addEventListener('click', function() {
          console.log('You clicked element #' + i);
       });
    }
    ```
What will be printed on the console if a user clicks first and fourth button in the list? Why?
21. Fix the previous question’s issue so that the handler prints 0 for the first button in the list, 1 for the second, and so on.
22. Define a repeatify function on the String object. The function accepts an integer that specifies how many times the string has to be repeated. The function returns the string repeated the number of times specified. For example:
`console.log('hello'.repeatify(3))` should print hellohellohello.


# Python questions
[Download python.docx](https://github.com/lev-veshnyakov/interview-questions/blob/master/python.docx?raw=true)

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


