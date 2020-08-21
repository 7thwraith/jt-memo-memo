---
layout: post
title: Attempts on Dissecting a Booru-style Image Board
date: 2013-04-09 18:50:03.000000000 -04:00
tags: projects
meta-tags:
permalink: "/2013/04/09/attempts-on-dissecting-a-booru-style-image-board/"
excerpt: "\n\t\t\t\t\t\t"
thumbnail: sample-e6fcd45065055b18015e92a23f475599-e1365551262472.jpg
thumbnail-caption: "Illustration by きのこ (dead link)"
thumbnail-caption-link: "https://www.pixiv.net/en/artworks/20092435"
---
[//]: # ([caption id="attachment_60" align="aligncenter" width="640"][![Art by 廿楽きのこ]({{ site.baseurl }}/assets/sample-e6fcd45065055b18015e92a23f475599-e1365551262472.jpg)](http://blog.7thwraith.net/wp-content/uploads/2013/04/sample-e6fcd45065055b18015e92a23f475599-e1365551262472.jpg) Art by 廿楽きのこ[/caption])

The concept of a booru-style image board has always fascinated me. What would normally be just a regular image gallery is now suddenly one of the hubs for anime/manga-esque images (high-quality resolutions at that too) as well as what seems to me as an instigator to a whole new subculture formed by the marriage of animango and the internets (more specifically, the web's underlying technologies).

I can talk to you all day about how uber-awesome boorus are, but what exactly makes a booru-style distinctive from all the image galleries/boards available across the web?

Wikipedia has the following to say

> ...Danbooru and derivatives aim for a non-hierarchical semantic structure in which users are able to post content and add tags, annotations, translations, and comment.

Seems legitimate. It's a comprehensive summary of how it functions but....not really helpful if you're trying to build a booru-style image board from scratch. If anything, I would probably start by enumerating the important (at least the ones that I deem importabt)  microfunctions of the site.

Let's start with the original booru-style image board, Danbooru.

Note that this list is not complete. Some features are omitted, others have yet to be identified. I will be adding to this list over time.

[//]: # ([![danbooru_search_results]({{ site.baseurl }}/assets/danbooru_search_results-1024x622.png "Danbooru's Search Result Page")](http://blog.7thwraith.net/wp-content/uploads/2013/04/danbooru_search_results.png))

1.  Search Bar - can search all classications of tags
2.  Tag list - list of all tags associated to images that are currently visible
3.  Tag classications - tags of a certain classication are of one color
4.  Tag-specific links - links to wiki pages that explain what the tag is used for
5.  Thumbnails - resized/cropped/edited versions of the full image
6.  Grid format - a grid of thumbnails
7.  Pagination

[//]: # ([![danbooru_single_post]({{ site.baseurl }}/assets/danbooru_single_post-1024x622.png "A single danbooru post")](http://blog.7thwraith.net/wp-content/uploads/2013/04/danbooru_single_post.png))

1.  Search bar block
2.  Copyright tag block - block which holds one type of tag classification
3.  Characters tag block - block which holds another kind  of tag classification, self explanatory
4.  Artist tag blog - similar to above
5.  Related tag blog - block which holds the last kind of tag classification
6.  Information block - contains data about the image
    1.  ID - numerical ID of the post
    2.  Uploader - self explanatory
    3.  Date - self explanatory
    4.  Source - where the image originated
    5.  Rating - contains the values: safe, questionable, explicit
7.  Comments block - self explanatory

[//]: # ([![danbooru_upload]({{ site.baseurl }}/assets/danbooru_upload-1024x455.png "Danbooru's upload page")](http://blog.7thwraith.net/wp-content/uploads/2013/04/danbooru_upload.png))

1.  File Upload
2.  Source - where the image originated
3.  Rating - degree of explicitness
4.  Parent ID - field to tie into a parent post
5.  Tag field - self explanatory
    1.  Related tags - general tags related to this image
    2.  Artist tags - name of artists associated to the image
    3.  Copyright tags - tags pertaining to name of series, company, etc

If you have not guessed yet, I plan to build a booru-style image board using CMS platform. The list above will be my guidelines. I will be elaborating more on this project but I shall save that for another post.

Do feel free to add if you feel like I've missed something.