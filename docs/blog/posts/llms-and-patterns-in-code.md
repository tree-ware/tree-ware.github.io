---
date:
  created: 2026-02-22
authors:
  - deepak-nulu
categories:
- LLMs
---

# LLMs and Patterns in Code

Why are LLMs so good at generating code? It is because code tends to be structured and follows certain patterns.
LLMs are able to learn those patterns and generate code that conforms to those patterns.

But are patterns in your code a good thing?

<!-- more -->

Here is what [Paul Graham][1] said about patterns in code in his [Revenge of the Nerds][2]
essay:

> For example, in the OO world you hear a good deal about "patterns". I wonder if these patterns are not sometimes
evidence of case (c), the human compiler, at work. When I see patterns in my programs, I consider it a sign of
trouble. The shape of a program should reflect only the problem it needs to solve. Any other regularity in the
code is a sign, to me at least, that I'm using abstractions that aren't powerful enough-- often that I'm
generating by hand the expansions of some macro that I need to write.

and:

> [Peter Norvig][3] found that 16 of the 23 patterns in Design Patterns were "[invisible or simpler][4]" in Lisp.

You may be thinking, "what is the big deal? Instead of a macro, the LLM is generating the code." But would you think the
same about functions? Would you be okay with an LLM generating code inline instead of creating and using a function?

There are two problems with using LLMs to generate code. The first is that you can't trust the LLM, and so you need to
review all the code it generates. The more an LLM generates, the more there is for you to review. The second problem is
that when you ask the LLM to modify your code later on, it needs to read in a lot more code, unnecessarily filling up
its context window.

If there is an abstraction, then you can generate code deterministically and trust it without having to review it.
Even if LLMs become trustworthy in the future, why pay for an LLM when you can use a simpler and cheaper deterministinc
approach? For example, would you use an LLM instead of the protobuf compiler `protoc` to generate classes from a
`.proto` file? It makes sense to use an LLM to create the `.proto` file, but not to generate classes from it.

People are able to generate entire frontends and backends using LLMs these days. The non-functional aspects are similar
in all such systems. So LLMs are able to generate such systems. Is there an abstraction that can do the same? The answer
is yes! And ironically, it does _**not**_ generate code! Instead, it uses abstract-algebra to carry out the
non-functional aspects of the system.

It is called [Tree-Ware][5]. It is an open-source, end-to-end framework written in [Kotlin][6]. There is still a lot
to be built, so contributions are most welcome! And one last bit of irony: you can use LLMs to build it 🙂

[1]: https://paulgraham.com/bio.html
[2]: https://paulgraham.com/icad.html
[3]: https://norvig.com
[4]: http://www.norvig.com/design-patterns/
[5]: https://www.tree-ware.org
[6]: https://kotlinlang.org