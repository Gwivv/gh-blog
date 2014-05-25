Blog for GitHub
===

This is a blog for GitHub pages. You just have to [fork][0] this project and modify the configurations files to have your **own** blog.

 > First : you have to modify in the **index.html** the line
```html
 <base href="http://gwivv.github.io/gh-blog/">
```
By your own github page url :
```html
 <base href="http://[your.github.username].github.io/gh-blog/">
```

For more informations about gh-pages, go [there][gh-pages].


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
    |---blog            -> articles .md
|---styles
    |---theme.css       -> the css for customize theme
```


The **site.json** file
---

This is the principal file of configuration where you can activate or disable each part of the blog site :
```
"skills":true,
"cv":true,
"blog":true
```

 * If you don't want **skills** on Home / CV, just pass the attribute to false.
 * If you don't want to see menu for **cv** and / or **blog**, just pass the attribute to false.
 * If you don't want **picture** on Home, just delete the **picture** attribute, same for **descriptions**.


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


Your CV
---

Just edit the **cv.json** file.


Your Skills
---

Same, just edit the **skills.json** file.


Write an article
---

Add an entry in the **blog.json** file like example :
```
{
    "id" : "the-id",
    "title": "The title",
    "date" : "05/05/2014", // US format
    "file" : "config/md/blog/2014/05/my.blog.md", // path to the md file
    "visible" : false // use visible to show the article when is ready
}
```

Create a new file to the path and write your article.


Configure Disqus
---

Go to the [site][4] and register a new profile if you want to add disqus to your blog.

And add your username to the **site.json** file :
```
"disqus" : {
    "shortname":"username"
},
```


Customize Markdown text
---

Just change the css file in attribute **cssMarkdown** :
```
"cssMarkdown" : "github.css",
```

 > **Tip** : List of different files are inside folder **/bower_components/highlightjs/styles/**.


More informations about the project
---

 * Use of [Angular.JS][1] version 1.2.15.
 * Use of [Bootstrap CSS][2] for styles.
 * Use of [Markdown][3] for articles.
 * Use of [Disqus][4] for comments.
 * Customisation by JSON files.
 * Generated with Node.JS and Grunt/Bower/Yo.



Sources
---

The sources of project can be found [here][5] and the demo is [here][6].


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

 
 [gh-pages]: https://pages.github.com/
 [0]: https://github.com/Gwivv/gh-blog/fork
 [1]: https://angularjs.org/
 [2]: http://getbootstrap.com/css/
 [3]: http://fr.wikipedia.org/wiki/Markdown
 [4]: http://disqus.com/
 [5]: https://github.com/Gwivv/gh-blog
 [6]: http://gwivv.github.io/gh-blog
