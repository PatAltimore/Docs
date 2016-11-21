---
# required metadata

title: [ARTICLE TITLE | Microsoft Docs]
description: [BRIEF DESCRIPTION ARTICLE]
keywords:
author: [YOUR GITHUB USERNAME]
ms.author: 
manager:
ms.date: [TODAY'S DATE IN MM/DD/YYYY FORMAT]
ms.topic:
ms.prod:
ms.service:
ms.technology:
ms.assetid: 

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
#ms.reviewer:
#ms.suite:
#ms.tgt_pltfrm:
#ms.custom:

---

# docs.microsoft.com article template

This docs.microsoft.com template contains examples of markdown syntax. It is part of the [contributor's guide](/contribute, and referenced in [Create a new docs.microsoft.com article](create-new-article.md). 

You may find it useful to review both the [raw markdown for this file](https://raw.githubusercontent.com/Microsoft/Docs/master/ContributorGuide/template.md) and the [published article](./template.md).

## Basic Markdown and GFM

All basic and Github-flavored markdown is supported. For more information on these, see:

- [Baseline markdown syntax](https://daringfireball.net/projects/markdown/syntax)
- [Github-flavored markdown (GFM) documentation](https://guides.github.com/features/mastering-markdown)

## Headings

Examples of first- and second-level headings are above. 

There **must** be only one first-level heading in your topic, which will be displayed as the on-page title.  

Second-level headings will generate the on-page TOC that appears in the "In this article" section underneath the on-page title.

### Third-level heading
#### Fourth-level heading
##### Fifth level heading
###### Sixth-level heading

## Text styling

*Italics* 

**Bold** 

~~Strikethrough~~



## Links

To link to a markdown file in the same Github repository, use [relative links](https://www.w3.org/TR/WD-html40-970917/htmlweb.html#h-5.1.2). 

- Example: [Create a New docs.microsoft.com Article](create-new-article.md)

To link to a header in the same markdown file, view the source of the published article, find the id of the head (e.g. `id="blockquote"`, and link using # + id (e.g. `#blockquote`).

- Example: [Blockquotes](#blockquote)

To link to a header in a markdown file in the same repo, use relative linking + hashtag linking.

- Example: [technical overiew of the sign-up process](./understand-explore/rms-for-individuals-user-signup.md#technical-overview-of-the-sign-up-process)

To link to an external file, use the full URL as the link.

- Example: [Github](http://www.github.com)

If a URL appears in a markdown file, it will be transformed into a clickable link.

- Example: http://www.github.com

## Lists

### Ordered lists

1. This 
1. Is
1. An
1. Ordered
1. List  


#### Ordered list with an embedded list

1. Here
1. comes
1. an
1. embedded
    1. Miss Scarlett
    1. Professor Plum
1. ordered
1. list


### Unordered Lists

- This
- is
- a
- bulleted
- list


##### Unordered list with an embedded lists

- This 
- bulleted 
- list
    - Mrs. Peacock
    - Mr. Green
- contains  
- other
    1. Colonel Mustard
    1. Mrs. White
- lists


## Horizontal rule

---

## Tables

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| col 1 is default | left-aligned     |    $1 |


## Code

### Codeblock

    function fancyAlert(arg) {
      if(arg) {
        $.docs({div:'#foo'})
      }
    }

### In-line code

This is an example of `in-line code`.

## Blockquotes

> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## Images

### Static Image

![this is the alt text](media/azure.png)

### Linked Image

[![alt text for linked image](./media/azure.png)](https://docs.microsoft.com) 

## Alerts

### Note

> [!NOTE]
> This is NOTE

### Warning

> [!WARNING]
> This is WARNING

### Tip

> [!TIP]
> This is TIP

### Important

> [!IMPORTANT]
> This is IMPORTANT

## Videos

### Channel 9

<iframe src="http://channel9.msdn.com/Series/Azure-Active-Directory-Videos-Demos/Azure-Active-Directory-Connect-Express-Settings/player" width="960" height="540" allowFullScreen frameBorder="0"></iframe>


### Youtube

<iframe width="420" height="315" src="https://www.youtube.com/embed/R6_eWWfNB54" frameborder="0" allowfullscreen></iframe>

## docs.ms extentions

### Button

> [!div class="button"]
[button links](/rights-management)

### Selector

> [!div class="op_single_selector"]
- [foo](/rights-management/template.md)
- [bar](/rights-management/scratch.md)

### Step-By-Step

>[!div class="step-by-step"]
[Pre](https://www.example.com)
[Next](https://www.example.com)