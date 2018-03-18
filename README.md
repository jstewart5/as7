# as7
# Project 7 - WordPress Pentesting

Time spent: **4** hours spent in total

> Objective: Find, analyze, recreate, and document three vulnerabilities affecting an old version of WordPress

## Pentesting Report

1. WordPress <= 4.3 - Authenticated Shortcode Tags Cross-Site Scripting 
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.1.1
    - Fixed in version: 4.3.1
  - [X] GIF Walkthrough: https://puu.sh/zK4da/f02dedf433.gif
  - [X] Steps to recreate: Make a post with this code: ``` XSS Attack[caption width="1" caption='<a href="' ">]</a><a href="http://onMouseOver='alert(1)'">CLICK THIS</a> ``` and click the hyperlink while viewing the post.
  - [X] Affected source code: 
    - [Link 1](https://github.com/WordPress/WordPress/commit/f72b21af23da6b6d54208e5c1d65ececdaa109c8)
2. WordPress 3.7-4.4 - Authenticated Cross-Site Scripting
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2.2
    - Fixed in version: 4.2.5
  - [X] GIF Walkthrough: https://puu.sh/zK5Yt/c72f443e13.gif
  - [X] Steps to recreate: As an admin, append ``` <svg onload=alert(1)> ``` to the end of a url when adding text to a new post.
  - [X] Affected source code:
    - [Link 1](https://github.com/WordPress/WordPress/commit/7ab65139c6838910426567849c7abed723932b87)
3. (Required) Vulnerability Name or ID
  - [X] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [X] GIF Walkthrough: 
  - [X] Steps to recreate: 
  - [X] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
