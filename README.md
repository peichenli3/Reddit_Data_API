# Reddit WSB Webscraping

If you want to know about short selling, short sqeeze, GameStop and subreddit WallStreetBets, You probably want to read [this article](https://www.gq.com.au/success/finance/your-guide-to-gamestop-rwallstreetbets-and-the-short-squeeze-that-has-wall-st-in-chaos/news-story/46e90e8b16744794bfaadd5089afcc15).
Personally I find it quite enjoyable. Now back to our story. Technology breakthrough in the recent years is quite fascinating. It enpowers researchers in finance/econ great tools to analysis unstructured data.
Tools in natural language process area has made it possible for finance researchers to analysis its information. You may wonder why text data can be of our interest? Well, right after [the speech](https://www.wsj.com/articles/feds-powell-to-take-questions-on-job-market-interest-rates-bond-yields-11614872817) given my Fed Chairman powell on 03/04/2021, you can notice the big move of market.
What if we can analyze his speech text and do a series of analysis? That could be interesting! And this kind of textual analysis in not uncommon in finance. See related [paper1](https://github.com/MS20190155/Measuring-Corporate-Culture-Using-Machine-Learning),
[paper2](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3286887). For paper 1 in particular, it mainly uses Stanford NLP package [Stanza](https://stanfordnlp.github.io/stanza/index.html). I believe up to now it has been merged into [spaCy](https://spacy.io/universe/project/spacy-stanza) for easier use.
Now suppose you have the ideal statistical tools for textual analysis. What text data can be used? Paper 1 uses firm earning call transcripts while paper 2 utilizes patent documents.

## Description

Ok, now what if you want to use text data from subreddit wallstreetbets to better analyze the short squeeze frenzy event in early 2021? This github repo is the destination for you.
In short, I used the [Pushshift API](https://pushshift.io/) to extract the raw reddit data. You can see its Github repo [here](https://github.com/pushshift/api).
Why use Pushshift API? Well, there are also some other alternatives like ([PRAW](https://praw.readthedocs.io/en/latest/) in Python, and a wonderful package called [RedditExtractoR](https://cran.r-project.org/web/packages/RedditExtractoR/RedditExtractoR.pdf))
But unfortunately due to the limit of [Reddit API](https://www.reddit.com/dev/api/), you can only extract 1000 posts once. It may be impossible to extract all posts from WallStreetBets in a given period.

This project can serve as a data pipeline for textual analysis of reddit data. In particular, I'm going to use PushShift API to extract all raw data from subreddit Wallstreetbets, do some data cleaning and extract useful information.
In the end, I would convert the data into pickle format to make your NLP analysis easier. Pickle can be read into Python in few seconds.

## Getting Started

### Dependencies

* Describe any prerequisites, libraries, OS version, etc., needed before installing program.
* ex. Windows 10

### Installing

* How/where to download your program
* Any modifications needed to be made to files/folders

### Executing program

* How to run the program
* Step-by-step bullets
```
code blocks for commands
```

## Help

Any advise for common problems or issues.
```
command to run if program contains helper info
```

## Authors

Contributors names and contact info

ex. Dominique Pizzie  
ex. [@DomPizzie](https://twitter.com/dompizzie)

## Version History

* 0.2
    * Various bug fixes and optimizations
    * See [commit change]() or See [release history]()
* 0.1
    * Initial Release

## License

This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details

## Acknowledgments

Inspiration, code snippets, etc.
* [awesome-readme](https://github.com/matiassingers/awesome-readme)
* [PurpleBooth](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
* [dbader](https://github.com/dbader/readme-template)
* [zenorocha](https://gist.github.com/zenorocha/4526327)
* [fvcproductions](https://gist.github.com/fvcproductions/1bfc2d4aecb01a834b46)
