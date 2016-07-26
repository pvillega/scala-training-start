# Scala Training: Start!

This repository is basically this document. The idea is to create a list of links and tasks that can help junior developers to learn Scala and to understand why they should learn Scala.

To use it, just keep reading ;)

## Why Scala?

Let's start with the obvious: why should you spend valuable time and effort to learn Scala? 

There are plenty of articles around that explain why learning Scala is a good idea:

* https://www.lightbend.com/blog/why-scala
* http://www.cakesolutions.net/teamblogs/why-scala
* https://www.toptal.com/scala/why-should-i-learn-scala

As you may have noticed, I am cherrypicking and ignoring articles that argue you shouldn't learn it ;) 

Based on personal experience, I'd recommend you learning Scala as a gateway to advanced programming. Some people will say you should jump into [Haskell](http://haskellbook.com/), or [Idris](http://www.idris-lang.org/), or [Clojure](https://clojure.org/), and grab the power they offer. And they are right... in some circumstances.

But if you are reading this, you are most likely searching for a different approach. You can start using Scala as a *cleaner Java* and, once you are more experienced, you can introduce more advanced concepts to your code via libraries like [Cats](http://typelevel.org/cats/).

So I guess the real question is **Why should you I those advanced concepts?* After all Facebook was built using *PHP*... 

Yes, why?

Let me give you a very simple example:

In Object-Oriented programming you use [Design Patterns](https://en.wikipedia.org/wiki/Software_design_pattern) to do some tasks. There is a design pattern called [Strategy](https://en.wikipedia.org/wiki/Strategy_pattern) in which you decide how to do some operation at runtime, instead of at compile time. You achieve that by creating an interface and a few subclasses that implement the different behaviours. As you can see from the [example in Wikipedia](https://en.wikipedia.org/wiki/Strategy_pattern#Java), it's quite a verbose solution.

In functional programming implementing this is much simpler, given functions are [first class citizens](https://en.wikipedia.org/wiki/First-class_function). This means you can pass the function itself as a parameter, no need to use interfaces, or classes, or other helpers to encapsulate it. 

Be aware that it's not just a matter of code verbosity, but of code quality too. The less code you write, the less bugs you will have in your code. Sounds obvious, but sometimes we forget this! Also, the functional approach can be tested in a simpler and more direct way, making your unit tests simpler (you may never use mocking frameworks in a functional approach). And adding new strategies is also a much easier task.

And we are talking here about basic designs and concepts of functional programming, so imagine what may happen when you learn concepts like [Monad](http://typelevel.org/cats/tut/monad.html). You probably won't go back to object-oriented languages.

Now, I won't lie: some of the advanced stuff is not easy, and it requires time to understand it correctly. But learning Scala is not hard, and you don't need to learn the advanced stuff until you want to. When you do so, it will open the door to a new way of developing software. And the good news are that the advanced concepts you will learn are fully transferable to other functional languages: a [Functor](http://typelevel.org/cats/tut/functor.html) is a Functor, both in Scala and in Haskell. So the effort is worth it, trust me. 

There is also a more practical reason: you are reading this because you have, or may be considering, a career in software development. Things change, but right now it seems the next years (decades) may become dominated by languages that are functional at their core. Scala, F#, Elm, Elixir... there's a long list. As I said in the paragraph above, the functional concepts, once learned, are transferable between languages. The same that inheritance is the same idea in Java, C++, or C#. So it may be a good idea, for your own professional projection, to start learning functional languages. Why not start with Scala, which makes it easy to transition?

## Requirements

Still around? I'll assume you want to learn a bit more. Before we start giving you links and resources, there's some stuff you may want to do.

If you are reading this I assume you know what [Github](https://github.com/) is. If you don't have an account with it, please create one. Github's BootCamp can help you [install Git](https://help.github.com/articles/set-up-git/) and [create your first repo](https://help.github.com/articles/create-a-repo/). You may also decide to [fork this repo](https://help.github.com/articles/fork-a-repo/) for your own reference.

Once you have your Github account, it is recommended to join [Gitter](https://gitter.im/). Gitter is web-based (with a desktop client you may use if you prefer so) and provides chat channels linked to Github repositories. You may find these channels very useful when having doubts regarding some Scala concepts, or if you need help with a library. I recommend joining the [Typelevel Scala Gitter Channel](https://gitter.im/typelevel/scala) to start with.

The exercises and guides you can use to start are all available online, so you only need your browser. At some point you will need to install [Scala](http://www.scala-lang.org/download/) in your computer, but don't worry about it right now.  

Familiarity with programming in some language is not required, but it may help. Ideally, you should follow this guide with someone that can provide guidance nearby. For the first parts, though, this is not necessary.

## Starting

There's plenty of good and free material out there to learn Scala. I recommend the StackOverflow [tag info for Scala](http://stackoverflow.com/tags/scala/info) as a starting point. Be aware some of the sources linked in there may point to older versions of the language, but they are good enough to start learning the basics.

From the [link](http://stackoverflow.com/tags/scala/info) above I recommend [Scala By Example](http://www.scala-lang.org/docu/files/ScalaByExample.pdf) as a reference for Scala syntax, as it's free and concise.

You should also check the links of the [*Scala Tutorial*](http://stackoverflow.com/tags/scala/info) section, including [What's so great about Scala?](http://stackoverflow.com/questions/727078/whats-so-great-about-scala) and [Difference between var and val](http://stackoverflow.com/questions/1791408/what-is-the-difference-between-a-var-and-val-definition-in-scala). Then keep checking the other links about the language, as needed.

The (at this point) new StackOverflow Documentation site has a [Scala](http://stackoverflow.com/documentation/scala) tag, in which you can see examples for several language concepts. 


## Basic exercises

Once we have the language reference at hand, nothing better than coding a bit with Scala. I recommend using [Scala Exercises](https://www.scala-exercises.org/), specifically the module for [Scala STD Lib](https://www.scala-exercises.org/std_lib/asserts). 

This will introduce you to Scala syntax and concepts, step by step. You don't need anything besides a browser, which means you can start right away, with the help of [Stack Overflow's resources](http://stackoverflow.com/tags/scala/info).


## Reinforcing concepts

Once you have completed the sections above, I recommend getting a copy of [Creative Scala](http://underscore.io/books/creative-scala/). It is designed to give you a fun introduction to functional programming using Scala, and it requires no previous knowledge of Scala nor of functional programming.

As you will have completed the exercises from the previous sections, the syntax and some basic concepts should not be an issue anymore, which will help you focus on the functional programming aspect of the book. 


## Using the skills you acquired

There is a website, [Exercism.io](http://exercism.io/), that provides a set of *katas*, or exercises, to practice your language skills. They have a [Scala track](http://exercism.io/languages/scala) with several exercises (more than 60!), with increasing difficulty. Once submitted, you can compare you answers with the answers of other participants, as well as comment on the answer of other people to understand why they did something in a specific way.

Exercism also provides instructions on [how to install Scala](http://exercism.io/languages/scala) or [run the tests](http://exercism.io/languages/scala), as well as a list of [resources to learn Scala](http://exercism.io/languages/scala).


## I need more!

Ok, we have more! [Cyber Dojo](http://cyber-dojo.org/) is a website in which you can create practice sessions to learn a language with other people, or on your own if you are so inclined. Create a Scala session in the site, and you will see several exercises you can solve. Their are, in average, more complex than those in Exercism.

If you solve them, there's a site that provides [Scala Koans](http://scalakoans.webfactional.com/installation). It's something similar to Exercism, but with different exercises and a different way of interacting with it.


## What next?

If you have completed everything up to here, you have accumulated quite the knowledge about Scala. Congratulation! Did you enjoy it? I hope so.

You may be wondering what can you do next to learn more and build upon these foundations. Here I have some suggestions that may help you:

* Join the [London Scala User Group](http://www.meetup.com/london-scala/). They have plenty of meetups, including coding dojos where you can learn more about Scala from people using it daily.
* Come to Hack The Tower. This is a monthly event (one Saturday, once per month), organised by Typelevel and the London Scala User Group. It's basically a hack day where people form groups to learn and code together. If you are member of the London Scala User Group you will get notifications about it, and there is a [Gitter channel](https://gitter.im/typelevel/hack-the-tower) where you can get more information.
* I recommend [Underscore books and courses](http://underscore.io/books/), which cover a wide range of Scala-related topics, for beginners and more experienced people. Full disclaimer: I know them and I work with some of the members, but I get nothing from this reference. Word.
* There's a site with a [list of programming katas](http://codekata.com/) you can try to solve with Scala, for practice. I'm afraid they don't provide the answers, but at this stage that is probably not an issue ;)


And that's all for today. I hope this has helped introducing you to the fascinating world of Scala. Remember to use Gitter and the meetups to explore more about Scala, and to find new ideas on how to get more experience with Scala and functional programming.

Cheers!