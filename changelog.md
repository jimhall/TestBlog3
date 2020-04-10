# Sources:
- https://github.com/tocttou/hacker-blog

# Wed Apr  8 13:23:16 EDT 2020 
- _config.yml file
    - Went from theme -> remote_theme (see:
      https://github.blog/2017-11-29-use-any-theme-with-github-pages/)
    - Added show_excerpts
    - Added author & email, changed title
- Moved over _includes files:
    - footer.html
    - head.html
    - header.html
    - social.html
- Moved over _layouts
    - default.html
    - post.html
 - Moved over assets
    - minima-social-icons.svg
 - Changed location in footer.html of minima-social-icons.svg to
   /assets/images
 
# Wed Apr  8 14:28:29 EDT 2020
- Changed layout keyword from default2 -> default
- Moved over sample posts

# Wed Apr  8 15:33:43 EDT 2020  
- Changed _includes/footer.html twitter icon file location
- Changed _includes/header.html rss icon file location
- Uncommented copyright logic in footer.html

# Wed Apr  8 16:31:10 EDT 2020
- Changed footer.html
    - .social-media-list li:last-of-type  margin-right:0 -> margin-right:40px
    - footer h2 -> commented out width

# Wed Apr  8 17:50:59 EDT 2020
- Trying to create a _sass/jekyll-theme-hacker-jimhall.scss
    - adding import statement to jekyll-theme-hacker
    - adding test css format
    - That worked moved styles in footer.html to _sass/jekyll-theme-hacker-jimhall.scss
    - Removed space between / and title @ header h1:before in
      _sass/jekyll-theme-hacker.scss
    - Migrated header.html css to _sass/jekyll-theme-hacker-jimhall.scss
    - Then deleted css in footer.html and header.html
    - NOTE: social-media* elements stolen from the minima theme @
    https://github.com/jekyll/minima

# Thu Apr  9 16:17:22 EDT 2020 (RSS changeset)
- Trying to add RSS // feed.xml using jekyll-feed
    - See https://dzhavat.github.io/2020/01/19/adding-an-rss-feed-to-github-pages.html
    - https://github.com/jekyll/jekyll-feed/releases
    - https://pages.github.com/versions/
- Changes to head.html
    - See See https://github.com/jekyll/jekyll-feed#meta-tags
    - Changed atom.xml -> feed.xml for defaults of jekyll plug-in


