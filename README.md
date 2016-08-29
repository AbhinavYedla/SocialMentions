# socmentionr
Description

Get Strength, Sentiment, Passion and Reach for a term. User can choose from five different sources. Blogs, MicroBlogs, Bookmarks, Images or combination of all the sources.

Usage

socialMention(term, source = "all", time.frame = "all")
Arguments

term	
- term for which user intend to get the data
source	
- An list indicating the source(s) from which the data has to be retrieved.
time.frame	
- An variable indicating the time frame for result data.
Details

term is any character string source can be Blogs, MicroBlogs, Bookmarks, Images, all (Any Source) or list of all of the mentioned sources. time.frame can be h, 12h, 24h, w, m or all. Meaning in respective order Last Hour, Last 12 Hours, Last Day, Last Week, Last Month or Anytime.

Value

A data frame consisting of data related to the term belonging to a source with in the given time frame.

Author(s)

Shawn Dorius sdorius@iastate.edu

Abhinav Yedla abhinavyedla@gmail.com

Examples

socialMention("United_States")

Date        Source     Term          Strength Sentiment Passion Reach TimeFrame

2016-08-11  all     United States       56       6:1      48    26       all

source <- "blogs"

time.frame <- "12h"

socialMention("India", source, time.frame)

Date         Source  Term       Strength Sentiment Passion Reach TimeFrame

2016-08-11  blogs     India       12       1:2       0     3       12h