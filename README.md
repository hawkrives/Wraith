# Wraith
Wraith is a fork of [Ghost](http://tryghost.org) that adds multi-user, multi-site support and configurable static file generation. Or, at least, it aims to. ;-)


## A History, of sorts
First, there were hyperlinked documents, edited by hand. Then there were tools to create them, and after them other tools to dynamically generate them on demand. These tools were used to build chronological records, and next thing we know Wordpress was the de facto winner for self-hosted blogging.

Then came the backlash. "Why," asked the Heathen, "should we spin CPU cycles and query databases and connect over network ports—even if on the same machine—to regenerate the same exact page, repeatedly?" And so [baking](http://inessential.com/2011/03/16/a_plea_for_baked_weblogs) entered our parlance, and it was good.

Except it wasn't. The Bakers (née Heathen) had thrown out much that was good, and looked upon the forcible regeneration of entire sites due to an inability to reliably tell what had changed as a *virtue*.


## More Seriously...
Static and dynamic generation of page content are simply *choices*, each valid for different use cases, satisfying different constraints. A large institutional site with dozens of editors frequently adding and updating pages benefits from dynamic generation and a live cache. A personal home page or blog, updated once or twice a week, is probably better rendered as static files with dynamic elements bound in-browser using JavaScript. And then there are cases in the middle, where individual article pages may be statically generated because they change infrequently, but new articles are added constantly and so the index page should be dynamic.

The "baked blogs" community seems to have overreacted to the complexity of the "blog engine" software, viewing the representation of entire blogs/sites purely as flat text files as an intrinsic virtue. Unfortunately, it doesn't scale *at all*, not even to small sites with two or three authors that would otherwise benefit from static generation.

I was looking to set up a personal blog and a blog for my nascent business. I didn't want to have to install separate blog engines or fiddle with rewrite regexes, and I wasn't enthused about any of the existing blog engines, anyway, as they all seemed to cater to needs far more complex than my own. So when I learned about _Ghost_, it sounded like the perfect base for my experiments.

Let's begin.
