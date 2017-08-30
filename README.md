The content of this Toolbox can be edited locally or directly here on GitHub with any Markdown editor or in a plain text editor.

### Editing the Toolbox locally

When you are ready to continue with the following procedure:

1. Install mkdocs as described by running `pip install mkdocs && mkdocs --version`. The last line of the output should look something like this: `mkdocs, version 0.16.3`. A detailed explanation on how to install MkDocs can be found [here](http://www.mkdocs.org/#installation).
2. Install the material theme for MkDocs by running `pip install mkdocs-material`. the last output line should like something like this: `Successfully installed mkdocs-material-1.9.0 pygments-2.2.0`. A detailed explanation on how to install Material for MkDocs can be found [here](http://squidfunk.github.io/mkdocs-material/getting-started/).
3. Install the Python-Markdown extension `markdown-include` by running `pip install markdown-include`.
4. Install  PyMdown extensions by running `pip install pymdown-extensions`.
5. Clone this repository to your local computer.
6. Open your terminal and navigate into the `online-learner-toolbox`.
7. Run `mkdocs serve` to view the Toolbox locally.
8. Edit the `.md`files within `.../docs` to change the content of the Toolbox.
9. Rund `mkdocs build` to build the Toolbox with the new content locally.
10. Push your changes to the repository.

### Universal Google Analytics tracking

The toolbox is equipped with a Universal Google Analytics tracking code for cross side tracking. It's located in the `~/online-learner-toolbox/mkdocs-material/material/base.html` file. 

```javascript
<script>
            (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
            (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
            m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
            })(window,document,'script','https://www.google-analytics.com/analytics.js','ga');


            // Connect with the master Kiron GA key
            ga('create', 'UA-67248439-8', 'auto');

            // allow for cross-domain linking
            ga('require', 'linker');

            //list all kiron domains
            ga('linker:autoLink', ['kiron.ngo','support.kiron.ngo', 'apply.kiron.ngo', 'buddy.kiron.ngo', 'campus.kiron.ngo', 'survey.kiron.ngo', 'forum.kiron.ngo'] );

            // Set IP tracking to anonymize #germanlaw
            ga('set', 'anonymizeIp', true);

            // Track this initial page load
            ga('send', 'pageview');
</script>
```

### Troubleshoothing

Python and pip are sometimes a fucking nightmare on OSX. In case you are running into any kind of trouble with those two, stick to the following procedure: 

1. Uninstall/Remove Python 2.7 dependencies by following this procedure: [https://stackoverflow.com/a/3819829](https://stackoverflow.com/a/3819829)
2. Install Python 3.x by downloading it from python.org [python.org](https://www.python.org/downloads/)
3. Upgrade pip to the latest version by running `sudo pip install --upgrade pip`.
4. Follow the installation procedure above again.
5. Be happy :boom: