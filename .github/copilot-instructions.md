## Project summary

- This repository contains notes and quick-start steps for learning Jekyll. It is not a full blog site; the only discoverable file is `README.md` which lists Ruby/Jekyll install and run commands.

## What an AI agent should know up front

- This is a simple learning repo focused on local Jekyll development. The **primary workflow** is creating a new Jekyll site and running it locally using Bundler. See `README.md` for the existing commands.
- Common commands to run (Windows PowerShell):

```powershell
# install gems (if needed)
gem install jekyll bundler

# create a new site
jekyll new myblog
cd myblog

# serve locally with livereload
bundle exec jekyll serve --livereload
```

## Project-specific guidelines for Copilot / AI agents

1. Preserve `README.md` content: it contains the authoritative local setup notes and package recommendations used by the repository owner. If you automate or change setup steps, add a short, explicit note to `README.md` describing why.
2. When adding a Jekyll site, follow Jekyll's default structure: `/_layouts`, `/_includes`, `/assets` and a `_config.yml` file. If you introduce a Gemfile, use Bundler and include `Gemfile.lock` for reproducibility.
3. The `README.md` asks "what is the use of `bundle add webrick`?" — include an explanation in proposals or PR descriptions if you add `webrick` as a dependency: Ruby 3.0 removed the stdlib WEBrick server, so adding it explicitly avoids server errors on newer Ruby.

## Troubleshooting & debugging tips (detectable from repo context)

- To debug site build or plugin issues, run `bundle exec jekyll build --trace` or `bundle exec jekyll serve --trace` to get a Ruby stack trace. Use `jekyll doctor` to spot common misconfigurations.
- Check the `_site` output folder after successful build; if missing files appear in the browser, inspect `_config.yml` or plugin entries in `Gemfile`.

## Suggested Pull Request behavior for changes

- Keep changes small and focused. For updates to `README.md`, add a short example that reproduces the change locally (commands and expected output).
- If you add a Jekyll blog or example site in the repository, include a minimal `.gitignore` that excludes `_site` and system-specific files.

## Where to look for further context

- `README.md` — existing setup and goals (primary source for local usage)
- Jekyll docs (https://jekyllrb.com/docs/) — authoritative behavior for site structure and commands

If anything in these instructions is unclear or you want the file to be more aggressive in enforcing repository rules, tell me where to expand and I'll iterate.