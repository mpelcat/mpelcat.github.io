---
title: Research Tips
---

Here are some frequently given pieces of advice for research. They are gathered here for students to inspire from when putting in place their research method. Please note that this content is provided by Maxime Pelcat, IETR, INSA Rennes under the GNU Affero copyleft license. Most elements are my opinion on the subjects, and are subject to discussions.

## Useful external resources

from Vincent Lepetit: [https://vincentlepetit.github.io/files/paper_writing.pdf](https://vincentlepetit.github.io/files/paper_writing.pdf)

from Fredo Durant: [http://people.csail.mit.edu/fredo/student.html](http://people.csail.mit.edu/fredo/student.html)

## Reading scientific articles

All scientific papers are written using the same method.

[https://en.wikipedia.org/wiki/IMRAD](https://en.wikipedia.org/wiki/IMRAD)

Some reading tips:

- A (conference) paper shall be read, and understood, with increasing depth, in:
  - 5 minutes, reading title and abstract
  - 10 minutes, additionally reading figures and conclusion
  - 20 minutes, additionally reading contributions and results
  - 1 or 2 hours, reading the whole paper

Each group below tells the same "little story" with an increasing amount of details:
- {title,abstract}
- {title,abstract,figures, conclusion}
- {title,abstract,introduction,contributions,results}
- {whole paper}

A journal paper, usually longer in number of pages, requires more time for each type of reading but the structure remains the same.

## Finding scientific articles

You can find PDF versions of articles on the free access Google Scholar repository: 
- [https://scholar.google.com/](https://scholar.google.com/)

and on websites accessible for a fee, depending on your institution subscriptions:
- [https://dl.acm.org/](https://dl.acm.org/)
- [https://ieeexplore.ieee.org/Xplore/home.jsp](https://ieeexplore.ieee.org/Xplore/home.jsp)
- [https://www.elsevier.com](https://www.elsevier.com)
- [https://www.springer.com](https://www.springer.com)

Many other websites reference publications, sometimes with PDFs. Open archiving systems include:
- [https://arxiv.org/](https://arxiv.org/)
- [https://hal.archives-ouvertes.fr/](https://hal.archives-ouvertes.fr/) (where we reference our publications)
- [https://tel.archives-ouvertes.fr/](https://tel.archives-ouvertes.fr/) (same as HAL for PhD thesis and HDR documents)

## Building a state-of-the-art review on a subject

You can combine several methods to build a state-of-the-art:
- find a recent survey on the subject
- find a recent paper on the subject and explore, breadth-first, its tree of references (i.e. you look in its references for the ones that are close enough to your subject; read these publications, and recursively look at their own references)
- use keywords on a paper repository such as [https://scholar.google.com/](https://scholar.google.com/)

Never read without writing something; otherwise you will forget. You can use a tool like [Zotero](https://www.zotero.org/) to organize your read papers.

## Evaluating publications (conferences and journals)

A good practice is to build your bibliography on peer reviewed publications, i.e. publications evaluated and accepted by expert reviewers with an external view on the subject. When you read a paper, check where it has been published.

Publications ranking is definitely not an exact science but here are some ranking websites for **conference** publications:
- [http://www.conferenceranks.com/](http://www.conferenceranks.com/)
- [http://portal.core.edu.au/conf-ranks/](http://portal.core.edu.au/conf-ranks/)

Conferences are ranked A*, A, B, or C based mostly on their acceptance rate (i.e. the rate of papers that get rejected after peer review). [GDR SOC2](https://www.gdr-soc.cnrs.fr/) ranks conferences on circuits and systems here: [https://www.gdr-soc.cnrs.fr/conferences/](https://www.gdr-soc.cnrs.fr/conferences/).

A free access ranking system for **journals** is:
- [https://www.scimagojr.com/](https://www.scimagojr.com/)

Journals are ranked there from Q1 (best quarter) to Q4 (last quarter), mostly based on their impact, i.e. on how many people read the articles.

[GDR SOC2](https://www.gdr-soc.cnrs.fr/) ranks journals on circuits and systems here: [https://www.gdr-soc.cnrs.fr/les-revues-tableaux/](https://www.gdr-soc.cnrs.fr/les-revues-tableaux/).

Do not forget that the most important for you is your own opinion on the publication: does it bring you clear, reusable ideas on your topic? Does it open promising questions?

## Writing a publication

### Finding a target journal or conference

The first method to find a target conference or journal is to look where closest state-of-the-art papers have been published. You can also use the french GDR (Groupement de recherche) communities to find the best community to communicate to. 

When choosing a conference, there are 4 criteria to consider:
1- Do your skills and planned work enable you to cover a topic within the scope of the conference?
2- will your presentation interest the specific conference reviewers, and other conference attendees?
3- will presentations of other conference attendees interest you?
4- will this publication count as a peer reviewed one published in proceedings, and what will be its impact?

For all these points, looking to previous proceedings of the conference is crucial.

### Writing method

Writing with the LateX language is now universal. You can use tools such as [Overleaf](https://www.overleaf.com), or setup a git with you own Latex repository (better but takes more time and requires installation). LateX templates are to be found on the websites of conferences and journals.

#### LateX tips

For acronyms, you can use the acronym package:

\usepackage{acronym}

- Examples of acronym definitions:
\newacro{snr}[SNR]{Signal to Noise Ratio}
\newacroplural{poi}[POI]{Points of Interest}

Then you can insert acronyms in text with for instance: \ac{snr}

it automatically decides where to put the long-form definition, i.e. at first use of the acronym. You can force long or short forms with \acl and \acs.

You can use plural with \acp (by defaut plural puts an s at the end, unless you define a specific plural).

#### Inkscape tips

For your figures, I advise to use mostly vector graphics and the open tool Inkscape. Activate the grid and experiment "snap to grid" options to be very precise in your graphics.

### Building the content of the publication

You should write something you would like to read. You should also go from very general knowledge to particular knowledge, for your reader to get the context of your discussion. This is true for the whole document but also for each paragraph.

Given the previous "Reading scientific articles" section here is a proposition of steps, that makes you write the paper in the reverse order it is read:

1. Write your paper "little story"
  - Problem, Postulates, Needs, Competition and Comparison (qualitative or quantitative), Contributions of the paper to meet the needs, Method followed, Expected results
  - Note: competition and comparison require knowledge of the state of the art, so a lot of reading
2. Put the titles of the sections
3. Draw the figures (to illustrate your point)
4. Insert the experimental results (this is, if you already have them)
5. Write the proposal sections (normally it goes fast because you are the expert)
6. Write the state of the art
7. Write the intro
8. Write the abstract and title

Inspiring from the papers you have liked reading is always good.

## Experimenting on system design

While each experiment requires specific thinking, some elements are quite universal:
- you can borrow the concept of "minimum viable product": what is the minimal system that can offer you reliable conclusions?
- you can use the concept of "design of experiments": taking the time to imagine an optimized set of experiments for your demonstration.
- for comparing different solutions, it is good to define "controlled experiments", i.e. experiments between which one parameter varies.



