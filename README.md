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

2. Also add yourself to `phackers.md`:

  ```markdown
  ## [Your Name](username.html)

  * Github: https://github.com/username
  * Website http://yoursite.com
  * Other links: http://otherlinks
  ```

3. Create an orphaned `master` branch and add a `README.md` that will contain your setup:

  ```bash
  git checkout --orphan master
  git rm -rf .
  vim README.md
  git add README.md
  git commit -m "Initial commit"
  git push origin master
  ```

  Check https://github.com/marksteve/use for an example.

4. Go to Settings and set `master` as default branch.

5. Send a pull request and your done.
