Twitter style buttons with CSS3 and Compass v0.9
===========

This cool recipe for SASS (Compass) lets you combine and create 
practically an infinite number of combinations that generate twitter style buttons.

Additionally you can also include an icon next to your text, keeking your code neat and clean.
This recipes use the Iconic typace by [**Some Random Dude**](http://somerandomdude.com/projects/iconic/).
No images are used at all in the making of this buttons.


Demo
====

![screenshot](http://eliseos.net/test/compass_css3_buttons/twitter_style_buttons.png)

Don't forget to check the [live demo](http://eliseos.net/test/compass_css3_buttons/)


Install
=======

Install the buttons module with:

    @import "fancy_3d_buttons";
    

Move the folder **fonts** to the root of your Rail project.

Configurable Variables
======================

	twitter_button(color-background, text-color, border-radius, font-size, icon-type)


Mixin
=====

                    a.default{
                    @include twitter_button();
                    }
                    /*/Default settings /*/
                    
                    
                    a.green{
                    @include twitter_button(#00AE3E, #fff, 5px,12px)
                    }
                    /*/ Custom background color, custom text color, custom border-radius, custom font size, no icon /*/
                    
                    
                    a.red{
                    @include twitter_button(#c63738,#fff, 0,0)
                    }
                    /*/ Custom background color, custom text color, default border-radius, default font size, no icon /*/
                    
                    
                    a.violet{
                    @include twitter_button(0,#000)
                    }
                    /*/ Default background color, custom text color,default border-radius, default font size, no icon  /*/
					
					
					a.icon_home{
                    @include twitter_button(#00A0B0, #fff, 5px,12px,'!')
                    }
                    /*/ Custom background color, custon text color, custom border-radius, custom font size, home icon /*/
                    
                    
                    a.icon_arrow-right 
					{@include twitter_button(0, 0, 5px,12px, "4") 
					}
					/*/ Default background color, default text color, custom border-radius, custom font size, right arrow icon  /*/
	

**For a full list of available icons please check the Demo**.


Changelog
=========
24/06/2011 - Fixed some bugs, add support to Opera gradients, Fixed the Typo weird bug in Safari
12/01/2011 - First release
12/01/2011 - Include the SASS files 


Todo
====

* Make a better :hover :visited state
* Find a solution  for IE9 Border-radius and Background Gradient Bleeding

Licence
=======

    Copyright (c) 2011 Alexis Sgavel (http://github.com/Baires)
    
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
    
    The above copyright notice and this permission notice shall be included in
    all copies or substantial portions of the Software.
    
    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
