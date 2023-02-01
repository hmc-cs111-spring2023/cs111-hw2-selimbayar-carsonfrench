_Fill in each this file with your responses, placing each response after its
corresponding question._

---

**Question**

Pick three quotes from the readings about language design. Good candidates
are:

- Something you agreed with / resonates with your own experience
- Something you disagree with
- Something that is interesting, a new idea or perspective you'd like to remember
- Something you didn't understand

For each quote, describe what it was about the quote that led you pick it.

**Response**

"Obey the principle of least astonishment. Every method should do the least surprising thing it could, given its name" [Bloch, 2006]. 

We chose this quote because we thought it was a good rule to go by for programming in general. We had not heard of this principle before, but it is something that we hope to follow in the future. Naming variables and functions can often see unimportant, but if someone else looks at our code they may be confused. Also, even if we choose names that make sense to us, they may not make sense to others. 

"The existence of a master plan alienates the users" [Steele, 1998].

We found it interesting that master plans are discouraged because how else would the future of the language be controlled. We guess the point is that they shouldn't be controlled, but then why even make a new language in the first place if you don't have a specific vision for its use. We think a master plan can still work for the development of a new language if all of the contributors agree on the fundamental ideas. 

"A thought that seems like a primitive in our minds turns out not to be a primitive in a programming language, and in each new program we must define it once more" [Steele, 1998].

This made us think of our process of learning smaller languages like Coq. Simple things we had taken for granted in the past like addition and subtraction had to be defined. In other languages like Python, we would never have to do anything like that which we prefer.

---

**Question**

How would you know a well-designed language? What are the symptoms? How would
you know a poorly designed language? What are the symptoms?

**Response**

A well-designed language would have just enough features to support the language's intended purpose and not more than that. If there are too many features, then it can be harder for new users to learn and nobody will use the language. However, at the same time you want to have enough features so that it is advanced enough to use for complex tasks. Symptoms of a poorly designed language include people struggling to learn the language. Perl, for example, is a popular programming language but is very difficult to learn. C++ is another language I can think of that is popular but notoriously difficult for newcomers. Symptoms of a well-designed language may be there are a lot of active contributors. That means that the language is at a state where many people find value in it and want to invest in its future, but it isn't so complex that people don't want to learn it. Carson pointed out that good languages should also be hard to misuse. If a programmer is doing something wrong they should be prevented from doing it, so they don't waste their time with broken code. It should also be easy to read and debug. Selim pointed out that good languages should also have proper documentation. It shouldn't take that many outside resources to learn it. However, it is understandable if some new users struggle to learn it. Even Python has courses to learn it, but someone with a basic understanding of programming should be able to pick it up relatively quickly. We both agreed that having an active community is also helpful to introduce new users to the language because they can help with any issues in online forums. 

---

**Question**

How might the themes of _Growing a Language_ relate to ideas from the Fowler reading?

**Response**

Fowler talks about how DSL's should be very simple and therefore easier to learn. This is similar to how Steele's argument that overbuilding a new language will scare away new users because it will be hard to learn. DSL's should be on the extreme end of simplicity though. General purpose languages that are grouping should be a mix between simple and complex. Steele's article explains why DSL's can be important for programming languages. If there is a specific niche use for a general purpose language that someone wants to add more functionality to, then a DSL is the best option because you wouldn't want to subject all the users of the general purpose language to learn them if only a few people are going to use it. DSL's allow programmers to add more advanced features to a language while also keeping the language in general easy to learn for everyone else. The idea of the "cost of building" a DSL could also be applied to any new programming language. If there is no interest in the language then it is probably not worth building. If a language would be useful to programmers, then it will generate a lot of interest and support and be much easier to build, but if nobody is interested it will be very hard to build and then nobody would use it anyway, so it is not worth it. Fowler also talks about how a DSL is "something that's evolving, not finished". This is similar to how a new programming language should be built. It should be designed so that it can be continued on in the future. 

---

**Question**

In what way is an API a language?

**Response**

