---
icon: material/package-variant-closed
title: lorem
---

# Tools: lorem

Generate random Latin looking text using Text::Lorem.

`lorem` is a simple command-line wrapper around the "Text::Lorem" module. 
It provides the same three basic methods: Generate "words", generate "sentences", and generate "paragraphs".

See more <https://manpages.ubuntu.com/manpages/noble/man1/lorem.1p.html>.

## Installation

Simply `sudo apt install libtext-lorem-perl`.

## Quick Start

Generate 3 paragraphs of Latin looking text:

```console
% lorem -p 3
Ut accusamus aut repellat nesciunt. Omnis perferendis et deleniti. Qui eum iusto ut. Quae iure nesciunt aliquid debitis exercitationem. Dignissimos in tempora omnis. Aperiam saepe alias labore ad nihil.Voluptatem sed expedita quaerat unde porro. Alias est molestiae ut facilis adipisci aut. Iure dolor qui numquam ut voluptatibus.Quo odit quibusdam animi odio. Nihil animi nesciunt sed. Exercitationem culpa eius debitis est aperiam ad quisquam.
```
Generate 5 Latin looking words:

```console
% lorem -w 5
quiperferendisveritatisfacerevel 
```

Generate a Latin looking sentence:

```console
% lorem -s 1
Impedit natus tempora nostrum facere nisi dicta.
```


