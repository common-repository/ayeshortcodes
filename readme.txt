=== AyeShortcodes ===
Contributors: psdtohtmlguru
Tags: shortcode, Post, accordion, tabs, vertical tabs, columns, buttons, icons, pricing table, fancy buttons, clean buttons, progress bar, message box, alert box, dropcap, drop capital, blockquote, label, tooltip, lead paragraph, google, google shortcodes, google fonts, divider, custom headlines, back to top, go to top, before and after, counter, bootstrap, fontawesome, shortcodes, shortcode manager, customization, tools, responsive, performance, tabbed content
Requires at least: 3.0.1
Tested up to: 4.6
Stable tag: 0.1
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

== Description ==
Helpful shortcodes with clean design, also a companion plugin for all themes available at AyeLabs. Build with developers, performance and user experience in mind.

## Features:
* 20+ shortcodes
* Highly optimised, all assets are loaded only on the page shortcode is used
* Theme authors can take advantage of assets management to load assets directly in theme and exclude the assets from plugin
* Clean design
* Easily extendable & development support ( via support forums )
* Multilangual
* Works with any theme ( or plugin, if you wish so )
* 100% responsive
* Developed with love

## Supported Shortcodes:
**[column]** - Add a column using Bootstrap style. Supports the following attributes:
* lg - Large display size
* md - Medium display size      
* sm - Small display size      
* xs - Extra-Small display size       
* pull_lg - Pull for large display size 
* pull_md - Pull for medium display size   
* pull_sm - Pull for small display size   
* pull_xs - Pull for extra small display size   
* push_lg - Push for large display size   
* push_md - Push for medium display size    
* push_sm - Push for small display size     
* push_xs - Push for extra small display size     
* offset_lg - Offset for large display size   
* offset_md - Offset for medium display size   
* offset_sm - Offset for small display size
* offset_xs - Offset for extra small display size
* pricing_table - Use this attribute to define a pricing table column, give it a name as value
* pricing_highlighted - If this is the highlighted column from your table, add this empty attribute

** Wrap the content inside of this shortcode **

**[aye_tabs]** - Creates tabbed content. Use it to wrap tabs created with [aye_tab]. Supports the following attributes:
* orientation - Choose the orientation of the tabs, possible options: "horizontal" and "vertical". Default is "horizontal"

** Wrap the content and [aye_tab] shortcodes inside of this shortcode **

**[aye_tab]** - Creates a tab content in [aye_tabs] shortcode. Supports the following attributes: 
* title - Tab title

** Wrap the content inside of this shortcode **

Example:

	[aye_tabs]
		[aye_tab title="About You"]Describe yourself[/aye_tab]
		[aye_tab title="Your Requirements"]What are your requirements?[/aye_tab]
	[/aye_tabs]

**[aye_button]** - Adds a custom button. Supports the following attributes:
* url - URL the button should link to
* label - Button label
* target - Where to open the button URL. Basic target attribute values http://www.w3schools.com/TAGS/att_a_target.asp. Default value is empty, but if you add an external URL the _blank target will be added automatically.
* id - Give an unique ID to the button
* postid - Link a post to the button ( 'url' attribute will be overwritten )
* icon - Font Awesome icon id ( without fa- prefix )

**[aye_cta]** - Creates an Call to Action section. Use [aye_button] to add a button inside of the CTA section. Supports the following attributes:
* position - Content position. Supports: "left", "right", "center". Default is "left"
* background - Background color. Default is "#007acc".
* color - Color for: button border, text and button label. Default is "#fff".

** Wrap the content inside of this shortcode **

Example:

	[aye_cta background="tomato"]
		We have the best tomatoes!
		[aye_button id="1" icon="shopping-cart" label="Buy now!"]
	[/aye_cta]

**[aye_pricing_title]** - Add a header title inside of your pricing table column. Use this shortcode inside [aye_column]. Supports the following attributes:
* title - Pricing table title ( ex. package name )
* price - The price displayed on your table without currency

**[aye_pricing_row]** - Add a feature row inside of your pricing table column. Use this shortcode inside [aye_column]. Supports the following attributes:
* content - A feature that table offers
* icon - Font Awesome icon id ( without fa- prefix )

Pricing table example with two packages:

	[aye_column md="6" pricing_table="demo" pricing_highlighted="true"]
		[aye_pricing_title title="Pack 1" price="$30"]
		[aye_pricing_row content="Awesome feature"]
		[aye_pricing_row icon="github" content="Github Compatible"]
	[/aye_column]
	[aye_column md="6" pricing_table="demo"]
		[aye_pricing_title title="Pack 2" price="$50"]
		[aye_pricing_row content="Awesome plugin"]
		[aye_pricing_row icon="gitlab" content="Gitlab Compatible"]
		[aye_button url=""  label="Icon Button" icon="gitlab"]
	[/aye_column]
*Add the shortcodes without spacing between them to avoid p tag wrapping.

**[aye_progress_bar]** - Create a simple progress bar. Supports the following attributes:
* percent - Percent the bar should load. From 0 to 100
* label - Text label that will be displayed insinde of the loading bar
* icon - Font Awesome icon id. The icon will be displayed before label, insinde of the loading bar

