# Primer contents      [Title](#j-primer)

# J Primer

![](_images/box.jpg)

**Eric Iverson**

Copyright © 1991-2011 Jsoftware Inc. All Rights Reserved.  
Last updated: 2001-3-29  
[www.jsoftware.com](www.jsoftware.com)  

# Start Here

J is a general purpose, high-level programming language. If you are new to J and want to be a J programmer, this is a good place to start. Even if you have considerable programming experience, there is much that is unique to J, and it is worthwhile to at least skim this book before jumping into the deep end.

# Why J
J is a very rich language. You could study and use it for years, and still consider yourself a beginner. This is in sharp contrast to simpler languages like Basic or Java, where months of concerted study and use would make you an expert. The effort required to become an expert J programmer is closer to that required to become an expert C++ programmer.

The good news is that the essence of J is so simple and consistent, that you can quickly learn enough to start solving real and interesting problems.

It is easier to learn enough Basic or Java to solve trivial problems, but it is easier to learn enough J to solve more interesting and challenging problems. And once you have that level of skill under your belt, you are not at the end of the road, but can continue to improve, making yourself a better and more formidable programmer.

J is particularly strong in the mathematical, statistical, and logical analysis of arrays of data. It is a powerful tool in building new and better solutions to old problems and even better at finding solutions where the problem is not already well understood.

As well as being a general purpose programming language, the J system also provides:

- an integrated development environment

- standard libraries, utilities, and packages

- a form designer for your application forms (windows)

- an event-driven graphical user interface to your application

- several methods of interfacing with other programming languages and applications

- rapid application prototyping and development

- royalty-free distribution of run-time versions of your application

If you are interested in programming solutions to challenging data processing problems, then the time you invest in learning J will be well spent.

# Purpose of this book
The J Dictionary is the authoritative and definitive specification of the J language. It can be used to learn J, but the fact that it covers all of the language concisely, yet completely and rigorously, with more emphasis on the complex than the mundane, does scare some of us away.

This online book provides a kinder, gentler start for beginners. This book takes you along a path in easy steps to the point where you can write an application in J. Along the way you will be introduced to all the key ideas in J by seeing them in simplified and specific contexts. At the end, you will be able to write real programs in J, and you will also be comfortable in using the J Dictionary as a reference for your work as a J programmer. The purpose of this online book is to get you up to speed where you can use the J Dictionary in a manner that makes you wonder why you ever bothered with this simple stuff.

You should be able to work your way through this book fairly quickly, and at the end you will be an entry-level J programmer. As such, you will have far more programming power at your fingertips than even the most experienced Basic or Java programmer.


# Your background
This online book assumes that you are familiar with another programming language such as Basic, Java, or C. However, this is not a prerequisite, and you shouldn't have particular problems if J is your first computer language (in fact, congratulations!).

Most things can be done in J much as they are done in other languages, and in several areas a topic is introduced just as it would be introduced in other languages. If you are familiar with other languages this makes it easier to follow how it works in J. In some cases there is a much better J way to solve a problem, and that is also covered.


# How to use this book
The online book is a series of small, bite-size sections that are intended to be read in order from the start to the end. Sections typically depend on most or even all of the previous sections having been read. Jumping around is pointless and likely frustrating.

The book is self-contained and could be read without access to a system. In particular, examples of interactions with the J system show both what you enter and how the system responds. However, it is intended to be read with access to a system and with as much use of a system along with the book as possible. It is strongly recommended that you eventually type in all the examples and play around as much as you can with variations on them.

Sometimes a section uses terms and concepts that aren't defined until later. This requires you to proceed with a soft understanding the first time through that becomes more concrete on a second reading.

This book is probably best read by reading it three times:

- Skim the whole book. Try some examples, but it is better to just plow on and get the big picture.

- The second time read it carefully and try all the examples.

- The third time try your own examples to clarify your understanding and to increase your comfort with the mechanics of actually using the system (instead of just reading about it and following instructions).

# Get started
Double-click the J icon to start J. The session opens with a window labeled n.ijx (for example, 1.ijx).

The ijx window is an execution window. You type J sentences into the ijx window and J executes them when you press enter and displays the result.

