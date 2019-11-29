---
layout: post
title:  "Why and How I moved to Jekyll?"
date:   2019-11-29 12:38:58 +0100
categories: jekyll meta
---

I shouldn't be writting this but in my attempt to document everything that
takes me more than 2h to do and I may do in the future I'll try to explain
the steps plus reasons why I moved from
[blogdown](https://bookdown.org/yihui/blogdown/) back to
[jekyll](https://jekyllrb.com/).

## Why

The reasons are a bit stupid. I liked the
[academic theme](https://themes.gohugo.io/academic/) from blogdown/HUGO and
it was a nice integration to Rmarkdown documents. I use R for most of my code
/ data analysis tasks so it seemed like a nice integration.

I think main problem is that I am lazy and I didn't keep any blog up to date,
I barely have time to spend in the things that I planned to blog about (mainly
datavizz and my [r/dataisbeautiful](https://www.reddit.com/r/dataisbeautiful/))
so posts became less and less frequent.
Unrelated the forum has lost a bit of the R vibe that had previously in favour
of some sort of devotion for maps and sankey diagrams.
When I had time, it was also a pain to move code to a "notebook" type of
analysis. I used to love notebooks when I started but now I find myself in a
complete mess when I use them. I think I went a bit deeper in what now I do
with R so notebooks got smaller and smaller.

All together I find myself, from time to time (year to year) trying to remember
how the blogdown system works. Trying to update HUGO and fighting with
dependencies and broken links to data. I also found that was very complicated
to mantain a decentralized blog with many computers.

One extra thing that was a bit annoying was the hosting.
I originally set up a system where I bought a google domain and used
[Netlify](https://www.netlify.com/) to host the hugo blog. The expirience was
fun and I learned a lot about CI and web deployment. However, it wasn't easy
to mantain, hugo issues were appearing from time to time and you still had
to run the markdown documents locally which is inevitable but problematic at
the same time.

All these reasons may be summarized in me being lazy and not updating the
blog often enough. Howver, I wanted to change.
I thought that going to my last configurations using Jekyll would be a great
compromise solution because it's easy to set up and easy to left unmantained.

## How

This is a bit ridiculous because I spent way too much time setting this up
and it should have been an easy config. I messed up some things but finally
is up and running!

### Step1

TBC


## Default Jekyll post

You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

Jekyll requires blog post files to be named according to the following format:

`YEAR-MONTH-DAY-title.MARKUP`

Where `YEAR` is a four-digit number, `MONTH` and `DAY` are both two-digit numbers, and `MARKUP` is the file extension representing the format used in the file. After that, include the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
