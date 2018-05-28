
# <img src="/static/img/jolly-roger-unshifted.jpg" width="60"> cryptoanarchy.wiki

If you're reading this, then it means that you're interested in contributing to [cryptoanarchy.wiki](https://cryptoanarchy.wiki). If you'd just like to view the site then please click [here](https://cryptoanarchy.wiki).

## For the Very Non-Technical:
Set up a github account, go to the "Issues" tab above and leave an issue with instructions on what information you'd like to see added to the repository, what corrections you'd like to make, etc.

## Basic Information

### Jekyll theme forked from:
* [agusmakmun/agusmakmun.github.io](https://github.com/agusmakmun/agusmakmun.github.io)

### Source code structure:
The site works primarily via [Jekyll Collections](https://jekyllrb.com/docs/collections/) (collections are defined in _config.yml). The primary types are as follows:

+ **Section** - This is for items that should be displayed in the hompage contents. There is a collection for each section on the homepage. The items within the collection form the list items below the header.
+ **Subsection** - This is for content which is to be listed on a section item's page (i.e. the page of a specific instance of the collection type above). An example of this type would be the "people" collection. Some of the items in this collection would be found on the "Early Cypherpunks" page.

If you create a new "section" type collection, you'll have to add it to index.html in order for it to display. If you create a new item within a "section" collection, then it will show up automatically. Note that ordering is done via a variable called "order" and you will have to +1 all of the order values for items after it in the list. I have an idea for a solution to this problem, but it's not implemented yet. You can have them show up as bare list-items (not links) by using the `no_content: true` flag. You can also use this collection type's item for an outbound link via the `external_link: true` flag.

If you want to create a new "subsection" type collection, you'll have to wire this up, but there are files in `_includes` that make this easy. To add a "subsection" items such as one in "people", you simply add a file to the relevant collection (and in the case of "people", add at least one category).

## Style Guide

### Spelling conventions
I use British spelling conventions because that's what I grew up with. For the sake of keeping the site internally consistent, I may ask you to "correct" your spellings to British spellings for any content you submit.

### Dates formats
Exact dates should be given in the following format: 31-Oct-2008. This is because this format is unambigious when accounting for US vs inernational date standards. Always use three-letter months. Other date formats I'll accept are:

+ 1990s (for a broad period of time without clear beginnings and ends)
+ Aug-Sep 2013 (for a month-to-month range in the same year)
+ Aug 2013-Sep 2015 (for a month-to-month range in different years)
+ 2008/2009 (for an ongoing period of time with an unclear start date - i.e. was Bitcoin created by the genesis block, or the announcement of the white paper?)

For new content that I create (i.e. that not directly imported from cypherpunk-research) I have started marking this with the date when they were true. For example:

> Wikipedia defines "[Cypherpunk](https://en.wikipedia.org/wiki/Cypherpunk)" as follows (2018-05-26)

In this instance I use (YYYY-MM-DD) because it's the shortest non-internationally-ambiguous date format.
