# DOC2QUERY

Transform document content into a set of questions using the T5 model.

## Table of Contents
- [Setup](#setup)
- [Generating Questions for GitHub Content Pages](#generating-questions-for-github-content-pages)
- [Reading GitHub Links](#reading-github-links)
- [Generating Questions for Headers](#generating-questions-for-headers)
- [Sample Questions](#sample-questions)

## Setup

Add the links for which you want to generate questions to the list below and set the number of questions to generate per document:

```python
topic_links = [
    "https://github.com/javascript-tutorial/en.javascript.info/blob/master/3-frames-and-windows/01-popup-windows/article.md",
    ...
]
num_questions_per_link = 30
```

## Generating Questions for GitHub Content Pages

- Download the content from a link.
- Parse the content by their headers.
- Go header by header and generate questions for it.
- Write the questions into a JSON format.

## Reading GitHub Links

Functions for reading and parsing Markdown content from GitHub.

## Generating Questions for Headers

Using the `doc2query/msmarco-t5-base-v1` model to generate questions based on header content.

## Sample Questions

Examples of generated questions can be found in the `test.json` file.

---

**Note**: This notebook requires the `transformers` and `sentence-transformers` packages to be installed.
```
