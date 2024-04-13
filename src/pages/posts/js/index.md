---
layout: "@layouts/Layoutmd.astro"
title: Learning Javascript
date: 21 Oct 2022
author: Demian Ruiz
desc: Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque reiciendis culpa nulla totam assumenda dolores eius aliquam quidem praesentium et libero ex error eaque tenetur, omnis beatae labore. Ipsum, nisi.
image: https://cdn.pixabay.com/photo/2015/04/23/17/41/javascript-736400_1280.png
---

# Learning Javascript

![html](https://cdn.pixabay.com/photo/2015/04/23/17/41/javascript-736400_1280.png)

Lorem ipsum dolor, sit amet consectetur adipisicing elit. Maiores, voluptate cupiditate eius iure nobis itaque modi sed necessitatibus ducimus officia consectetur numquam repudiandae, nihil esse saepe ullam ipsam quia quam.

Lorem ipsum dolor, sit amet consectetur adipisicing elit. Maiores, voluptate cupiditate eius iure nobis itaque modi sed necessitatibus ducimus officia consectetur numquam repudiandae, nihil esse saepe ullam ipsam quia quam.

Lorem ipsum dolor, sit amet consectetur adipisicing elit. Maiores, voluptate cupiditate eius iure nobis itaque modi sed necessitatibus ducimus officia consectetur numquam repudiandae, nihil esse saepe ullam ipsam quia quam.

Lorem ipsum dolor, sit amet consectetur adipisicing elit. Maiores, voluptate cupiditate eius iure nobis itaque modi sed necessitatibus ducimus officia consectetur numquam repudiandae, nihil esse saepe ullam ipsam quia quam.

Lorem ipsum dolor, sit amet consectetur adipisicing elit. Maiores, voluptate cupiditate eius iure nobis itaque modi sed necessitatibus ducimus officia consectetur numquam repudiandae, nihil esse saepe ullam ipsam quia quam.

Lorem ipsum dolor, sit amet consectetur adipisicing elit. Maiores, voluptate cupiditate eius iure nobis itaque modi sed necessitatibus ducimus officia consectetur numquam repudiandae, nihil esse saepe ullam ipsam quia quam.

```javascript
function getTags(tagsResponseJson){
	var tags = '';	
	if (tagsResponseJson != undefined){
		if (tagsResponseJson.Tags != undefined){
			if (tagsResponseJson.Tags.Tag != undefined){ 
				if (isArray(tagsResponseJson.Tags.Tag)){
					for (var i = 0;i<tagsResponseJson.Tags.Tag.length;i++){
						tags = tags + tagsResponseJson.Tags.Tag[i].TAG_TIPO + ",";
					}
					return tags;
				} else {
					return tagsResponseJson.Tags.Tag.TAG_TIPO + ",";
				}
			}	 	 
		}
	}
	return tags;
}
```