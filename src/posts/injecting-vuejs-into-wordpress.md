---
title: Injecting VueJS into Wordpress
description: Here's the Quick Scoop on using VueJS in a Wordpress Template
author: J-Dog
date: 2021-12-03T17:06:09.075Z
tags:
  - Tags
---
Here are some quick snap shots of codes that you would need to insert into a Wordpress template.

The process is pretty straight forward after you've done this a few times.

First off you need to insert the script into the **Functions.php**.

![vue in functionphp](/src/static/img/vue-inject.png "VueJS in Functions.php")

Next create a custom php file, in this case its called "**any-name-u-want.php**" (you can name it any way you like). Follow the Wordpress guidelines on this.

![custom php](/static/img/topcustomphp.png "Custom PHP")

Underneath the get_header(); ?> is where you put the Vue codes say for this typical search of images. This is just searching a short dedicated list not from a remote api.  Keeping this simple. Above the html is the style which I left out then follows what you see next. (below)

![VueJS HTML](/src/static/img/vue-search.png "VueJS HTML")

Here's the script for VueJS.

![VueJS Script](/static/img/vue-static-list.png "VueJS Script")

Next create another custom php file, very similar to the previous. However, this one is like another homepage or maybe a custom category page.  This is like a component, in Wordpress php they call it "get_template_part('vue1.php)".

![Get VueJS Component](/static/img/insert-vue.png "Get VueJS Component")

To get this to display in Wordpress, you would go to the page editor in the wp-admin. (after logging in) On the right side under "page" section choose the newly template.

![Choose Template in WP](/static/img/choose-template.png "Choose Template in WP")

Here's what it would look like from the frontend.

![vuejs search example](/static/img/vuejs-search.gif "Vuejs Search example")

Obviously, this scenario works on the type of project and the complexity.  This is a quick example to sprinkle in VueJS without having to do a separate whole build if you were working on a Reacts app.
