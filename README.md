# [jekyll](https://jekyllrb.com/docs/)

- jekyll is a static site generator (SSG) - it takes a markup doc, uses layouts (?) and creates a static site.
- we can tweak the static sites' look, feel (?), URLs, data displayed & more.

## pre-requisites

- ruby >= 2.7.0
- rubyGems
- gcc & make

## prep (one-off)

- winget install RubyInstallerTeam.RubyWithDevKit.3.2 (or) choco install ruby
- choco install mingw make -y
- gem install jekyll bundler
- what is the use of `bundle add webrick` ?

## jekyll-101

- jekyll new {myblog}
- cd {myblog}
- bundle install (optional)
- bundle exec jekyll serve
  - **flags**: --livereload, --incremental

## [ruby-101](https://jekyllrb.com/docs/ruby-101/)

- since jekyll is written in [Ruby](https://www.ruby-lang.org/en/), it'd be good to learn basics of ruby
- **some ruby terminologies:**
  - **Gems**: a piece of code that we can reuse in other ruby projects. example: jekyll is a Gem.
    - shareable with multiple projects/people.
    - Gems package functionalities specifically like converting a ruby object to JSON, interacting with APIs or Pagination (?)
  - **Gemfile**: a file that contains the list of gems used by our ruby project.
  - **Bundler**: a gem that installs all the gems listed in the Gemfile.
- **Note**: Both Gemfile & Bundler are optional but it is highly recommended because they ensure that, we are running the same version of jekyll & it's plugins across diff env's

## [jekyll-102: jekyll from scratch](https://jekyllrb.com/docs/step-by-step/)

### **1. Setup:**

- `mkdir jekyll-site-name && cd jekyll-site-name` to create a new dir for the new jekyll site project
- `bundle init` to create a new Gemfile to list our project's dependencies
- edit the generated Gemfile to add jekyll as dependency `gem "jekyll"`
- manually create a basic `index.html` landing page for our project
- since jekyll is a SSG (Static Site Generator), we have to build the site before viewing:
  - To build, use `jekyll build` which generates a static website to the current directory as `_site` (or)
  - `jekyll serve` (which automatically builds the site everytime using `jekyll build` internally; for reloading the site post every build add flag `--livereload`)

### **2. Liquid:**

### **3. Front Matter:**

### **4. Layouts:**

### **5. Includes:**

### **6. Data Files:**

### **7. Assets:**

### **8. Blogging:**

### **9. Collections:**

### **10. Deployment:**

## Questions

- What does `jekyll serve` & `bundle exec` or `bundle exec jekyll serve` do?

## Advisory to Read More

- <https://guides.github.com/introduction/git-handbook/>
- <https://jekyllrb.com/docs/configuration/>
- <https://jekyllrb.com/docs/step-by-step/10-deployment/>
- <https://jekyllrb.com/docs/configuration/options/#serve-command-options>
