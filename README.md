ElementSwap
===========

ElementSwap is a simple Slide Show class that will swap between any element.

![Screenshot](http://github.com/vincentbluff/ElementSwap/raw/master/screenshot.png)

Requirements
------------

* [MooTools Core 1.2.4](http://mootools.net/core): Class, Class.Extras, Element, Selectors (and their dependencies)

How to use
----------

### Syntax
	#JS
	var myElSwap = new ElementSwap(elements[, options]);

### Arguments

1. elements - (*mixed*) A collection of elements to add. Takes the same arguments as [$$]
2. options - (*object*, optional) An object with options. See below.

### Options
- selectedClass - (*string*: defaults to 'active') the css class for the slide when it is displayed.
- elementSwapDelay - (*integer*: defaults to 3) the number of seconds to wait to change to the next slide.
- panelWrap - (*string*: defaults to 'elementSwapWrap') the id of the slide wrap.
- panelWrapClass - (*string*: defaults to 'elementSwap') the css class for the slide wrap.
- events - (*boolean*: defaults to true) whether to setup the slide events. On mouse enter the slide show stops, on mouse leave the slide show starts, on mouse click fires the onClickView event.
- activateOnLoad - (*mixed*: defaults to 0) which slide to activate on loading the class, can be the id of an element or the index number of the slides array
- autoPlay - (*boolean*: defaults to false) whether to start looping though the slides on initialization.

### Events
- onActive - (*function*) callback executed when a slide is shown, passed two arguments: the index of the slide (*integer*), the slide (*element*)
- onClickView - (*function*)  callback executed when the user clicks on the current slide, passed two arguments: the index of the slide (*integer*), the slide (*element*)
- onNext - (*function*)  callback executed when the next method is executed.
- onPrevious - (*function*)  callback executed when the previous method is executed.

### Returns:

* (*object*) A new ElementSwap instance.

### Example:


[$$]: http://www.mootools.net/docs/core/Element/Element#dollars