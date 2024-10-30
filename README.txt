===  Mimo Maps ===
Contributors: mimothemes
Donate link: http://mimo.media/
Tags: maps, locations,google map,google maps,easy google maps,google maps locations, google map for posts, google map shortcode, map shortcode,address, cross-browser, custom google map, custom google maps, easy map, geo, geocoder, gmaps, google, google earth, google map, google map plugin, google maps plugin, googlemaps, map markers, map plugin, map styles, map widget, maps, marker, openstreetmap, place, polygons, polylines, post map, routes, streetview, widget map, wp google map, wp google maps, wp map, wp maps, wordpress google maps, wordpress google map, api, directions, driving,map custom color,custom markers colors, custom icons, custom map colors, custom icon colors, custom map markaers colors, custom markers, google map custom markers, custom google routes
Requires at least: 4.3
Tested up to: 4.5.2
Stable tag: 3.2
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Integrate Google Maps easily in your site, no coding required! Show multiple Google Maps.

== Description ==

Google Maps easy in your site. This plugin gives a you a shortcode to show your color customized Google Map with no coding knowledge.. Just set your post locations, map colors, height and zoom and show your customized maps easily in your pages and posts, show different Google Maps per Category.





With this Google Maps Plugin you can:
<ul>
	<li>Create, edit and delete your custom locations for your posts</li>
	<li>Easy to use, no coding required</li>
	<li>100% Responsive Maps</li>
	<li>Google Maps Streetview supported</li>
	<li>UTF-8 character support</li>
	<li>Choose Zoom and Height of your map</li>
	<li>Customize markers colors and icons for each posts category</li>
	<li>Create Routes</li>
	<li>Customize map colors easily</li>
</ul>




== Installation ==



= Using The WordPress Dashboard =

1. Navigate to the 'Add New' in the plugins dashboard
2. Search for 'mimo-maps'
3. Click 'Install Now'
4. Activate the plugin on the Plugin dashboard

= Uploading in WordPress Dashboard =

1. Navigate to the 'Add New' in the plugins dashboard
2. Navigate to the 'Upload' area
3. Select `mimo-maps.zip` from your computer
4. Click 'Install Now'
5. Activate the plugin in the Plugin dashboard

= Using FTP =

1. Download `mimo-maps.zip`
2. Extract the `mimo-maps` directory to your computer
3. Upload the `mimo-maps` directory to the `/wp-content/plugins/` directory
4. Activate the plugin in the Plugin dashboard


== Frequently Asked Questions ==

None by the moment.

== Screenshots ==


== Upgrade Notice == 

No upgrades yet

== Changelog ==


= 1.0 =

First Version


= 2.0 =

Changed coordinates field to manual


= 3.0 =

Added map icon font
Added error message when no locations found in posts
Deleted Locations post type


== Usage instructions ==

Set category icons and colors in plugin Settings, Goto Settings/Mimo Maps</br>

Use [mimo-maps] shortcode to show the map with all locations(all posts or products locations), using shortcode:

[mimo-maps post_id="id of location" ] Shows only one location

[mimo-maps category_slug="slug" ] Shows locations from one category

[mimo-maps category_slug="slug" posts_per_page="2" ]



Shortcode atributtes:



<ul>
	<li><strong>post_id</strong> = Id of post to show(only one post), default empty</li>
	<li><strong>category_slug</strong> = slug of category to show, default empty</li>
	<li><strong>posts_per_page</strong> = Number of posts to show(only posts with locations), default -1</li>
</ul>



== Developer instructions ==



You can pass your options to the opstions array:

<code>

$args = array(
'post_id' => '',
'category_slug' => '',
'posts_per_page' => '',

);


if (  class_exists('Mimo_Maps_Display')  ) Mimo_Maps_Display::display_map( $args );</br>

</code>


Find plugin and issues solved at http://mimo.studio