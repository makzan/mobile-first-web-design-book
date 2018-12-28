# Chapter 2 – Content strategy

Content is king.

In this chapter, we focus on the fundamental of the web. It’s so fundamental that these techniques apply to both desktop web and mobile web design. It’s so fundamental that we often overlook and forget about it.

Table of Content for Chapter 2 – Content strategy:

1. Document title
2. Content strategy
3. Content structure
4. Mobile first approach
5. Sketching for mobile web
6. Minimal mobile friendly website
7. Listview
8. Do mobile web has to be a webpage?

## Document title

![Doc title](https://junkdraft.s3.amazonaws.com/attachments/1/652/original/3db7d56dc40dfb9640c41c77835fec2c3eac578d/doc-title-tab.png)

First thing is the title of the document. Title of the document is used in the following places:

- Home screen
- Bookmark
- History log
- Tab
- Back button in browser
- Social network

The following is the screen of sharing a webpage on Facebook. Facebook fetches the document title when it is shared.

![Title in Facebook sharing dialog](https://junkdraft.s3.amazonaws.com/attachments/1/653/original/1c5c85e42b9b5f4632547c507ac05b8bcf54ad63/fb-sharing.png)


This screenshot shows how confuse it is when every page shares the same document title.

![](https://junkdraft.s3.amazonaws.com/attachments/1/654/original/cd8277559d90d44760415dd6b8ec056a36561099/macao-gov-history.png)


This screenshot, on the other hand, shows the website with corresponding title set for each page.

![](https://junkdraft.s3.amazonaws.com/attachments/1/655/original/b98c2da0bc7007e7823c3cddbab0c7a0c9bfad85/makzan-net-history.png)

## Content strategy

Why we should care about content first?

Because no matter how the web and app present our content, the content itself doesn’t change. So the first thing we should focus is the content structure.

By structure, I meant the important order of our content. I meant the correct headings for our content. The informative HTML tags we applied to our content.

The next most important thing after document title is our headings.

Headings define the document outline. It shows the architecture of the essay.

Correct use of headings helps both readers and software process the content.
Our main heading (h1) may be used in many places. It could be the title of our essay that’s displayed in:

- Email newsletter
- Read later service

For detail about how we should use the headings, we may check the [reference to the W3C spec about the headings](http://www.w3.org/html/wg/drafts/html/master/sections.html#the-h1,-h2,-h3,-h4,-h5,-and-h6-elements).

### Exercise

Now try to make use of the HTML5 tags to write a news web page. You may create or copy dummy content. We focus only on the structure.

Try to write the core content first. Then add the author information. Then the category of this essay. Then add a website header and footer. Then add a navigation list. Then add a side bar to display related content. After adding all these things, can the reading tool still extract your essay content?

## Content structure

Remember, people don’t consume website. They consume content.

![](https://junkdraft.s3.amazonaws.com/attachments/1/657/original/f349dac5c2d504b5179fea5137d5a4e68486f10d/article-extraction.png)

The first step is not make your website fit in mobile. The first thing you should do is make your content fits in the mobile device.

Remember, people don’t consume website. They consume content.

There is an article view in mobile Safari. The iOS parsed the web page and try to extract the content for a better reading experience.

![](https://junkdraft.s3.amazonaws.com/attachments/1/658/original/75ea66ae920b5b25a1c25c5d8bdcda5bf00747f6/macao-portal-normal.png)

![](https://junkdraft.s3.amazonaws.com/attachments/1/659/original/a63284ab77c3e13a6886be3e78a3ded81d8b498d/macao-portal-article.png)

Moreover, most read-later service also supports content extraction. For example, the following screenshot shows how Pocket displays the content in its mobile app, with a good reading experience.

![](https://junkdraft.s3.amazonaws.com/attachments/1/660/original/d5422da5e657509648388dc09314ae925f6af8c6/macao-portal-pocket.png)

### Another example

![](https://junkdraft.s3.amazonaws.com/attachments/1/661/original/b15f2b7f8b0fe0ff648fe5bc55de2db466d213dd/hk-news-normal.png)
![](https://junkdraft.s3.amazonaws.com/attachments/1/662/original/b3747b73e752332a59a6deb6b85cf9305f32c619/hk-news-article.png)

### Yet another example

Similar article view is not only use in mobile but also desktop service, such as Evernote.

![](https://junkdraft.s3.amazonaws.com/attachments/1/663/original/b91ee829ba9cab10c279ea055cd741af0491ca73/evernote.png)

So how we could make the system or service extract the content correctly?
When we plan our HTML structure, we can make use of the `<article>` tag. Here is the explanation from Mozilla.

> The HTML `<article>` Element represents a self-contained composition in a document, page, application, or site, which is intended to be independently distributable or reusable, e.g., in syndication.
It’s often confusing when deciding when to use the section tag and when to use the article tag.

Good structure helps web service analysis your content.

Two quotes from the w3 spec helping us to choose between section and article.

> Authors are encouraged to use the article element instead of the section element when it would make sense to syndicate the contents of the element.

> When an element is needed for styling purposes or as a convenience for scripting, authors are encouraged to use the div element instead. A general rule is that the section element is appropriate only if the element's contents would be listed explicitly in the document's outline.

