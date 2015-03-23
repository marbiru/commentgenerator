# commentgenerator
Code for the Comment Generator project, creating random blocks of vapid text for various social situations.

## Overview

Comment Generator concatenates little pieces of text/vocabulary to create plausible-sounding jargon-filled comments that an annoying person could use in class (or at a startup party, or whatever).

## Mechanisms

Basically, CG is a random number generator tied to a small collection of words and phrases. When you click "Regenerate", the CG concatenates some vapid empty phrases (e.g. "Isn't it the case that" or "Surely we can all agree that") with some domain-specific jargon to create a Comment roughly 15-30 words in length.

## Philosophy

CG is meant to be funny, and funny for about 5-20 "regenerations" in each domain. The idea is to make each sentence in a domain sufficiently similar that the reader's brain can tell there must be something mechanistic creating the sentences – the whole joke is that some real-life people make such empty comments that they might as well be concatenating random strings – but with enough variation that the variations also feel funny. This is obviously a judgement call. Then, each different generator in a different domain should be sufficiently different that they're not just implementing the exact same concept with a different set of subject-specific jargon, because that would get boring.

##  To-do list

- separate out css, html and javascript into separate pages
- create a menu of some sort to make it easy to navigate between different generators
- do some css/design to improve presentation
- a lot of the code is repeated across different generators. Would it be preferable to have the functions written out just once and then called 
- the current setup has one variable creating a list of vocab and a second variable choosing a random element of that list. Is that really necessary? Can it be compacted into one variable? In a lot of cases maybe the list doesn't even really need a name because it's only used once.
