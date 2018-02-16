---
title: Submission guidelines
layout: default
---

## Structure
Each post should start with a header information, starting and ending with a line with three slashes '---'. Then, three meta-information shall be inserted:
- title - a short title. Can be nested into quotes to prevent special characters (e.g. colons) from breaking the text.
- author - authors of the contribution and their affiliations, preferably in 
- category
        ---
        layout: default
        title: "XenGen: Web-Based Deployment of FMI Models"
        author: Michael Tiller ([Xogeny](http://www.xogeny.com))
        category: "vendor"
        ---
        ![XOGENY](https://www.modelica.org/publications/newsletters/2015-1/images/iPad_Portrait_Design.png)

        Xogeny is proud to announce that we will be demonstrating our latest tool, XenGen. XenGen is a tool that transforms FMI compliant models (FMUs) into web-based applications. Come see us on Monday, September 21st at 5:00pm in the "Colbert" room at the Modelica Conference.

Hello world!

We do propose the following categories:
-  MA
-  Meetings
-  Vendor
-  Education
-  Library

here is the set of all [categories](google.com):

{% for collection in site.collections %}
{% assign name = collection.label %}
## {{ name }}
    {% for page in site.[name] %}
  [{{ page.title }}]({{ page.url }}) - {{ page.category }}
    {% endfor %}    
{% endfor %}