API stands for application programming interface and it is a set of definitions and protocols to build and integrate application software. In the most basic way, a language is the principal method of communication and APIs are communication mechanisms that allow applications to communicate, so it can be considered a language. Just like how humans communicate with each other speaking in English, French or any other language, computer programs communicate with each other through APIs. It is important to consider who is creating and using the API language. Developers design an API, hence also the language, and others have to learn the API just like learning a new foreign language in order to use it. Users and app developers read the API documentation and learn about the language.
In the readings, we read an article by Joshua Bloch called "How to design a good API and why it matters". In the article, there are many bullet points giving different ideas on how to design a better API. We both had different views in choosing the most significant bullet point in designing an API. Selim thinks that the best point in the article was "Names matter. Strive for intelligibility, consistency, and symmetry. Every API is a little language, and people must learn to read and write it. If you get an API right, code will read like prose." [Bloch, 2006]. Selim believes that the first thing an API should consider is being clear for every user, since learning is like learning a new language, and the namings should be clear. Carson thinks that the most important point was "When in doubt, leave it out. If there is a fundamental theorem of API design, this is it. It applies equally to functionality, classes, methods, and parameters. Every facet of an API should be as small as possible, but no smaller. You can always add things later, but you can't take them away." [Bloch, 2006], as he believes that keeping it smaller to be added later is more essential, as it is impossible to go back and take out something if it is wrong.
---

**Question**

What does the post on grayscale tell us about the process of API design?

**Response**

The post on grayscale by Lea Verou talks about the naming of a function to produce different shades of gray. When using the gray() function, gray(0%) is black, gray(50%) is gray and gray(100%) is white. This probably is very straightforward for many people, but can be confusing sometimes. This is a clear example of why naming matters is the most important factor for Selim in the previous question. Even though gray() can be used for white, black, and (all shades of) gray, people may assume gray(100%) is another shade of gray, hence the other two functions - white(), and black() - that work the same way as gray are key in naming to avoid confusion. There, white(100%) is white, as it "gives the 'full effect' of white" [Verou, 2014], and the same with black. "The idea is that people are familiar thinking that way from grayscale printing." says Verou.
The process of API design in this post is the way of how different functions are named and clearly documented for users and developers to read and understand, and easily use to print different shades of gray. Carson mentioned how important it was in this API that the functions were short and clear, and that if anything were to be added, it could be added later on, but is perfectly functional now.

---

**Question**

The Pavlus article mentions the researchers' comments that people preferred
"natural-language replacements for some of the more abstruse syntax". In other
words, people found it easier to work with code that looks more like a human language (e.g.,
English). Consider the following quote by William R. Cook, one of the creators
of AppleScript:

> The experiment in designing a language that resembled natural languages (English
> and Japanese) was not successful. It was assumed that scripts should be
> presented in “natural language” so that average people could read and write
> them. … In the end the syntactic variations and flexibility did more to confuse
> programmers than to help them out. It is not clear whether it is easier for
> novice users to work with a scripting language that resembles natural language,
> with all its special cases and idiosyncrasies. The main problem is that
> AppleScript only appears to be a natural language: in fact, it is an artificial
> language, like any other programming language. … even small changes to the
> script may introduce subtle syntactic errors that baffle users. It is easy to
> read AppleScript, but quite hard to write it.
> [[Cook 2007, page 1-20]](https://dl.acm.org/citation.cfm?doid=1238844.1238845)

Are these two experiences of natural languages at odds with one another? Would
you choose to include natural language in the design of a DSL? If so, how might
you do so? If not, why not?

**Response**

We both agreed that the two experiences mentioned are not necessarily at odds with one another. Both the researchers' comments and Cook's quotes reflect the challenge of creating a programming language that resembles natural language. Cook mentioned that even though the language appears to be a natural language, it is actually an artificial language that can be confusing for users to write, due to the special cases and idiosyncrasies of the language. Both experiences highlight the difficulties in designing a programming language that effectively balances ease of use and readability with accuracy and consistency. When designing a DSL, we had agreements and disagreements. Carson said that he may include little natural language so that the DSL is understood and used by a larger audience, even beginners, rather than only for people who are experienced in some programming languages. A way that it may be done is, for example, using the natural language when using loops. It may be confusing for someone who doesn't know Java to see a for loop in Java and instantly understand what is going. Using a natural language here can make it much easier for newer people.
Selim said that he would not include natural language in the design of a DSL because he believes it would only make it confusing for the users and developers. He believes that the programming language(s) used in the DSL is a language itself, so mixing it with natural language would be like mixing two languages, which would make it more confusing. Natural language should only be used in docstrings, comments, and documentations so that people who are familiar with the syntax of the used language(s) can easily understand what is going on in the DSL. However, we both agreed that using too much natural language in a DSL would be wrong as it would, like Cook said, "introduce subtle syntactic errors that baffle users."[Cook, 2007].
---
