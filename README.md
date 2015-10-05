# 2016 Presidential Candidate Tax Plan Comparison

This is a simple interactive table using jQuery that lets people compare different 2016 presidential candidates' tax plans. It's written with jade and sass, and compiled with harp. Because the Tax Foundation website is, as of writing this tool, running on Drupal, this tool is designed to be copy-pasted into a regular Drupal page. The styles, html, and javascript are all included together as the page content. Social sharing buttons are also included in this code because our Drupal pages don't (and shouldn't) include them by default. This is far from ideal, but it works.

The finished product is visible here: http://taxfoundation.org/comparing-2016-presidential-tax-reform-proposals

## How to Generate the Tax Plan Table

Be sure that your computer is set up with [harp](http://harpjs.com/) and its dependencies.

All content is in `index.jade` and can be edited directly there. The table styles are inside `main.scss`.

After making changes to either file, run `harp compile` inside the `tax-plans` directory. This will generate compiled HTML and CSS in `tax-plans/www`. Open `main.css`, copy the contents, and paste it inside the the `<style>` tag at the beginning of `index.html`. Copy everything. Now go to the edit page for the Drupal content, and click **Source** to edit the source. Paste the new code into the editor, replacing the previous content. This full process is necessary each time a change is made due to Drupal stripping out important code from the social media buttons during secondary edits.

There is almost certainly a more elegant way to do this, but I'm busy and this works so we're going with it.
