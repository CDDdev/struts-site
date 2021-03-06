# Apache Struts Website

This project is used to update the main Apache Struts website http://struts.apache.org/  
See the [update website documentation](source/updating-website.md) on how to push changes online. 
However as ASF is using aggressive caching, for a while one still may need to forcely reload the page (<kbd>CMD+R</kbd> or <kbd>Shift+F5</kbd>) after changes.

Site is generated by Jekyll and uses pure html either markdown format.
To test website locally you can use the below command:

 > bundle exec jekyll serve -w --trace --host 0.0.0.0

or you can use `Docker` (please install it first) with one of the provided scripts:

 > ./docker-run.fish

when running `fish-shell`, or:

 > ./docker-run.sh

when running `Bash` or `Sh`.

All pages are generated into the `content` folder.

There are two scripts used to build the image but this should be used only when `Dockerfile` was modified.

Some redirect rules are configured in `source/.htaccess` file.
