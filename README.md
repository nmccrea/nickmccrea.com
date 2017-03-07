# nickmccrea.com

This site is built with [Jekyll](https://jekyllrb.com/), to be hosted on [GitHub Pages](https://pages.github.com/).

GitHub Pages sites are hosted in GitHub repositories following one of the specific repository-and-branch naming patterns described [here](https://help.github.com/articles/user-organization-and-project-pages/). In the case of nickmccrea.com, the site is hosted in a repository with the naming pattern `USERNAME.github.io`.

A dedicated deployment repository is used. To deploy, create a new repository in GitHub named `USERNAME.github.io`. In your development machine, add the deployment repository as a remote repository for your project:

```
git remote add deploy git@github.com:USERNAME/USERNAME.github.io.git
```

To deploy, simply push to this deployment repository:

```
git push deploy master
```

If the build is successful, the site will be available at `http://USERNAME.github.io`. To learn about using custom domain names with GitHub pages, start [here](https://help.github.com/articles/using-a-custom-domain-with-github-pages/).