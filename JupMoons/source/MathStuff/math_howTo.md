# How to do math in Sphinx

You can use either Markdown or reStructured Text files (.md and .rst). However, there is a bug where Sphinx does not load MathJax unless is sees an .rst file with math in it. So I include both .md and .rst files. 

In the conf.py file, you need to replace this line

``` 
extensions = [
]
```

with this

```
extensions = [
    'sphinx.ext.mathjax'
]
```


## More on math

I could test this more. 