Type the following line into the ijx window and press Enter.
```J
   2 + 3
```
The sentence is executed and the result is displayed. Type the following line and press Enter.
```J
   5 - 3
```
Your session should look something like this:
```J
   2 + 3
5
   5 - 3
2
```
Lines you enter are indented three spaces and the J answers start at the margin.

# Experiment
You are encouraged to experiment. Try entering similar lines with different numbers. It is clear that `+` is plus and `-` is minus. Enter lines that use `*` for times and `%` for divide. From using `%` you will pretty quickly see that numbers such as `2.5` can be the result, and that they can also be used as arguments.

Until you have more experience, you might sometimes be surprised or even disconcerted by what you observe. Take things in small steps. Try examples where you are pretty sure you already know the answer, and do the experiment to confirm your understanding. If a result puzzles you too much, don't spend time on it in these early stages.
```J
   3 - 5
_2
```
The `_2`, instead of `-2`, might confuse you. Don't worry, it will be explained in a bit.

Most examples in this book show what you should type, indented by three spaces, and also show the result the system displays. This means that you can read the book in a casual manner, without having to use the system to see results. However, the only way you will really learn is by eventually trying the examples and experimenting with your own. Examples are shown in a fixed-pitch font much as they would appear in the ijx window of your system. A larger font is used in some examples to make it easier for you to read and type the example into the system. This is done where you might mistype something because of being unfamiliar with some of the words, or where a typo could have confusing results.

While experimenting, you frequently want to execute minor variations on sentences you have already tried. There are several shortcuts that make this easier. In the ijx window you can move the cursor to any line in the window and press Enter to recall that line as a new line at the bottom of the window ready for editing. You can recall previous input lines for editing by holding down Shift+Ctrl and pressing the up arrow key until you see the line you want to work with.

The examples in most sections are self-contained, but a later part of a section might depend on steps taken in an earlier part. A few sections depend on steps taken in previous sections, but this should be fairly obvious.

# Standard profile
The examples assume that your system runs the standard profile when it is started. This configures your system and makes some standard utilities available.

Enter `CR` (capital letter `C` followed by capital letter `R`) into the ijx window as a quick check on whether the profile has been run.
```J
   CR
```
If the result is a blank line, then profile has been run and you can skip the rest of this section.

If instead you see:
```J
   CR
|value error
```
you will have to change your system so that the standard profile is run. A normal J install is always configured to run profile.

# Terminology
All programming languages have things in common with the English language. Where the analogy is close, J tends to use English language terms in preference to terms used in math and other programming languages.

You could, as in other languages, say line of code, but in J you tend to say sentence instead. Similarly you could refer to the + function, but you usually say verb.

Some English language terms used in J are: alphabet, word, sentence, verb, noun, adverb, and conjunction.

There are several reasons for this approach. One problem it deals with is the plethora of related, but subtly different, uses of traditional terms in math and numerous programming languages. For example: function, subfunction, operator, program, routine, and subroutine are all used in slightly different ways in different programming languages. Rather than inherit this confusion, J adopts its own terms, and defines them precisely within its context.

Using English terms gives you a good idea of what the general meaning of the term is in J. In addition, using natural language terms encourages and facilitates taking the English statement of a problem and more directly writing the corresponding J sentences.

The use of the J terms is encouraged, but certainly isn't mandatory, and using the term function instead of verb is quite OK.

# Alphabet
The J alphabet is the ASCII alphabet and consists of:
```J
26 lowercase letters (a to z)
26 uppercase letters (A to Z)
0 1 2 3 4 5 6 7 8 9
 = < > _
 + * - %
 ^ $ ~ | 
. : , ;
# ! / \
[ ] { }
" ` @ & ?
( )
'
```
There are a few characters that sometimes cause confusion. The `-` (minus) character is different from the `_` (underbar) character and there are three different quote characters:
```J
'  quote
"  double-quote
`  back-quote
```
If you try an example and type " (a double-quote) instead of '' (two quotes) you will be disappointed that your result is not the same as in the book.

The . (period) is usually called dot.

# Word
A word is a group of characters from the alphabet that has a meaning.
```J
   2.5 + 5
```
The sentence has three words: the number `2.5`, the `+`, and the number `5`.

The rules for forming words from the characters in a sentence are simple, and for now, common sense will suffice in recognizing the words in a sentence. There are some complications that will be dealt with in later sections.

