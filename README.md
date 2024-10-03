# pythonWebPrj1



How did that happen:
* Created new repository on GitHub
* Cloned repository to local
* Created new *test1* branch
* Created venv
* Installed mkdocs to venv
* Used *mkdocs new* and mkdocs serve
* Server is up at 127.0.0.1:8000

* Enabled GitHub Pages for the repo on GH
* Created docs/index.md as the source for site page
* Created .github/workflows/actions.yml for GH actions configuration
* Added to actions.yml job **Build and Deploy** with following steps:
  * Checkout
  * Python Setup
  * MkDocs Setup
  * Build
  * Deploy
    * Uses *mkdocs gh-deploy --force*
* Did not work, created Enviroment and Repository secrets on GH
* Did not work, added ```permissions:
  contents: write
  pages: write``` to actions.yml

* On any push GH builds site at https://zombe2203.github.io/pythonWebPrj1/ using MkDocs