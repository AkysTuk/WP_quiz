#### 1. You're working in the WordPress code of a philosophy blog.

It should only show posts that:

Have the 'ethics' (id 8) or 'metaphysics' (id 9) category.
Have the 'daily' (id 1) tag.
Which queries will retrieve only the required posts?

(Select all acceptable answers.)

1. [x] `$query = new WP_Query( array( 'tag__in' => array ( 1 ), 'category__in' => array( 8, 9 ) ) );`
2. [ ] `$query = new WP_Query( array( 'tag' => 'one', 'category__in' => array( 8, 9 ) ) );`
3. [ ] `$query = new WP_Query( array( 'category__and' => array( 8, 9 ), 'tag__in' => array( 1 ) ) );`
4. [ ] `$query = new WP_Query( array( 'tag' => 'daily', 'cat' => 'ethics', 'cat' => 'metaphysics' ) );`
5. [x] `$query = new WP_Query( array( 'category_name' => 'ethics, metaphysics', tag => 'daily' ) );`

#### 2. A WordPress theme contains, among other things, all the files listed below. Which of these files will be used to display the homepage after this theme is activated?

1. [ ] page-front.php
2. [x] front-page.php
3. [ ] home.php
4. [ ] index.php

#### 3. You are hosting a WordPress site for veterinary procedures with lots of animal images. The content has 86 WordPress taxonomies related to the respective body parts involved in each procedure.

Recently, the site became very slow in peak hours, when the pictures are requested very often, overloading the network.

Which of the following options are likely to increase the performance of the site enough for the peak hours to be fast again?

1. [x] Add WordPress caching.
2. [x] Use a CDN to distribute the animal images content.
3. [ ] Organize taxonomies to reduce their number.
4. [ ] Split the PHP files so each one deals with just one functionality.
5. [ ] Move the pictures from Image blocks to Cover blocks without enabling the Toggle full height button.

#### 4. A possible way to allow the display of several authors’ names on one post is to ______

1. [ ] update the database
2. [ ] change the admin settings
3. [ ] change the config files
4. [x] use a plugin

#### 5. How can WordPress comments be saved in Markdown format?

1. [ ] `<?php add_filter(«hook_comment_text’, ‘Markdown’); ?>`
2. [ ] WordPress does not support the Markdown format.
3. [x] `<?php add_filter(‘comment_text’, ‘Markdown’); ?>`
4. [ ] `<?php add_filter(‘comments’, ‘Markdown’); ?>`

#### 6. The REST API is a simple way to get data in and out of WordPress over HTTP. Applications using the REST API should be written in which programming language?

1. [ ] PHP
2. [x] any programming language that can make HTTP requests and interpret JSON
3. [ ] Java
4. [ ] Node.js

#### 7. Theme developers can take advantage of the izer API to give users a way to manipulate basic theme settings. The Customizer API is object-oriented and provides four main objects. What are they?

1. [ ] widgets, containers, sections, settings
2. [ ] containers, hooks, settings, styles
3. [ ] panels, blocks, controls, settings
4. [x] panels, sections, controls, settings

#### 8. Which of the following file types is NOT involved in translating WordPress?

1. [ ] .po
2. [x] .pot
3. [ ] .mot
4. [ ] .mo

#### 9. What is the default priority for an action hook or filter?

1. [x] 10
2. [ ] 15
3. [ ] 0
4. [ ] 5

#### 10. What's the primary difference between template tags prefaced with the versus get_the?

1. [ ] Template tags prefaced with the _ don't accept arguments.
2. [ ] Template tags prefaced with the _ can be used directly within a template.
3. [x] Template tags prefaced with the _ display a value. Template tags prefaced with get_the return a value.
4. [ ] Template tags prefaced with the _ return a value. Template tags prefaced with get_the display a value.

#### 11. What is a user role that is unique to WordPress Multisite?

1. [ ] MU Admin
2. [ ] Owner
3. [x] Super Admin
4. [ ] Multisite Master