**[aye_message_box]** - Create a message/alert box, personalized or using predefined styles. Supports the following attributes:
* type - Predefined type of the box: error, warning, info, success. Don't use this attribute if personalized box is created.
* text - Text the box will display

Customization attributes:
* icon -  Add a icon at the begining of the box.
* color - Text color
* background - Background color

**[aye_icon]** - Add an simple inline icon. Supports the following attributes:
* icon - The Font awesome icon id, without -fa prefix.

**[aye_drop_capital]** - Creates a drop capital letter. Supports the following attributes:
* letter - The letter
* color - The letter color
* font - The font-family style

**[aye_blockquote]** - Creates a blockquote. Supports the following attributes:
* position - Choose between 'left' or 'right'. Default is 'left'.
* columns - Choose the bootstrap columns classes. Default is 'col-md-4' ( width of four columns )
* author - The quote author

** Wrap the content inside of this shortcode **

**[aye_label]** - Creates a minimal text label. Supports the following attributes:
* icon - Add an icon on your label
* background - Background color
* text - Label text
* arrow - Your label can have a small arrow on the sides, pointing at something. Choose the arrow direction from: left, right, bottom and top
* color - Text color

**[aye_accordion]** - Creates an accordion slider. Supports the following attributes:
* title - Title of the box
* active - Add this attribute without a value to open the box by default

** Wrap the content inside of this shortcode **

**[aye_divider_gotop]** - Creates an simple border divider with Back to top link. Supports the following attributes:
* border_color - The divider border color
* border_height - The divider border height
* color - 'Back to top' text color
* margin - The top and bottom margins

**[aye_divider_headline]** - Creates a styled divider headline. Supports the following attributes:
* border_color - The two borders color
* color - Text color
* background_color - Divider background color

** Wrap the content inside of this shortcode **

**[aye_lead_paragraph]** - Transform your paragraph into a lead paragraph [wikipedia](https://en.wikipedia.org/wiki/Lead_paragraph) . Doesn't support any attributes. 

** Wrap the content inside of this shortcode **

**[aye_tooltip]** - Adds an simple tooltip to your content. Supports the following attributes:
* text - Tooltip text

** Wrap the content inside of this shortcode **

**[aye_google_font]** - Wrap your content with a Google Font. Don't worry, the font will be loaded only on the pages this shortcode is used. Supports the following attributes:
* font - Google Font name ( valid example: 'Open Sans' invalid example: 'Open+Sans' )
* weight - The font weight, ex: 400. For italic style add your desired font weight followed by 'i', example for normal italic: 400i

** Wrap the content inside of this shortcode **

**[aye_before_after]** - Creates an before and after image slider. Supports the following attributes:
* before - Before image URL
* after - After image URL

**[aye_counter]** - Creates a number counter. The counter starts when your page loads. Supports the following attributes:
* from - The number to start counting from
* to - The number to stop counting at
* speed - The number of milliseconds it should take to finish counting
* refresh - The number of milliseconds to wait between refreshing the counter

== Installation ==
### Manual Installation
1. Unzip 'AyeShortcodes' inside of '/wp-content/plugins/' directory
2. Activate the plugin through the 'Plugins' menu in WordPress

### Recommended Installation
1. Seach 'AyeShortcodes' in Plugins > Add new
2. Click 'Install Now' and Activate the plugin

Updates will be provided through the WordPress updater.

== Frequently Asked Questions ==

### What is a shortcode?
A shortcode is a WordPress-specific code that lets you do nifty things with very little effort. Shortcodes can embed files or create objects that would normally require lots of complicated, ugly code in just one line. [source](https://en.support.wordpress.com/shortcodes/)

### How do i use a shortcode?
Simply add the shortcode id between squere brakets and place it in your post content. [shortcode_id]. If the shortcode supports attributes add them using the following sintax [shortcode_id attribute="attribute with value" attribute_without_value]. If your shortcode needs to alter your content, simply wrap the content with the shortcode. [shortcode_id]Your content[/shortcode_id]

### How can i integrate AyeShortcodes with your theme?

AyeShortcodes it's a plugin developed with flexibility in mind. Besides the basic shortcode manager, it comes with a small assets dependecy manager that will allow you, as a developer, to manage the assets loaded on the website ( both from plugin and theme ). This will optimize the page and avoid loading it with unused/duplicate assets. The following code will help you setup your theme to be compatible with this plugin, follow the code comments

	// Check if AyeShortcodes plugin exists
	if(class_exists('\Aye\Shortcodes\Core')) {
		
		// Tell AyeShortcode plugin that you use the theme mode
		add_filter('aye_shortcodes_theme_mode', '__return_true');
		
		// Access core class, if you don't need it you can delete it
		global $aye_shortcodes;
		
		// Let the plugin know all the shortcodes your theme is compatible with
		add_filter('aye_shortcodes_available_filter', function($array) {
			return array('column', 'label');
		});
		
		// Exclude assets from plugin if they are already bundled in the theme ( ex. Exclude 'bootstrap-columns' beacause you theme already use bootstrap ).
		add_filter('aye_shortcodes_style_assets', function($array) {
			return array('bootstrap-columns');
		});
		
	}

See the markup generated by each shortcode on /assets/dev/markup.html.

== Changelog ==
= v0.1 =
* Initial release