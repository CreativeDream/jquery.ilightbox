jquery-iLightbox 0.1
================

jQuery Lightbox is a simple port of the popular lightbox script.

__<a href="http://creativedream.net/plugins/jquery.iLightbox/" target="_blank">Demo Page</a>__

Usage
-------
The function is called 'iLightbox'. So just call it ;)
~~~ javascript

$('a[data-lightbox-gallery]').iLightbox({
    type: 'image', //'image', 'ajax', 'iframe', 'swf' and 'html'
    loop: true,
    arrows: true,
    closeBtn: true,
    title: null,
    href: null,
    content: null,
    beforeShow: function(a, b){ },
    onShow: function(a, b){ },
    beforeClose: function(){ },
    afterClose: function(){ },
    onUpdate: function(a){ },
});
	
~~~~

License
-------
> Licensed under <a href="http://opensource.org/licenses/MIT">MIT license</a>.

