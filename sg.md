---
title: Submission guidelines
layout: default
---
## Process
Everyone is welcome to contribute a post to the Modelica newsletter, however the editor holds the right to decline without reason. Please create a pull request to the newsletter repository.

## Structure
Each post should start with a header information, starting and ending with a line with three slashes '---'. Then, three meta-information shall be inserted:
- `title` - a short title. Can be nested into quotes to prevent special characters (e.g. colons) from breaking the text.
- `author` - authors of the contribution and their affiliations, preferably including hyperlinks `[Modelica Association](http://modelica.org)`
- `category` - a category of the post. Currently, these four categories are currently accepted:
  - `"association"` - news regarding Modelica association
  - `"education"` - news regarding educational resources, or training  
  - `"library"` - news regarding new or improved libraries
  - `"vendor"` - news regarding new Modelica tools versions
  
## Markdown syntax   
For the text body, use the [kramdown](https://kramdown.gettalong.org/) flavor of the Markdown syntax. See the [quick reference](https://kramdown.gettalong.org/quickref.html).

## Images
Each post is welcome to have one image. Please commit the image together with your post, e.g.

    ![](logo.jpg)

or provide an absolute address, e.g.

    ![](https://modelica.org/logo.jpg)
    
## Preview
If writing directly in GitHub, make use of the *Preview changes* - a live formatted preview of your text, including the images.

## Example
You can use the following code as a basis for your article:

    ---
    title: FMI User Meeting at the Modelica Conference 2015
    author: Christian Bertsch ([Robert Bosch GmbH](https://www.bosch.com/))
    category: ma
    ---
    ![FMI lofo](http://fmi-standard.org/assets/img/fmi-logo.svg "FMI image")

    The FMI Project will organize an "**FMI User Meeting**" within the tutorial/workshop session on the first day of the Modelica Conference 2015 as a complement to the scientific track(s) on FMI. *(Notice the line break here)*\
    The intention is to increase the interaction between FMI users in different companies / institutions and the Modelica Association Project FMI.

    ### Agenda
    - FMI overview
    - FMI current status
    - future developments \\
      (a longer discussion is anticipated here)
    - conclusion

## Example output
This code would yield the result in GitHub preview similar to this: \\
(The table with the meta information would be stripped in the final output)

| title  | author | category |
| :----: | :----: | :----: | 
| FMI User Meeting at the Modelica Conference 2015 | Christian Bertsch ([Robert Bosch GmbH](https://www.bosch.com/)) | ma |


![FMI lofo](http://fmi-standard.org/assets/img/fmi-logo.svg "FMI image"){:height="250px" width="250px"}

The FMI Project will organize an "**FMI User Meeting**" within the tutorial/workshop session on the first day of the Modelica Conference 2015 as a complement to the scientific track(s) on FMI.   
The intention is to increase the interaction between FMI users in different companies / institutions and the Modelica Association Project FMI.

### Agenda
- FMI overview
- FMI current status
- future developments   
  (a longer discussion is anticipated here)
- conclusion
