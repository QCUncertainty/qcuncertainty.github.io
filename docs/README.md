# QCUncertainty Project Website

## Building the Website Locally

GitHub pages is designed for use with Jekyll, which is a ruby package for
building static websites using GitHub flavored markdown. Don't worry you
shouldn't need to know ruby at any stage of website maintenance as long as you
follow these command-line instructions:

1. Ensure `ruby-bundler` is installed. On Ubuntu this is done by:

   ```.sh
   sudo apt install ruby-dev ruby-bundler
   ```

2. Clone this repo, i.e.,

   ```.sh
   git clone https://github.com/QCUncertainty/qcuncertainty.github.io
   ```

3. Install the dependencies via bundler. This is done by:

   ```.sh
   cd qcuncertainty.github.io/docs
   bundle config set path 'vendor/bundle'
   bundle install
   ```

4. Launch the website server via:

   ```.sh
   bundle exec jekyll serve
   ```

5. View the website by following the instructions from the previous command (
   should be something like opening http://127.0.0.1:4000 in a web browser).

6. Start adding/modifying content. The local copy of the website should
   automatically update after you modify a file. You will likely need to reload
   the page to see the changes. The caveat to this is if you modify
   `docs/_config.yml`; if you modify that file you will have to stop the current
   server and repeat step 4.
