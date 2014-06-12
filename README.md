tabStop
=======

In the need to mess with the focus of elements this plugin gives you the next or previous 'focusable' element according to the [HTML5 Standard Draft] [1].

Call `$.tabStop( direction, focusables )` where `direction` may be a negative value to receive the previous element, else the next element is given, and `focusables` is an optional string, by default ´focusables = 'a[href],link[href],button,input:not([type="hidden"]),select,textarea,menuitem,[draggable="true"]'´.
If the jQuery object on which this method is called is empty the next (or previous) element after the active element is returned.
If the first element of the jQuery object is not focusable itself the first focusable element in the document is returned.
The order of elements is handled as circle, as next element after the last focusable element you will receive the first and the other way around.

[1]: http://www.w3.org/html/wg/drafts/html/master/editing.html#focus "HTML5 Standard Draft"
