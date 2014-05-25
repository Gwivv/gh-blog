gh-blog
===

This is a blog for GitHub pages. You just have to fork this project and modify the configurations files to have your **own** blog.

Structure for personalize **your** blog :
---

All files you have to modify are in folder **config** :
```
config
|---json
    |---site.json       -> site configuration (title,logo,photo,description...)
    |---skills.json     -> your skills for displaying on home and cv
    |---cv.json         -> your cv experiences and formations
    |---blog.json       -> the list of your blog articles
|---md
    |---blog            -> articles
|---styles
    |---theme.css       -> the css for customize theme
```


Personalize your picture
---
You have three choices for your picture :

1. An image in the folder **images** :
    ```
    "photo": {
        "img":"/images/me.jpg"
    }
    ```
2. Your **GitHub's username** :
    ```
    "photo": {
        "github":"github"
    }
    ```

3. Or your **gravatar mail** :
    ```
    "photo": {
        "gravatar":"github@mail.com"
    }
    ```

More informations about the project
---

 * Use of [Angular.JS][1] version 1.2.15.
 * Use of [Markdown][2] for articles.
 * Use of [Disqus][3] for comments.
 * Customisation by JSON files.
 * Generated with Node.JS and Grunt/Bower/Yo.

License
---
The MIT License (MIT)

Copyright (c) 2014

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

 [1]: https://angularjs.org/
 [2]: http://fr.wikipedia.org/wiki/Markdown
 [3]: http://disqus.com/