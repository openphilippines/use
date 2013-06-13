# Phackers Use

What Pinoy Tech Hackers use.

## Adding yourself

1. Fork phackers/use and add a `username.html` file containing this:

  ```html
  ---
  layout: default
  ---

  <script>
  Flatdoc.run({
    fetcher: Flatdoc.github('username/use')
  });
  </script>
  ```

2. Add yourself to `phackers.md`:

  ```markdown
  ## [Your Name](username.html)

  * Github: https://github.com/username
  * Website http://yoursite.com
  * Other links: http://otherlinks
  ```

3. Send a pull request.

4. Create an orphan `master` branch and add a `README.md` that will contain your setup:

  ```bash
  git checkout --orphan master
  git rm -rf .
  vim README.md
  git add README.md
  git commit -m "Initial commit"
  git push origin master
  ```

  Check https://github.com/marksteve/use for an example.

5. Go to Settings and set `master` as default branch. You're done!

Note that you do the pull request with the `gh-pages` branch. Your `master`
branch is your own. Its readme is fetched by Flatdoc dynamically, making it
possible for you to update your setup without waiting for pull requests to be
approved and merged.

## Powered by

* Flatdoc by @rstacruz
* Jekyll by @mojombo
* Github Pages