# Sentence
A sentence is a group of words that form a complete instruction. Unlike English sentences, J sentences do not end with a period or other punctuation mark. Instead a J sentence is usually a complete line.

# Verb
In the following sentence `+` is a verb (a word that expresses an action).
```J
   2 + 5
```
# Noun
In the following sentence the numbers 2 and 5 are both nouns.
```J
   2 + 5
```
# Number
The following are numbers: 0 1 2 2.5 12.75 0.5 7e6

Enter these, and other numbers, in simple sentences with the verbs `+ - *` and `%`.
```J
  2 * 12.75
25.5
```
An important rule is that a number does not start with a dot.
```J
  0.5
0.5
   0.5 + 3
3.5
   .5
+-+-+
|.|5|
+-+-+
   .5 + 3
|syntax error
|        .5+3
```
Clearly `.5` is not the same as `0.5`. You don't need to know now what `.5` is yet, but it is important to understand that a number does not start with a dot.

The `_` (underbar) is infinity and is a number.

# Negative number
A negative number is indicated by a `_` (underbar), not a `-` (minus).
```J
   5 + _3
2
   _7
_7 
   _5e_3
_0.005
   5 - 9
_4
```
Leaving out the blank between the `-` and the `9` does not change the meaning.
```J
   5 -9
_4
```
The `-` is always a verb. This simplifies the rules for evaluating sentences as there is no special case for `-` when it is used immediately to the left of a number. But if `-` is always a verb, then another character, the `_` (underbar) is required to spell a negative number.

The `_` is used in spelling numbers, along with the digits, dot, and the e for exponential notation; it indicates a negative number.

Remember: `_` in front of a number is part of the number and indicates that it is negative, and `-` is always a verb and is not part of a number.

The `__` (two underbars) is negative infinity and is a number.

# Primitive
A primitive is a word that is defined by the system. For example, `+` is a primitive. The meaning of a primitive is fixed and cannot be changed.

A primitive is spelled with a graphic character (such as `+`) or with a graphic modified by an inflection (a dot or colon), as in `+.` or `+:` .

A primitive is also spelled by one or more letters followed by a dot or colon. For example, `i.` is a primitive that is called index or index of depending on how it is used.

# Name
Whereas a primitive is a word defined by the system, a name is a word defined by you. The primitive `=.` defines a name.
```J
   v =. 23
```
The sentence can be read as `v` is `23`. The word `=.` is called copula (another good English language term). The name `v` is defined as the number 23 and can be used in other sentences.
```J
   5 + v
28
```
Unlike a primitive, a name can be redefined.
```J
   v =. 45
   5 + v
50
```
The system does not display the result of the sentence when it begins with a copula. A sentence that contains only a name shows a display form of the definition of the name.
```J
   abc =. 123
   abc
123
```
You can give anything a name. For example, you could give a name to the verb `+` .
```J
   plus =. +
   23 plus 45
68
```
The preferred way to read `abc =. def` is: `abc` is `def` or `abc` is defined as `def`. However, borrowing from other computer languages, it is also common to say: `abc` is assigned the value `def` or the value `def` is assigned to `abc`.

# Comment
The primitive `NB.` starts a comment that runs to the end of the line.
```J
   2 + 23   NB. this is a comment and is not executed
25
```

# Error
An error in a sentence is reported and the execution stops.
```J
   123 foo 234
|value error
|   123     foo 234
```
A vertical bar marks the error report. When appropriate, the sentence is displayed with extra spaces marking where the error was detected.

# Ambivalence
Every verb has two definitions: a dyad used when it has both a left and right argument, and a monad used when it has only a right argument. The two definitions are usually related, as in - with a dyad definition of minus and a monad definition of negate.
```J
   5 - 3
2
   - 7
_7
```
The dyad is also referred to as the dyadic case of the verb and the monad is referred to as the monadic case of the verb.

The term ambivalence is used in the chemical sense of both valences to indicate that a verb can react with both a single argument and with two arguments.

Remember: every verb has both a monad and dyad definition.

# Dyad
The dyadic case of a verb is used if the verb has both a left and right argument.

The dyad `%` (divided by) is defined as the left argument divided by the right argument.
```J
   5 % 2
2.5
```

# Monad
The monadic case of a verb is used if the verb has only a right argument.

