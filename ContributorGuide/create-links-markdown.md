<properties
   pageTitle="Create links in markdown articles" description="Explains how to code crosslinks in markdown." metaKeywords="" services="" solutions="" documentationCenter="" authors="tysonn" videoId="" scriptId="" manager="carolz" />

<tags ms.service="contributor-guide" ms.devlang="" ms.topic="article" ms.tgt_pltfrm="" ms.workload="" ms.date="02/03/2015" ms.author="tysonn" />

# Linking guidance for Azure technical content

### Links from one article to another

To create an inline link from one technical article to another, use the following link syntax:  

- An article in a service directory links to another article in the same service directory:

  `[link text](article-name.md)`

- An article links from a service subdirectory to an article in the root directory:

  `[link text](../article-name.md)`

- An article in the root directory links to an article in a service subdirectory: 

  `[link text](./service-directory/article-name.md)`

- An article in a service subdirectory links to an article in another service subdirectory:

  `[link text](../service-directory/article-name.md)`
 

## Links to anchors

You do not have to create anchors - they are automatically generated at publishing time for all H2 headings. The only thing you have to do is create links to the H2 sections.

- To link to a heading within the same article:

  `[link](#the-text-of-the-H2-section-separated-by-hyphens)`  
  `[Create cache](#create-cache)`

- To link to an anchor in another article in the same subdirectory:

  `[link text](article-name.md#anchor-name)`
  `[Configure your profile](media-services-create-account.md#configure-your-profile)`

- To link to an anchor in another service subdirectory:

  `[link text](../service-directory/article-name.md#anchor-name)`
  `[Configure your profile](../service-directory/media-services-create-account.md#configure-your-profile)`


## Links from includes

Since include files are located in another directory, you will need to use longer relative paths as shown below. To link to an article from an include file, use this format:

    [link text](../articles/service-folder/article-name.md)
    

## Reference-style links

You can use reference style links to make your source content easier to read. The reference style links replace the inline link syntax with simplified syntax that allows you to move the long URLs to the end of the article. Here's Daring Fireball's example:

Inline text:

    I get 10 times more traffic from [Google][1] than from [Yahoo][2] or [MSN][3].

Link references at the end of the article:

    <!--Reference links in article-->
    [1]: http://google.com/
    [2]: http://search.yahoo.com/  
    [3]: http://search.msn.com/

Make sure you include the space after the colon, before the link. When you link to other technical articles, if you forget to include the space, the link will be broken in the published article. 

## Using an absolute URL 

To link to an article that is not part of the technical documentation set (ie: in a different URL domain), use an absolute URL, but omit the locale. 

    [link text](http://azure.microsoft.com/pricing/details/virtual-machines/)


## Do not embed the language-locale segment in a link

When you need to link to a localized article, but sure to remove the embedded language-locale segment from the link (for example, "en-us"). This will allow the link to correctly redirect to the localized version of the page, if available.

### Use friendly link text for all links

The words you include in a link should be friendly - in other words, they should be normal English words or the title of the page you are linking to. Do not use "click here". It's bad for SEO and doesn't adequately describe the target.

**Correct:**

- `For more information, see the [contributor guide index](https://github.com/Microsoft/Docs/blob/master/ContributorGuide/readme.md).`

- `For more details, see the [SET TRANSACTION ISOLATION LEVEL](https://msdn.microsoft.com/library/ms173763.aspx) reference.`

**Incorrect:**

- `For more details, see [https://msdn.microsoft.com/library/ms173763.aspx](https://msdn.microsoft.com/library/ms173763.aspx).`

- `For more information, click [here](https://github.com/Azure/azure-content/blob/master/contributor-guide/contributor-guide-index.md).`

### Contributors' Guide Links

- [Overview article](readme.md)

<!--image references-->
[1]: ./media/create-tables-markdown/table-markdown.png
[2]: ./media/create-tables-markdown/break-tables.png
