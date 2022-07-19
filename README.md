# Learning WordPress

Basic list of things to learn when getting into WordPress. 

## Theme basics. 

- [ ] Create a theme, no functionality but you can activate it in the WP admin. Create a few posts to use as test data.
- [ ] Create a basic theme stylesheet and make sure it is loaded by your theme by enqueuing it in the functions.php file. Remember you're not learning front end here so don't spend a long time making it look nice! But you could include a CSS framework or something so that you're working with something that looks decent.
- [ ] Basic template files.
	- [ ] index.php - don't worry about outputting anything just yet.
	- [ ] Header - display site title.
	- [ ] Footer - Display something basic here - e.g. copyright notice
- [ ] The Loop.
	- [ ] Display a list of the latest posts on the homepage of your site by adding "the loop' to the index.php template file. Output the title, post date and excerpt. The post title should link to the single post page.
- [ ] Single post template. Display title, date, author, and full content.
- [ ] Learn about [Template Hierarchy](https://codex.wordpress.org/Template_Hierarchy). Experiment with a different view for category and tag archives from the home page. Create a slightly different design for pages compared to posts. How are date archives shown or author archives. Have a play around and see all the different ways WordPress can display content.
- [ ] Add a header image from your theme file to the header template of your site. Including the full img tag in your code, not just using CSS. Use the size 'full'. 
- [ ] Add a theme JavaScript file
	- [ ] That file should include jQuery as a dependency. 
	- [ ] That file should be loaded in the footer. 
	- [ ] Just console.log something to verify it is loaded, we're not learning JS here. 

## Plugin Basics

- [ ] [Create a plugin that you can activate from the plugins admin page.](https://developer.wordpress.org/plugins/plugin-basics/)
- [ ] Understand the difference between Plugins and MU Plugins. 
- [ ] Actions and filters. 
    - [ ] https://codex.wordpress.org/Plugin_API/Action_Reference
    - [ ] Use a filter to modify the post content and insert some text at the end of each post. 
    - [ ] Use an action to output some HTML in the head section of the page.  
- [ ] Conditional tags. e.g. is_home 
    - [ ] Update the filter above to use conditional tags to only modify the content for posts of type 'post' when on the single post page. 

## Block Editor Basics

- [ ] [Learn about using the block editor to create media rich posts and pages.](https://wordpress.org/support/article/wordpress-editor/). You should cover the following:
    - [ ] Common blocks and media blocks. Including changing the block settings and styles.  
    - [ ] Layout blocks e.g. column blocks
    - [ ] Using block patterns
    - [ ] Reusable blocks
- [ ] [Using Theme.json to configure the editor](https://developer.wordpress.org/block-editor/reference-guides/theme-json-reference/)

## Theme Intermediate

- [ ] Register a custom post type.
- [ ] Register a custom taxonomy for that post type.
- [ ] Create a custom template for the new custom post type. 
- [ ] Register a nav menu and display it in your site header template.
- [ ] Display a post thumbnail on the homepage at size 'thumbnail' and on the single post page using the 'large' size. This should be conditional on the post having a thumbnail set. 
- [ ] Register a custom image size of 400x225 and use that on the homepage. 
- [ ] Custom WP Query.
    - [ ] Explore the documentation. Understand using different arguments to retrieve different content. 
    - [ ] In the footer of your site, output 5 posts from a single author. Output the title and a link to that post.
    - [ ] Update the above query to include only posts in the category 'news' and with the tag 'breaking'.
    - [ ] Pagination.
- [ ] Add comments to template for single posts. Just copy/paste at this point is fine, don't dive in too deeply but try to get an understanding of the functionality and what is possible. 
- [ ] Child themes. Create another new theme, that is a child theme of this one and use it to modify some behaviour.


## Plugins Intermediate

- [ ] Admin menu pages. 
- [ ] [Settings API.](https://developer.wordpress.org/plugins/settings/settings-api/)
- [ ] [Writing a custom WP CLI command](https://make.wordpress.org/cli/handbook/guides/commands-cookbook/)

## Block editor Intermediate

- [ ] Create a custom block following [the tutorial on WordPress Developer Handbook](https://developer.wordpress.org/block-editor/getting-started/create-block/). You should cover the following: 
    - [ ] Registering a block
    - [ ] `block.json`
    - [ ] Block Stylesheets (and editor styles)
    - [ ] Block attributes, using TextControl to edit them.
- [ ] Custom block stretch goals
    - [ ] Use pre-built components to create a better User interface for managing your block attributes. 
        - [ ] Different input types e.g. Date picker
        - [ ] Sidebar/InspectorControls
	- [ ] Rich Text
- [ ] [Create a block editor plugin with a sidebar.](https://developer.wordpress.org/block-editor/how-to-guides/plugin-sidebar-0/) 
- [ ] [Use API Fetch to retrieve data from the WP REST API.](https://developer.wordpress.org/block-editor/reference-guides/packages/packages-api-fetch/)

## Theme advanced. 

- [ ] Use [HM Webpack Helpers](https://humanmade.github.io/webpack-helpers/) to build a JavaScript file in your theme so that you can write modern JS and JSX. Just production mode is fine to start. 
- [ ] Use HM Webpack Helpers to compile a SCSS file. 
- [ ] Use [Asset Loader](https://github.com/humanmade/asset-loader) to load your files. 
- [ ] Set up webpack dev server so that it 
- [ ] Elasticsearch/Elasticpress
    - [ ] Have an understanding of this integration. How it works. Why it is necessary. 
    - [ ] Running elasticpress sync CLI command.
    - [ ] Know when a WP_Query is offloaded to Elasticsearch. 
    - [ ] Add custom data to Elasticsearch
    - [ ] Doing custom queries. 

## Block Editor Advanced

- [ ] Hooks/Filters & Slot Fills to modify editor functionality.
- [ ] Using the wp data store
    - [ ] [Get current value of post meta.](https://developer.wordpress.org/block-editor/reference-guides/data/data-core-editor/#geteditedpostattribute)
    - [ ] Update the value of post meta. 
    - [ ] [Fetch a post.](https://developer.wordpress.org/block-editor/reference-guides/data/data-core/)
    - [ ] [Register a custom data store.](https://developer.wordpress.org/block-editor/reference-guides/packages/packages-data/#registering-a-store)

## Front end concepts that are important for theme development at HM. 

- [ ] SCSS
	- [ ] Variables
	- [ ] Partials
	- [ ] Mixins
	- [ ] Functions
	- [ ] Nesting
- [ ] [BEM css naming convention](http://getbem.com/naming/). 
	- [ ] Why is this useful?