#### 12. Within the editor, blocks are rendered as JavaScript. How are blocks rendered on the front end of a site?

1. [ ] as plain HTML
2. [x] as a React component
3. [ ] as JavaScript comments
4. [ ] as HTML comments

#### 13. Which of these is NOT a part of the internationalization and localization process?

1. [ ] using a gettext function to wrap translatable strings when writing code
2. [ ] installing/using the WordPress Multilingual Plugin
3. [ ] using a tool like Poedit to parse source code and extract translatable strings into a POT file
4. [x] translators translating the POT file into a PO file, one for each language

#### 14. The REST API provides public data, which is accessible to any client anonymously, as well as private data available only after authentication. How could you ensure that no one can anonymously access site data via the REST API?

1. [ ] Disable the REST API via the site's wp-config.php file.
2. [ ] Use the rest_authentication_errors() filter along with the is_user_logged_in() conditional to limit access to logged in users.
3. [ ] Use the rest_authentication_errors() filter along with cookie authentication to limit access to logged in users.
4. [x] Use the Disable REST API plugin.

#### 15. Which of these snippets represents a wrapper that calls jQuery safely and doesn't require repetitive use of the word "jQuery"?

1. [ ] .

```js
$.ready(function () {
  // do stuff
});
```

2. [ ] .

```js
(function ($) {
  // do stuff
})(jQuery);
```

3. [x] .

```js
$(function () {
  // do stuff
});
```

4. [ ] .

```js
jQuery(function ($) {
  // do stuff
});
```

#### 16. What is the correct order of parameters for the add_action() function?

1. [ ] `add_action( 'example_hook', 'example_function', $accepted_args, $priority )`
2. [ ] `add_action( 'example_function', 'example_hook', $priority, $accepted_args )`
3. [x] `add_action( 'example_hook', 'example_function', $priority, $accepted_args )`
4. [ ] `add_action( 'example_function', 'example_hook', $priority )`

#### 17. You might see this code in a WordPress plugin. What does it do?

```
if ( ! defined( 'ABSPATH' ) ) {
   die;
}
```

- [ ] This is how WordPress detects a plugin's presence. This ensures that the plugin is running from the /wp-content/plugins/ directory. If it is not, the plugin should not run.
- [x] This is a way to prevent naming collisions. ABSPATH is the absolute path to the plugin's directory. If ABSPATH is defined by another WordPress plugin with the same directory slug, the plugin should not run.
- [ ] This is a security measure. ABSPATH is the absolute path to the WordPress directory. If the file is called directly, ABSPATH will not be defined and therefore the plugin should not run.
- [ ] This is a compatibility checker. ABSPATH is defined in WordPress core. The plugin checks that the minimum version of WordPress needed to support the plugin is installed. If it is not, the plugin should not run.

#### 18. Which is a best practice for working with WordPress CSS?

- [ ] Use !important next to styles if they don't give you the result you want.
- [ ] Use hyphens in class names.
- [x] Use spaces to indent each property.
- [ ] Avoid CSS shorthand for proper documentation.

#### 19. What is the difference between an action and a filter?

- [ ] Actions are used to add custom functions and remove WordPress functions. Filters are used to make strings translatable for localization.
- [x] Actions are used to add or remove code at runtime. Filters are used to modify data before it is either displayed in the browser or saved to the database.
- [ ] Actions are used to assign values to variables at runtime. Filters are used to extract data from actions and display it in the browser.
- [ ] Actions are used to add user-inputted data to the database. Filters are used to validate user-inputted data prior to adding it to the database.

#### 20. If you activate or update a plugin and it breaks your site so that you cannot manage it via wp-admin, how can you disable the plugin?

- [x] all of these answers
- [ ] Access the WordPress install via WP-CLI. Run the following command: wp plugin deactivate offending-plugin.
- [ ] Access site files via FTP and navigate to /wp-content/plugins/. Delete the folder of the plugin that you would like to disable or simply rename it.
- [ ] Use phpMyAdmin to change the wp_options table's active_plugins option value to a:0:{}.