# Notes

## Abstract

Headlines in major news outlets over the last five years reveal the profound suspicion with which statistical methods have been received within the humanities. The pervasive belief is that a chasm lies between statistics and the humanities that not only cannot be bridged but should not be attempted, at the risk of losing the human. And yet slowly and steadily a growing number of practitioners have not only developed research programs but also pedagogical methods that open up new analytical perspectives as well as new avenues for students to explore their relationship between the subject matter and their own understanding. This paper offers a small survey of various practices to be found in the digital humanities alongside a few experiments by the author in allowing students to experience how statistical methods in fact de-mystify the meaning-making process in language and empower students not only to ground their insights in things they can see, and count, but also, in understanding texts as nothing more than certain sequences of words, build write better. Working from a broad survey to narrow applications, the paper suggests that concerns about a loss of humanity in the humanities is actually a concern for loss of certain kinds of authority, but that new kinds of authority are possible within which researchers and teachers will find a firm ground from which to offer interpretations and evaluations of the kinds of complex artifacts that have long been the purview of the domain.

## Build Notes
- Twenty years ago the literary critic Stanley Fish complained that quantitative methods could only discover what is already known, but he forgot the importance of understanding the why and what of a text but the how. Data science as a microscope makes understanding how texts work trivial. 
- I’m not entirely sure what my assigned role is, but if it’s something like “using data science in the humanities,” then maybe framing it through “The Most Dangerous Game” isn’t a bad idea. In the humanities starting out with a data set to be understood except through statistical summary doesn’t jive with the tendency to focus on single objects,so I choose to use statistics to estrange the object and then bring it back into focus in ways students already understand but didn’t realize would be our destination.
- "Typical applications of textual data mining involve a trade-off: speed for accuracy, coverage for nuance. Such methods are efficient for industries, sectors, and disciplines that are dealing with so much textual data at such fast speeds that they cannot possibly (nor would want to) read it all or where one wants to extract from a large data set a relatively simple piece of information that is either actionable or that can be quickly labelled and classified along simple features." (Da 620)  
- *From the Retention Summit talk*: We spend 3 weeks on 8000 words, but, by the end of it, they know that text. They know it. They know something in a way they have too often not known it before. Not by what they already thought they knew, but by prolonged entanglement with the object itself. In some ways, this particular pedagogical moment is nothing more than a working out in the humanities of Pound's story of Aggasiz and the fish.
- _Des Chiffres et des Lettres_ has been running since 1965. At first the program had only the unscrambling of letters to produce the longest word. In 1972 they added combining numbers to match, or come closest to matching, a provided three-digit humber. What’s interesting about this: in reinforces the idea that letters and numbers are two distinct domains. 

## A Series of "Parts Schedules"

### Part Schedule 1: Frequencies
- words
- ngrams
- sentences
- paragraphs

### Part Schedule 2: Relations
- collocation network
- word2vec
- topic model


###  Part Schedule 3: Controlled Vocabularies
 
- What about putting all quotation/dialogue in a color — like Mahlberg and Wiegand do — but is that a frequency or a relation? **Frequency**, I think. 

## Brezina on "Discourse"[^1](youtube.com/WX0u-lj3dkw)
- Why focus on discourse?
	- focus on communication of **meaning** not form
	- focus on **connections between words** not single words
	- focus on **repeated patterns** not one-off occurrences
	- focus on both quantitative and qualitative exploration
- Association measures (statistical procedures)
	- Tokens in corpus (overall size)
	- Frequency of node/word
	- Frequency of collocate anywhere in corpus
	- Frequency of collection of node word and collocate
expected = node x collocation / corpus size

MI = log2 (observed / expected)

### Collocation Criteria
1. distance
2. frequency
3. exclusivity
4. dispersion
5. directionality
6. type-token distribution
7. connectivity

Stubbs, M. (2005). Conrad in the computer: examples of quantitative stylistic methods. Language and Literature, 14(1), 5–24. https://doi.org/10.1177/0963947005048873

Short, M. (2007). Thought Presentation Twenty-five Years On. Style, 41(2), 227-243. Retrieved from http://www.jstor.org/stable/10.5325/style.41.2.227

## Draft 1

> In the humanities starting out with a data set to be understood except through statistical summary doesn’t jive with the tendency to focus on single objects, so I choose to use statistics to estrange the object and then bring it back into focus in ways students already understand but didn’t realize would be our destination.


## Sum|marize

The pedagogy I am about to discuss is perhaps best described as a pedagogy of exhaustion. At the beginning of a semester in which I teach the freshman honor’sI English seminar, I assign students an eight thousand word short story to read before the first day of class. When they walk into the room on the first day, I first quiz them to let them know I’m serious about them getting work done, and then I let them discuss the story however they are used to doing. Typically this involves a fairly formless series of unconnected statements which often drag up things like symbols — whatever those are (because they don’t know; they just know symbols are important). What the students can’t know at the end of this first class is that we are going to spend the next 3 weeks on this one text. 3 weeks. 8000 words. Exhaustion.

We spend 3 weeks on 8000 words, but, by the end of it, they know that text. They know it. They know something in a way they have too often not known it before. Not by what they already thought they knew, but by prolonged entanglement with the object itself. In some ways, this particular pedagogical moment is nothing more than a working out in the humanities of Pound's story of Aggasiz and the fish.

