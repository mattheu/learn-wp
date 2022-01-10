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

## Theme intermediate

- [ ] Register a custom post type.
- [ ] Register a custom taxonomy for that post type.
- [ ] Create a custom template for the new custom post type. 
- [ ] Register a nav menu and display it in your site header template.
- [ ] Display a post thumbnail on the homepage at size 'thumbnail' and on the single post page using the 'large' size. This should be conditional on the post having a thumbnail set. 
- [ ] Register a custom image size of 400x225 and use that on the homepage. 

## The intermediate stretch goals. 

- [ ] Add comments to template for single posts. Just copy/paste at this point is fine, don't dive too deeply. 
- [ ] Create another new theme, that is a child theme of this one. 

## Theme advanced. 

- [ ] Use [HM Webpack Helpers](https://humanmade.github.io/webpack-helpers/) to build a JavaScript file in your theme so that you can write modern JS and JSX. Just production mode is fine to start. 
- [ ] Repeat for a SCSS file. 
- [ ] Use [Asset Loader](https://github.com/humanmade/asset-loader) to load your files. 
- [ ] Set up webpack dev server so that it 

## Front end concepts that are important for theme development at HM. 

- [ ] SCSS
	- [ ] Variables
	- [ ] Partials
	- [ ] Mixins
	- [ ] Functions
	- [ ] Nesting
- [ ] [BEM css naming convention](http://getbem.com/naming/). 
	- [ ] Why is this useful?
