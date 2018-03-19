# as7
# Project 7 - WordPress Pentesting

Time spent: **4** hours spent in total

> Objective: Find, analyze, recreate, and document three vulnerabilities affecting an old version of WordPress

## Pentesting Report

1. WordPress <= 4.3 - Authenticated Shortcode Tags Cross-Site Scripting (XSS)
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.1.1
    - Fixed in version: 4.3.1
  - [X] GIF Walkthrough: ![Alt Text](https://puu.sh/zK4da/f02dedf433.gif)
  - [X] Steps to recreate: Embed the following code into a post: ``` XSS Attack[caption width="1" caption='<a href="' ">]</a><a href="http://onMouseOver='alert(1)'">CLICK THIS</a> ``` and click the hyperlink while viewing the post.
  - [X] Affected source code: 
    - [Link 1](https://github.com/WordPress/WordPress/commit/f72b21af23da6b6d54208e5c1d65ececdaa109c8)
2. WordPress 3.7-4.4 - Authenticated Cross-Site Scripting (XSS)
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2.2
    - Fixed in version: 4.2.5
  - [X] GIF Walkthrough: ![Alt Text](https://puu.sh/zK5Yt/c72f443e13.gif)
  - [X] Steps to recreate: As an admin, append ``` <svg onload=alert(1)> ``` to the end of a url when adding text to a new post.
  - [X] Affected source code:
    - [Link 1](https://github.com/WordPress/WordPress/commit/7ab65139c6838910426567849c7abed723932b87)
3. 3.6.0-4.7.2 - Authenticated Cross-Site Scripting (XSS) via Media File Metadata
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2.2
    - Fixed in version: 4.7.3
  - [X] GIF Walkthrough: ![Alt Text](https://puu.sh/zKDpz/5f87f9b7b8.gif)
  - [X] Steps to recreate: After uploading the [laced media file](https://www.securify.nl/advisory/SFY20160742/xss.mp3), insert it as a playlist into a post.
  - [X] Affected source code:
    - [Link 1](https://github.com/WordPress/WordPress/commit/28f838ca3ee205b6f39cd2bf23eb4e5f52796bd7)

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

This is a big leap from last week's assignment. Found it challenging to make this report ontop of understanding how to work the VM and Wordpress site. This was less of a learning experience and more of a hassle.

## License

    Copyright [2018] [Jesse Stewart]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
