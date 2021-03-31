
# website setup

## notes on how I set this up

```
 1663  3/31/2021 11:09  gem install jekyll bundler
 1664  3/31/2021 11:09  jekyll new gde-jekyll
 1665  3/31/2021 11:09  cd gde-jekyll
 1666  3/31/2021 11:10  bundle exec jekyll serve
```


```
  $ bundle exec jekyll serve
Configuration file: /home/knerr/repos/gde-jekyll/_config.yml
            Source: /home/knerr/repos/gde-jekyll
       Destination: /home/knerr/repos/gde-jekyll/_site
 Incremental build: disabled. Enable with --incremental
      Generating...
       Jekyll Feed: Generating feed for posts
                    done in 0.158 seconds.
 Auto-regeneration: enabled for '/home/knerr/repos/gde-jekyll'
    Server address: http://127.0.0.1:4000/
  Server running... press ctrl-c to stop.
[2021-03-31 11:28:11] ERROR `/favicon.ico' not found.
```

## things to do

 - set up skeleton site
     > nav bar: home links webmail mytrilog
     > image: dogs/etc
     > footer: gbaddr, sk blog, eff, storygraph, etc
 - play with css/styling/themes, get it to look reasonable
 - set up autodeploy to gde

## more stuff I did...

```
   scp favicon.png from another server
   ln -s favicon.png favicon.ico
   vim links.markdown
   (added stuff here, Links automatically added to nav bar)
   vim _config.yml
   (changed some settings here)
   bundle exec jekyll serve
   gem list
   gem environment
   bundle info minima
   sudo gem uninstall minima
   (had a globally-installed version I didn't want)
   cp links.markdown webmail.markdown
   vim webmail.markdown
   (trying to make nav-bar link point to external url)
   cp webmail.markdown mytrilog.markdown
   vim mytrilog.markdown
   (same)
   mkdir assets
   cd assets
   mkdir images
   cd images
   mv ~/lily-chair.jpg lily-chair.jpg
   vim index.markdown
   (added lily-chair image)
   cd assets
   cp ~/gems/gems/minima-reboot-1.0.30/assets/main.scss .
   vim main.scss
   bundle exec jekyll serve
   vim assets/main.scss
   (added test header & footer colors)
   vim README.md
```

- made new empty git repo
- cloned it to my linux computer
- moved all of my gde-jekyll stuff into this new cloned empty repo
- git added everything (including the .gitignore file)
- pushed it back to main branch on github

