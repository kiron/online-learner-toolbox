The content of this Toolbox can be edited locally or directly here on GitHub with any Markdown editor or in a plain text editor.

### Editing the Toolbox locally

When you are ready to continue with the following procedure:

1. Install mkdocs as described [here](http://www.mkdocs.org/#installation).
2. Install the material theme for mkdocs has described [here](http://squidfunk.github.io/mkdocs-material/getting-started/).
3. Clone this repository to your local computer.
4. Open your terminal and navigate into the `online-learner-toolbox`.
5. Run `mkdocs serve` to view the Toolbox locally.
6. Edit the `.md`files within `.../docs` to change the content of the Toolbox.
7. Rund `mkdocs build` to build the Toolbox with the new content locally.
8. Push your changes to the repository.

###Universal Google Analytics tracking:

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
