# on persistent memory

short note about why Mini-Memori exists and what I learned building it.

## the problem

most LLM apps treat memory as either a stuffed prompt or an expensive vector DB. neither feels right for personal/local use. a small SQLite-backed engine with semantic recall is the sweet spot.

## what I tried

- pure keyword: too lossy
- big vector DB: way too heavy for what I needed
- sqlite-vss: just right

## takeaway

memory is mostly retrieval. retrieval is mostly ranking. ranking on small corpora doesn't need millions of vectors and a docker container.

> Mini-Memori is ~600 LOC and runs anywhere SQLite does.
