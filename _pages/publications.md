---
layout: page
permalink: /publications/
title: publications
description: 
nav: true
nav_order: 1
---


<html>

<head>
    <!-- Include Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <title>Posts</title>
        <style>
        /* CSS for the navigation bar */
        .navbar {
            background-color: #333;
            overflow: hidden;
        }
        .navbar ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        .navbar li {
            display: inline;
            margin: 10px;
        }
        .navbar a {
            color: white;
            text-decoration: none;
        }
        .section-divider {
            border: 5px solid #FFF; /* Add a border */
            margin: 40px 0; /* Adjust spacing as needed */
        }
        body {
            padding-bottom: 70px;
            color: var(--global-text-color);
            background-color: var(--global-bg-color);
            h1, h2, h3, h4, h5, h6 {
                scroll-margin-top: 66px;
            }
        }
    </style>


</head>

<body>
<!-- _pages/publications.md -->
<div class="publications">

{% bibliography -f {{ site.scholar.bibliography }} %}

</div>

</body>
</html>