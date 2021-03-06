---
layout: post
title:  Harry Potter and the Order of the Vowels
date: "2017-06-29 08:30:10"
image: /figure/source/harry-potter/occurrences.png
share-img: https://github.com/nathancunn/nathancunn.github.io/blob/master/figure/source/harry-potter/occurrences.png?raw=true
---

My post earlier this week on [why the 'except after c' rule is a bit useless](http://www.nathancunn.com/2017-06-26-i-before-e-except-after-w/) gathered [a lot more attention](https://www.washingtonpost.com/news/wonk/wp/2017/06/28/the-i-before-e-except-after-c-rule-is-a-giant-lie/) than I expected. Although largely positive feedback, inevitably when you say anything online, no matter how trivial or innocuous, you will have someone telling you that you're wrong, or that you are somehow everything that's wrong with the world:

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">nobody is taught the rule without the next part<br><br>this is why Trump won <a href="https://t.co/LnJx41JFvz">https://t.co/LnJx41JFvz</a></p>&mdash; Gerry Canavan (@gerrycanavan) <a href="https://twitter.com/gerrycanavan/status/880060763632750593">June 28, 2017</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
The criticisms primarily centred on:

-   **The rule is for children, and it definitely works if you just use words children would use** \[citation needed\] - this is a fair point, and largely why I decided to do the post in the first place.
-   **Examining the rule should account for frequency of use** - this is a similar point. If the rule's only exceptions are words nobody uses then that shouldn't count against it. I don't necessarily think weighting by frequency of use is the best approach, as I'll explain later, but certainly restricting the body of words looked at makes some sense.
-   **You're forgetting the rest of the rhyme, 'and when said A as in neighbour and weigh'** - people really seemed to get annoyed when I told them that this is completely irrelevant to whether or not the 'except after c' rule works; if you have a 'cei'/'cie' word, it doesn't matter how it's pronounced, 'cei' is what the rule suggests is correct, and 'cie' incorrect.

I decided to address the first two problems by examining the efficacy of the rule on a series of texts that relatively young children should have few problems with: the Harry Potter series. (I decided to address the third problem by continuing to assert that it's *not* a problem.) Text files of the books can be easily found through a Google search (sharing an actual link seems morally dubious). From there the analysis can be done as in the previous post, simply searching for all mentions of words which contain the 'cei' or 'cie' pairs. The ie/ei rule still holds, so I'm not looking at that here.

I've split all hyphenated words so that, e.g., 'high-ceilinged' would be the same as 'ceilinged'. In contrast to the previous post, however, this time I've accounted for the frequency of the words in the text.

<center>
<embed src="../figure/source/harry-potter/occurrences.svg" type="image/svg+xml" />
</center>
...and, it looks like the critics were right. Adjusting for frequency of use, the 'except after c' rule does hold, with at least 60% of occurrences in each book favouring 'cei' over 'cie'.

However.

This is predicated on the idea that adjusting for frequency of words is a *good* thing. I don't feel that's necessarily the case. Consider if you were examining a rule that said 'h always comes before e', the words satisfying this condition would almost certainly be dominated by the word 'the'. Therefore, once you learn how to spell 'the', the rule is no longer useful to you, because it likely unduly influenced the results.

That might seem like a stretch because surely no 'cei' word will be as dominant as the word 'the'. However, looking at the number of unique words which have a 'cei' or 'cie' pair in the Harry Potter series, the rule fares much worse:

<center>
<embed src="../figure/source/harry-potter/uniques.svg" type="image/svg+xml" />
</center>
In four of the books at least half of the words containing a 'cei' or 'cie' pair would've broken the rule. Interestingly, these are all the later books in the series, which might lend some credence to the idea that words which break the rule are more likely to be encountered by older, more experienced readers.

It's worth noting in all this, that there really aren't many words where the rule is relevant. It turns out that across all the books the *only* 'cei' words which come up are variations on 'ceiling', 'receive', 'perceive', 'conceit', and 'deceive'. 'Cie' words, on the other hand, are a little more numerous: science, ancient, species, fancies, glacier, sufficient, conscience, emergencies, societies, omniscient, deficient, efficient, prophecies.
