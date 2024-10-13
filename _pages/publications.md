---
layout: page
permalink: /publications/
title: publications
description: my publications
nav: true
nav_order: 1
---


<html>

<head>
    <title>Posts</title>
</head>

<body>
<!-- _pages/publications.md -->
<div class="publications">

    {% bibliography -f {{ site.scholar.bibliography }} %}

</div>

</body>
</html>