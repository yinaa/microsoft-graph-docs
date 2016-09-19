


# Overview of Microsoft Graph

Microsoft Graph exposes multiple APIs from Microsoft cloud services through a single REST API endpoint: **https://graph.microsoft.com**. This simplifies the queries you use to access resources. 
 
You can use Microsoft Graph to:

- Access data from multiple Microsoft cloud services in a single response.
- Navigate between entities and relationships powered by the Office Graph (for commercial users).
- Access intelligence and insights from the Microsoft cloud.

**Microsoft Graph developer stack**

![Microsoft Graph API developer stack.](./images/MicrosoftGraph_DevStack.png)

With Microsoft Graph, you can:

- Use any development environment you choose.
- Use any  programming language, development platform, and hosting environment.
- Build an  app that accesses the Microsoft Graph API using any web language.  
- Use the IDE of your choice.
- Host your apps in Microsoft Azure or any cloud platform.
- Develop apps for a variety of device platforms.
- Call the Microsoft Graph API from Office or SharePoint add-ins.

<!--<a name="msg_queries"> </a>-->

##Common Microsoft Graph queries


| **Operation**	| **Service endpoint** |
|:--------------------------|:----------------------------------------|
|   GET my profile |	`https://graph.microsoft.com/v1.0/me` |
|   GET my files|	`https://graph.microsoft.com/v1.0/me/drive/root/children` |
|   GET my photo	 | `https://graph.microsoft.com/v1.0/me/photo/$value` |
|   GET my mail |	`https://graph.microsoft.com/v1.0/me/messages` |
|   GET my high importance email | `https://graph.microsoft.com/v1.0/me/messages?$filter=importance%20eq%20'high'` |
|   GET my calendar |	`https://graph.microsoft.com/v1.0/me/calendar` |
|   GET my manager	| `https://graph.microsoft.com/v1.0/me/manager` |
|   GET last user to modify file foo.txt |	`https://graph.microsoft.com/v1.0/me/drive/root/children/foo.txt/lastModifiedByUser` |
|   GET unified groups I’m member of|	`https://graph.microsoft.com/v1.0/me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')` |
|   GET users in my organization	 | `https://graph.microsoft.com/v1.0/users` |
|   GET group conversations |	`https://graph.microsoft.com/v1.0/groups/<id>/conversations` |
|   GET people related to me	| `https://graph.microsoft.com/beta/me/people` |
|   GET files trending around me |	`https://graph.microsoft.com/beta/me/trendingAround` |
|   GET people I am working with	 | `https://graph.microsoft.com/beta/me/workingWith` |
|   GET my tasks	| `https://graph.microsoft.com/beta/me/tasks` |
|   GET my notes |	`https://graph.microsoft.com/beta/me/notes/notebooks` |

<!-- <a name="msg_roof"> </a> -->

##Explore Microsoft Graph

- Learn more about how to [authenticate]() your Microsoft Graph app.
- [Get started]() using Microsoft Graph and the platform of your choice.
- Discover the resources and operations that you can use in your production environment by browsing the TOC.
- Preview the new [beta APIs]().
- Visit the [Microsoft Graph Explorer]().

 >  Your feedback is important to us. Connect with us on [Stack Overflow](http://stackoverflow.com/questions/tagged/office365+or+microsoftgraph). Tag your questions with [MicrosoftGraph] and [office365].



