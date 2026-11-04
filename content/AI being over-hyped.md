---
publish: true
created: <% tp.date.now('YYYY-MM-DD HH:mm') %>
modified: 2026-09-04T12:24:00.596Z
published: <% tp.date.now('YYYY-MM-DD HH:mm') %>
category:
  - personal
  - writings
  - ai
date: <% tp.date.now('YYYY-MM-DD HH:mm') %>
reviewed: false
rating:
temporary: true
AI:
country:
  - Tanzania
---

AI is over hoped because,

cannot write more than 5 pages of coherent text. getting to 10s of pages will require exponentially more compute.

it's terrible at iterations. can write a script, has a bug, fix that bug (by rewriting the whole thing), introduces a new bug. goes back and forth between these two states (or eventually reintroduces the first bug ). to some extent it's the same with text. also very hard to fix something once it has been produced.

agenti ai, burns through CPU/GPU time when two lines of code would do it in no time. also, lms are designed to have some degree of randomness in the behavior. if I want consistent outputs, I have to set temperature to zero but the model goes in loops. better python most of the times. It might be a missconception here. LLMs generate the python code that is then ran by the agent.

In summary,
LLM use should be confined to very specific user cases. scripts should be 99% python and basically one LLM function when needed to do stuff like sentiment analysis. Text manipulation is really the only application I see. Things like,

- is the person responding happy or not?
- classify this text as about: floods, costal erosion, changes in heat or rain patterns, etc...

LLMs are effectively better ways to I tract with search engines. i like the way it presents information as digested content.better than a link to a webpage but the content is still often better on a webpage. I just like the fact that it's summarized and reformatted.

it's great for outlines
it's great at fixing text
it's great at extracting text from other text
would be more useful if it had access to all of my documents, including emails. but this is maybe because outlook and mac search functions are both incredibly ineffective. I am not sure we need LLM to fix that. Gmail is 10x better and probably sufficient.

spending billions of USD on this seems excessive.
