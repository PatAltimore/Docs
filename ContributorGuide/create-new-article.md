---
# required metadata

title: Creating a New docs.microsoft.com Article | Microsoft Docs
description: A guide for creating a new article within a Microsoft Docs repository
keywords:
author: msmbaldwin
ms.author: mbaldwin
manager: mbaldwin
ms.date: 11/21/2016
ms.topic: article
ms.prod:
ms.service:
ms.technology:
ms.assetid: 568792af-19f4-4d94-8b21-c94a103d863b

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
#ms.reviewer: [ALIAS]
#ms.suite: 
#ms.tgt_pltfrm:
#ms.custom:

---

# Creating a new docs.microsoft.com Article

Here are steps on creating a new article within a docs.microsoft.com Github repository:

1. Fork, clone, and set remote aliases for the Github repository to which you wish to contribute, using the guidance in [Git and GitHub initial setup](git-and-github-repository-initial-setup).

1. Create a new branch for your new article, using the guidance in the [Creating a local working branch](contributing-and-publishing.md#creating-a-local-working-branch) section of [Major contributions and publishing](contributing-and-publishing.md).

1. Copy the [docs.microsoft.com article template](template.md) to your local repository. If you had previously forked and cloned https://github.com/Microsoft/azure-docs for instance, and wished to create a new article for the virtual machines service, you would copy the template to ~/azure-docs/articles/virtual-machines.

  Alternatively, you copy the raw markdown of the template file [from here](https://raw.githubusercontent.com/Microsoft/Docs/master/ContributorGuide/template.md), paste it into a new file in the text editor of your choice, and save it to the desired location in your local repo.

1. Update the following fields in the standard metadata block:

  * **title**: The article's title.  The title field should end with "! Microsoft Docs", per the template (e.g., "About Linux virtual machines | Microsoft Docs").
  * **description**: Provide a brief description for your new article, no longer that 180 characters (e.g. ("Learn about the basics of Linux virtual machines in Azure using both deployment models.")
  * **author**: Your Github username
  * **ms.date**: The current date in MM/DD/YYYY format (e.g., 11/28/2016).
  
  Leave the other metadata fields blank; a Microsoft writer will provide the appropiate values as part of publication.

1. Delete the body of the copied template file and write your new article. Before deletion you may wish to read the template content, however, as it provides guidance on markdown syntax and docs.microsoft.com-sepcific markdown extentions. 

  Articles should:

  * Have one (and only one) H1 header, speficying the title of the article.
  * Use H2 headers sparinging, as these populate the righthand-sidebar on docs.microsoft.com.
  * Adhere to the principles outlined in the [Style and voice cheat sheet](style-and-voice.md)

1. Check in your new article as you would any change to our content set, following the guidance in the [Committing changes to your local working branch](contributing-and-publishing.md#committing-changes-to-your-local-working-branch) section of [Major contributions and publishing](contributing-and-publishing.md).

## See also

* [docs.microsoft.com contributor's guide](index.md)
* [Major contributions and publishing](contributing-and-publishing.md)
* [docs.microsoft.com article template](template.md)
