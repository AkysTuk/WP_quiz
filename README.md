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

#### 21. The WordPress REST API is designed to receive and respond to particular types of requests using basic HTML methods. For example, a request to upload a PHP file into a particular folder on a server might look like the code POST /folder/_file.php. Based on this code, what would you call /folder/_file.php (in REST API terms)?

1. [ ] schema
2. [ ] route
3. [ ] response
4. [x] request

#### 22. Which WP-CLI command would you use to manage the capabilities of a user role?

1. [ ] wp admin
2. [ ] wp manage
3. [ ] wp cap
4. [x] wp role

#### 23. What technique would you use to secure data before rendering it to a user?

1. [ ] escape and sanitize
2. [ ] validate and escape
3. [x] validate and sanitize
4. [ ] escape and secure

#### 24. If your WordPress site is seriously compromised, what is the best course of action to return your site to good health?

1. [ ] Determine the date of the attack and restore your site to a backup point prior to that date.
2. [x] Hire a third-party service to clean up your site because it is difficult for someone who is not a WordPress security expert to find and remove all traces of an attack.
3. [ ] Manually delete suspicious files on the server and delete any database tables that are not core WordPress.
4. [ ] Change your hosting password, your WordPress admin password, and your database password.

**Explanation:** It's not the cheapest, but it's the most reliable. Restoring the backup might not help if you have backdoor scripts installed outside of WP directory.


#### 25. If you wanted to register a custom post type, which hook would you use?

1. [x] register_post_type
2. [ ] add_meta_box
3. [ ] wp_head
4. [ ] init

#### 26. Which of the following is NOT a suggested security improvement for your WordPress website?

1. [ ] The site should communicate with WordPress.org.
2. [ ] Remove inactive themes.
3. [ ] Do not output debug information.
4. [x] WordPress updates are accomplished manually only.

**Explanation:** Communicating with WordPress.org is needed for detecting new versions.

#### 27. The Block API enables developers to register custom blocks in themes or plugins. How would you register a custom block?

1. [ ] Use the registerBlockName() function.
2. [ ] Use the createGutenBlock() function.
3. [ ] Use a block template.
4. [x] Use the registerBlockType() function.

#### 28. Which software development principle, often used in WordPress, aims to reduce the repetition of code?

1. [ ] RRR
2. [ ] WET
3. [x] DRY
4. [ ] KISS

#### 29. In a standard template file, how often does the WordPress Loop run?

1. [ ] It runs once per post in the database.
2. [ ] It runs once.
3. [ ] The Loop doesn't run in template files.
4. [x] It runs once per fetched post.

#### 30. Which is NOT a suggested performance improvement for your WordPress website?

1. [ ] The site should run the most recent version of WordPress.
2. [ ] Remove or inactivate unnecessary plugins.
3. [x] UTF8 is supported.
4. [ ] Choose a very recent version of PHP.

**Explanation:** New versions usually come with speed improvements. Inactivating plugins improves performance. By exclusion, it's UTF8.

#### 31. On a regular WordPress install, what is the difference between transients and the object cache?

1. [x] Transients are persistent and write to the wp_options. The object cache persists only for the particular page load.
2. [ ] Transients are stored in the WordPress database. The object cache is stored on the server where the WordPress install is located.
3. [ ] Transients are available for the duration of a user session and apply to all page components. The object cache is available only for scripts.
4. [ ] Transients persist only for the particular page load. The object cache is persistent and writes to the wp_options table.

#### 32. You can harden your WordPress site security by adding __ to your wp-config.php file?

1. [ ] database usernames and passwords
2. [x] unique keys and salts
3. [ ] accessibility
4. [ ] documentation

#### 33. If you have pretty permalinks enabled on a WordPress site, the REST API index is exposed by appending what to the end of the site URL? (for example, http://example.com/answer/) Note that the index provides information regarding which routes are available for that particular WordPress install.

1. [x] `http://example.com/wp-json/`
2. [ ] `http://example.com/wp-admin/`
3. [ ] `http://example.com/wp-rest/`
4. [ ] `http://example.com/wp-rest-api/`

