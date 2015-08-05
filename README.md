jquery-iLightbox 0.1
================

jQuery Lightbox is a simple port of the popular lightbox script.

__<a href=http://grandesign.md/__cr/plugins/jquery.iLightbox/" target="_blank">Demo Page</a>__

Usage
-------
__Styles:__

Include the jquery.lightbox css file in your html page.
~~~~ html
<link href="jquery.lightbox.css" type="text/css" rel="stylesheet" />
~~~~

__Javascript:__

Include the jQuery library and jquery.iLightbox script file in your html page.
~~~~ html
<script src="http://code.jquery.com/jquery-latest.min.js"></script>
<script src="jquery.lightbox.min.js"></script>
~~~~
Create link elements whose href attributes will contain the path of the element you wish to open within the iLightbox.
~~~~ html
<a href="http://www.lifelenta.ru/images/uploads/files/FE4kxj8ylCwmc.jpg" data-lightbox-gallery="gallery" data-lightbox-title="Image 1" class="lightbox">Image 1</a>
<a href="http://www.lifelenta.ru/images/uploads/cs41/Nt1cVeiuHds5I.jpg" data-lightbox-gallery="gallery" class="lightbox">Image 2</a>
~~~~
The plugin is named "iLightbox" and can be applied to any element. You will probably also specify some options while applying the plugin.
~~~~ javascript
$(document).ready(function() {
	$('a.lightbox').iLightbox({
		type: 'image', //'image', 'ajax', 'iframe', 'swf' and 'html'
		loop: true, //loop media
		arrows: true, //show arrows
		closeBtn: true, //show close button
		title: null, //title
		href: null, //link to media
		content: null, //html content
		beforeShow: function(a, b) {},
		onShow: function(a, b) {},
		beforeClose: function() {},
		afterClose: function() {},
		onUpdate: function(a) {},
		template: {
			container: '<div class="iLightbox-container"></div>',
			image: '<div class="iLightbox-media"></div>',
			iframe: '<div class="iLightbox-media iLightbox-iframe"></div>',
			title: '<div class="iLightbox-details"></div>',
			error: '<div class="iLightbox-error">The requested content cannot be loaded.<br/>Please try again later.</div>',
			closeBtn: '<a href="#" class="iLightbox-close"></a>',
			prevBtn: '<div class="iLightbox-btnPrev"><a href="javascript:;"></a></div>',
			nextBtn: '<div class="iLightbox-btnNext"><a href="javascript:;"></a></div>'
		}
	});
});
~~~~

Features
-------
__manual Options:__
* $.iLightbox.close()

__attribute Options:__
* data-lightbox-gallery | name of gallery
* data-lightbox-title | media title
* data-lightbox-title | type of media
* data-lightbox-content | media content

License
-------
> Licensed under <a href="http://opensource.org/licenses/MIT">MIT license</a>.
