---
title: Security and Privacy Wizard
layout: 'index'
pages: 'pages/en'
start_url: '/en/'
lang_label: 'English'
desc: 'This guide will help you make Samsung Internet be as secure as possible and explain how it protects you.'
---
{
"dir": "ltr",
"lang": "en",
"name": "{{page.title}}",
"short_name": "{{page.title}}",
"scope": "{{ page.start_url  | relative_url }}",
"display": "standalone",
"start_url": "{{ page.start_url | relative_url }}",
"url": "{{ page.start_url | relative_url }}",
"background_color": "rgb(242, 242, 242)",
"theme_color": "rgb(242, 242, 242)",
"description": "{{page.desc}}",
"orientation": "any",
"related_applications": [],
"prefer_related_applications": false,
"icons": [
	{
		"src": "{{ "/assets/icons/images/android-launchericon-512-512.png" | relative_url }}",
		"sizes": "512x512"
	},
	{
		"src": "{{ "/assets/icons/images/maskable_icon.png" | relative_url }}",
		"sizes": "682x682",
		"type": "image/png",
		"purpose": "maskable"
	},
	{
		"src": "{{ "/assets/icons/images/android-launchericon-192-192.png" | relative_url }}",
		"sizes": "192x192"
	},
	{
		"src": "{{ "/assets/icons/images/android-launchericon-144-144.png" | relative_url }}",
		"sizes": "144x144"
	},
	{
		"src": "{{ "/assets/icons/images/android-launchericon-96-96.png" | relative_url }}",
		"sizes": "96x96"
	},
	{
		"src": "{{ "/assets/icons/images/android-launchericon-72-72.png" | relative_url }}",
		"sizes": "72x72"
	},
	{
		"src": "{{ "/assets/icons/images/android-launchericon-48-48.png" | relative_url }}",
		"sizes": "48x48"
	}
]
}