#### 34. In your wp-config.php file, you've added the following line of code. What does it do?
`define( 'DISALLOW_FILE_EDIT', true );`

1. [ ] prevents any non-admin user from directly editing theme or plugin files
2. [x] disables the theme and plugin editor in the WordPress admin
3. [ ] disables the ability to edit core WordPress files from either within the WordPress admin or via direct file access
4. [ ] sets read-only permissions on all files in the WordPress install

#### 35. Which of the following must have underlined links in order to meet WCAG 2.0 accessibility standards?

1. [ ] links on images
2. [ ] links in user interface controls
3. [ ] links in a nav bar
4. [x] links in paragraph text

#### 36. Review the HTML on line 1. The goal of the PHP on line 2 is to extract the field value and assign it to a variable prior to inserting into the database. What is wrong with this PHP code?

```php
<input type="text" id="title" name="title" />
$title = $_POST[ 'title' ];
```

1. [ ] The code sample does not use the GET method. It should be wrapped in the get_post_field() function and look like this $title = get_post_field( $GET[ 'title' ] );
2. [x] The code sample does not sanitize the form data. It should use the sanitize_text_field() function and look like this: $title = sanitize_text_field( $_POST[ 'title' ] );
3. [ ] There is no error. The code follows WordPress best practices.
4. [ ] The code sample does not allow for translation. It should use a translation function and look like this: $title = __( $_POST[ 'title' ];

#### 37. Which of these CSS classs naming convention is correct according to WordPress CSS Coding Standards?

1. [x] .selector-name
2. [ ] .selector_name
3. [ ] .selectorName
4. [ ] div.selector_name

#### 38. What are transients?

1. [ ] short database queries
2. [x] a way to cache information
3. [ ] plugins used for quick debugging
4. [ ] post draft stored in the database

#### 39. When should you edit core WordPress files?

1. [ ] when there is no plugin available to make a customization you need
2. [ ] when you need to add a custom page template
3. [ ] when you need to add a custom script to the header or footer of every page in a site
4. [x] You should never edit WordPress core.

#### 40. Which Wordpress conditional would you use to determine if you were on a single page?

1. [ ] is_archive()
2. [ ] is_page()
3. [ ] is_page_template()
4. [x] is_single()

#### 41. Which of these are the minimum files required to make a child theme?

1. [ ] index.php functions.php
2. [ ] index.php style.css script.js
3. [ ] functions.php style.css script.js
4. [x] functions.php style.css

#### 42. In the WordPress template hierarchy, which file could not be used to display an archive?

1. [ ] archive.php
2. [x] index.php
3. [ ] page.php
4. [ ] category.php

#### 43. Why can't you modify the query in a template page?

1. [ ] The query can only be run inside the Loop.
2. [x] You can modify the query in a template page if you use pre_get_posts().
3. [ ] According to WordPress best practices, the query should only be modified in functions.php.
4. [ ] Due to execution order, the query has already run by the time a template is loaded.

#### 44. For the majority of modern themes, what is the standard method used to customize various details of site appearance and features, such as changing the site description or adding a logo and favicons?

1. [ ] WordPress settings
2. [x] Customizer
3. [ ] wp-config.php
4. [ ] Theme settings

#### 45. How would you write a text string containing "Hello World!" in a way that makes it possible for someone else to translate the string into a different language?

1. [ ] `apply_filters( 'Hello World!', 'mytextdomain' );`
2. [ ] `esc_html( 'Hello World!', 'mytextdomain' );`
3. [ ] `$string = "Hello World!";`
4. [x] `__( 'Hello World!', 'mytextdomain' );`

#### 46. You would use a post instead of a page when the content is _.

1. [ ] for a top-level menu item
2. [ ] nested (has a parent/child relationship with another piece of content)
3. [x] when the content is part of a blog.
4. [ ] evergreen

#### 47. Which of these does not impact your site speed?

1. [ ] caching
2. [ ] your web host
3. [x] inactive plugins
4. [ ] content delivery network (CDN)

#### 48. What can you not configure via wp-config.php?

1. [x] changing the default user role
2. [ ] changing the default wp_table prefix
3. [ ] changing your site or WordPress address
4. [ ] changing the default number of post revisions
