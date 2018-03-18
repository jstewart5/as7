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
  - [X] Steps to recreate:
    - Make a post with this code: <code> XXS Attack[caption width="1" caption='<a href="' ">]</a><a href="http://onMouseOver='alert(1)'">CLICK THIS</a></code>
  - [X] Affected source code:
    - [Link 1](https://github.com/WordPress/WordPress/commit/f72b21af23da6b6d54208e5c1d65ececdaa109c8)
2. WordPress 4.1-4.2.1 - Unauthenticated Genericons Cross-Site Scripting
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version:
    - Fixed in version: 
  - [X] GIF Walkthrough: 
  - [X] Steps to recreate: 
  - [X] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
3. (Required) Vulnerability Name or ID
  - [X] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [X] GIF Walkthrough: 
  - [X] Steps to recreate: 
  - [X] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