The story we read is "The Most Dangerous Game" written by Richard Connell and published in Collier's in 1924. I chose it because of how well established it is in American popular culture and because it will enter the public domain in 2020. While many of you may not have read the short story, all of you will know its essential plot of a famous hunter ending up being hunted. It is almost a rule, I think -- let's call it Laudun's Rule -- that if a television series goes long enough, it will feature an episode with a version of "the most dangerous game." (My favorite is Archer's "El Contador.")

My copy of the story began life as a PDF linked from the story's Wikipedia page. I stripped it to bare text, and I then re-produce it as a PDF with the same number of pages as students in the class. On the second day of class, after students have run out of steam with their own analyses, I ask them to summarize the story. They flounder, because writing a summary of fiction is somewhat difficult. How do you prioritize events within a story? 

My suggestion is to them to let the text do the work: I assign each student the task of designating one sentence from a given pageant that best represents what happens on that page. We compile the 16 sentences and then check for redundancy, with the goal of either eliminating redundancy or transforming it into a qualification or digression that adds nuance to the summary. 

As we discuss the strengths of this method, I do not use words like *set* and *subset* and instead of distinguishing between extractive and abstractive methods, we discuss the difference between quotative and paraphrased summaries. My argument for this method is that it is mechanical. "Let the text do the work," I tell them. With each page averaging between 450 to 500 words, a 20-word sentence achieves a 20-to-1 compression. 

What I stress for them is that writing a summary requires discipline, which in most instances we recognize as a method, a theoretically-informed method, which is nothing more than a reliable, repeatable process with clear instructions. `Capture one sentence per page; compile; reduce redundancy` is a clear, repeatable method. 

Having demonstrated the utility of such an approach, I then ask them to tell me not what the story means but how the story achieve its possible meaning(s). After all, whether it is oral or written, discourse is nothing more than a string of words. In the stream of oral discourse, we define a text as a chunk of words that can be removed from one event and transported to another. Portability, then, is a key element of texts, and understanding the dynamics of removing a text from one context, holding it in the brain, and then inserting it into another context is one of the central foci of my home field of folklore studies. 

Written texts come pre-packaged -- _prêt à porter_, if you like. They are fixed string of words, a coded sequence we so readily ingest/download that we don't think about the nature of the operation, until we are stuck in a room with an English professor. My job is to convince my students, and perhaps you, that texts are nothing more than meaning-making machines and as such can be mechanically broken down, as some of us still do with other machines in our world. The trick is to piece out the parts and much of what comes next is creating different parts schedules that can, perhaps, be overlaid to discover how a text works. 

Much of what follows is simply a variation on a theme: how can various forms of counting reveal the way a text work? Simple descriptive statistics deployed in the service of understanding how 8017 words make up 700 sentences that make up 206 paragraphs that make up 1 story that has become in its almost 100 year a history an important part of our cultural matrix. 

## Part Schedule 1: Word Frequencies

One of the things I regularly skip past is how we define the constituent elements of a population. While I might find discussions about tokenization thought-provoking -- e.g., is the contraction *can't* one word or two? -- I keep the discussion, and the code, focused on commonsensical perspectives. And that means that *can't* is one word and so is *you've* because to break them up into either the somewhat nonsensical NLP conventions of *ca* and *n't* is more into the weeds than I wish to wander. I also don't worry about stemming, for reasons that I hope will become clear in a moment.

Thus, when I tell them that the 8000 word story is composed of a little less than two thousand words, they are a bit surprised simply because they've never thought about the fact of how redundant language, especially when it comes to the small things. 

A simple graph of the 50 most common words works well: I ask them to tell me which of those words is at all significant to the story. (FTR, no one ever chooses *the*.) 

## Part Schedule 2: Word Relations

##  Part Schedule 3: Sentence Lengths (or paragraph lengths)


Quotatives fit in here somewhere. 

##  Part Schedule 4: Controlled Vocabularies


[^1](#): For more background information and to begin to get a sense of just how many times the story has been adapted see the Wikipedia entry: [https://en.wikipedia.org/wiki/The\_Most\_Dangerous\_Game](https://en.wikipedia.org/wiki/The_Most_Dangerous_Game)


## Draft 2: "Are we not doing phrasing anymore?"

**Abstract**: This paper offers a small survey of various practices to be found in the digital humanities alongside a few experiments by the author in allowing students to experience how statistical methods in fact de-mystify the meaning-making process in language and empower students not only to ground their insights in things they can see, and count, but also, in understanding texts as nothing more than certain sequences of words. 

> Narratives are situated: they must be interpreted in light of a specific discourse context or occasion for telling. 

We deal with this dimension first because it is the one least susceptible, at least on the surface, of being examined with data science methods. As a folklorist, I think of this as two people talking, and in the middle of that talk one person tells another a story. The nature of that story is shaped by what has come before and, in turn, it shapes what comes next. It's also the case that the story is shaped by other stories like it that have come before and will, if successful, shape stories that will come next — and it may even help shape subsequent stories if it is unsuccessful. (e.g., We make mental notes about what works and what doesn't.) Thus there are both performance contexts as well as traditional, or intertextual contexts. Textual webs are obviously open to exploration through data science, and, we'll see in a moment, even some of the performance contexts are open to examination through recent developments in cognition studies.

> A narrative cues interpreters to draw inferences about a structured time-course of particularized events. 

> In turn, these events are such that they introduce some sort of disruption or disequilibrium into a storyworld involving human or human-like agents, whether that world is presented as actual or fictional, realistic or fantastic, remembered or dreamed, etc. 

> Narratives convey the experience of living through a storyworld-in-flux, highlighting the pressure of events on real or imagined consciousnesses affected by the occurrences at issue: qualia. 