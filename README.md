# jekyll

- learning jekyll from [jekyllrb.com/docs](https://jekyllrb.com/docs/)
- jekyll is static site generator - it takes a markup doc, uses layouts (?) and creates a static site.
- we can tweak the static sites' look, feel (?), URLs, data displayed & more.

## pre-requisites

- ruby >= 2.7.0
- rubyGems
- gcc & make

## prep

- winget install RubyInstallerTeam.RubyWithDevKit.3.2 (or)
- choco install ruby mingw make -y
- gem install jekyll bundler
- what is the use of `bundle add webrick` ?

## jekyll-101

- jekyll new {myblog}
- cd {myblog}
- bundle exec jekyll serve (or) bundle exec jekyll serve --livereload (or) bundle exec jekyll serve --livereload --incremental

## [ruby-101](https://jekyllrb.com/docs/ruby-101/)