The monad `%` (reciprocal) is defined as 1 divided by the right argument.
```J
   % 2
0.5
```
The relationship between the monad `%` and dyad `%` where the monad is the dyad with a fixed left argument is quite common, and you will see this in a number of the other primitive verbs.

# Vocabulary
The J Dictionary (menu Help|Dictionary) is the J reference book and is your ultimate, authoritative source of information on J. The sooner you become familiar with using it the better, and a good way to start is by looking up the primitives that have been introduced so far.

Press F1 to show the vocabulary and click a primitive to jump to the entry. If you press F1 while holding down Ctrl you get context sensitive help. If the caret is at a `+`, pressing Ctrl+F1 will jump to the `+` entry.

In the vocabulary take a look at the row for `+`, which is the fifth row. The first entry in this row contains: `+` Conjugate `o` Plus. The word `+` is a verb and its monad is called conjugate, and its dyad is called plus. The dyad `+` is plus as defined in arithmetic.

The monad `+` is interesting. In math, the conjugate of a complex number is the number with the same real part and an imaginary part of opposite sign. On real numbers the conjugate has no effect and the result is the argument, and on complex numbers it changes the sign of the imaginary part. J supports complex numbers just as directly as integers or real numbers. A complex number is indicated by a j separating the real and imaginary parts.
```J
   int =. 23
   + int
23
   float =. 23.5
   + float
23.5
   imagine =. 2j3    NB. 2 real part, 3 imaginary part
   + imagine	     NB. change sign of imaginary part
2j_3
```
Many primitives support complex numbers and the J Dictionary must document this, which means there is a bit of extra complexity in some of the descriptions. If you need complex numbers in your application this is fantastic. But if you are a beginner and are not concerned with complex numbers, then you have to know enough to be able to ignore these bits and not get distracted or confused.

Let's look at the `+` Dictionary page. The header line of the page gives the monad name Conjugate on the left side, and the dyad name Plus on the right. The formal name of the primitive `+` is near the center. The `0 0 0` to the right of the `+` will be explained later.

Below this header are two boxes. The left box has the monad definition and the right box has the dyad definition. The page then continues with general discussion and examples.

The J Dictionary is a concise, rigorous, and complete reference suitable for the most experienced users. This can make it difficult for beginners who don't know what to expect. For example, in the general discussion and examples for `+` there is considerable discussion of complex numbers and not a single example of just adding a couple of integers. Great for the experienced user who would be insulted if told how to add integers, but a bit of a reading challenge for the real beginner. You have to learn how to tune out, for now, the bits that are too advanced or are not relevant to your current interest, and concentrate on the parts that are.

Go to the vocabulary page and take a look at the `+.` entry (fifth row, second entry) which contains: `+.` Real/Imaginary o GCD (Or). There is a lot of information here, and again much of it is not relevant at this early stage. Let's look at the definition.

Glance at the left box for the monad definition and notice that it is for complex numbers. File it for future reference, but give it a pass for now.

The dyad case in the header is described as: GCD (Or). This gives two informal names, GCD and Or, and indicates it can be used in two different ways. The dyad definition is in the right box. Note that GCD stands for greatest common divisor (which should at least ring a bell of math memories). Further on in the definition you will find that if the arguments are boolean then the `+.` is the logical or function. The GCD is a useful extension of the domain of the or function to non-boolean arguments. This extension of the domain of primitives is common in J. For now, it is interesting to note that `+.` has this larger domain, but it is also easy to limit it to boolean arguments.
```J
   0 +. 0	NB. 0 or 0
0
   0 +. 1
1
   1 +. 0
1
   1 +. 1
1
```
The vocabulary page entry for `+:` contains: Double o Not-Or. The definition page gives quite simple definitions for both the monad and dyad.

The monadic case is called double and does just what you'd expect.
```J
   +:  3
6
```
The dyadic case is the logical negation of the or of the arguments.

Again, for both `+.` and `+:` much of the general discussion and examples are perhaps beyond your capabilities right now. But the key is to know how to navigate and to get the information that is relevant.

After the row for `?` there are additional rows for primitives that are spelled with names that are inflected with a dot or colon.

# Checkpoint A
At this point you should understand:

  - how to use the J Dictionary vocabulary
  - terms such as word, sentence, noun, verb, ambivalence, dyad, monad
Check your understanding by doing the following exercises:
  - look up the definition of the monads `+: *: -: %:`
  - experiment with these new monads
