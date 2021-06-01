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

# Numeric constant
You have seen the use of single numbers. It is also possible to have a list of numbers.
```J
   num =. 5
   nums =. 23 0.5 12.5 7e6 _12 7
```
You'll do lots more with numeric lists, but for now we just want to establish that there is such a thing.

# String
Characters bracketed by quotes create a string.
```J
   char =. 'Q'
   chars =. 'this is a list of characters' 
```
The quotes are not displayed when the string is displayed.
```J
   char
Q
   chars
this is a list of characters
```
The quote starts and ends a string. A pair of quotes indicates that the quote character itself is in the string.
```J
   'put 2 ''s to get 1 '' in the string'
put 2 's to get 1 ' in the string
```
An unmatched quote is an error.
```J
   abc =. 'asdf
|open quote
|   abc =. 'asdf
|          ^
```
A string can be empty.
```J
   abc =. ''
   ```
A string is also referred to as a literal constant or as a character constant.

# Word formation
The monad `;:` can be useful in figuring out what the words are in a sentence. The word formation primitive takes a string as its right argument, splits it into words, and returns a result with each word in a box. For now, don't worry about what the boxes are, just note how visually helpful they are. You'll learn about boxes in later sections.
```J
   ;: '2 + 3'
+-----+
|2|+|3|
+-----+
   ;: '2.5 + 3e4'
+---+-+---+
|2.5|+|3e4|
+---+-+---+
   ;: 'a =. 1 2 3'
+-+--+-----+
|a|=.|1 2 3|
+-+--+-----+
   ;: 'test + 123 NB. this is a comment'
+----+-+---+---------------------+
|test|+|123|NB. this is a comment|
+----+-+---+---------------------+
   ;: 'def =. ''testing 1 2 3'''
+---+--+---------------+
|def|=.|'testing 1 2 3'|
+---+--+---------------+
```
Note that the following are all J words and each goes in its own box:
```J
2.5
3e4
=.
1 2 3
test
NB. this is a comment
'testing 1 2 3'
```
It might surprise you that constants such as `1 2 3` and `'testing 1 2 3'` are J words. This is an important point and understanding it is necessary in reading and writing J sentences.

If you are ever puzzled by a J sentence (it could happen), one of the things you can do is apply `;:` to it to be sure you know the words. You can then worry about the meanings of those words.

Look up `;:` in the J Dictionary. The informal name for `;:` is word formation.

# Space
Spaces are not required to separate primitives from other words. On the other hand extra spaces don't change the meaning.
```J
   2+3
5
   2 + 3
5
   2    +    3
5
```
Most examples in this book have spaces around all primitives. This makes the individual words stand out and allows you to concentrate on the meaning of the words without the additional problem of first figuring out what the words are.

However, most J programmers, as they become more experienced, reach a point where they can easily read the words in a sentence, and the extra spaces become a nuisance and hindrance to understanding, rather than an aid. You will notice that in some of the later examples that some of these unnecessary spaces are left out.

There are some cases where a space is essential.

A space must separate names.
```J
   a=.3
   plus=.+
   a plus a
6
   aplusa
|value error
```
The `.` (dot) and `:` (colon), used as inflections, change the word immediately in front of them into a new word. When used as a primitive or as the start of a primitive, they must have a space in front so that they are not treated as an inflection.
```J
   ;: 'a . b'	NB. 3 words
+-+-+-+
|a|.|b|
+-+-+-+
   ;: 'a .b'	NB. same 3 words
+-+-+-+
|a|.|b|
+-+-+-+
   ;: 'a. b'	NB. 2 words
+--+-+
|a.|b|
+--+-+
```
A space must separate a `.` or `:` , that is not being used as an inflection, from the previous word.

Numbers, for example 1e7, can contain letters. There are in fact several letters that can be used in spelling numbers in J. Letters that immediately follow a number are treated as part of the spelling of the number.
```J
   plus =. +
   1plus 3
|ill-formed number
   1 plus 3
4
```
A space must separate a number from a letter that is not a part of the number.

# Precedence
Math traditionally gives multiplication precedence over addition. In math class (or a skill testing question from a cereal box contest), if you were asked what 2 + 3 * 4 was, you would know the answer was 14.

This is not too confusing if there are only a few functions and only a few levels of precedence (division | multiplication | addition and subtraction). But it gets awkward in languages such as C which have many functions and many levels of precedence.

With the large number of verbs in J it would have been difficult to define the precedence, let alone trying to remember it when reading or writing. Moreover, being able to name things means you would also have to figure out what to do with the sentence:
```J
   2 plus 3 times 4
```
In a break with traditional math and in contrast to most other programming languages, J has no verb precedence. It will take you a little while to stop doing the multiplication first, but the overall simplification is worthwhile.

Remember: there is no verb precedence.

# Parentheses
Math and most programming languages, including J, use parentheses to control the evaluation of a sentence. If a sentence is fully parenthesized then the order of evaluation is identical in most languages and is independent of verb precedence or any other rules.
```J
      2 + (3 * 4)
14
   (2 + 3) * 4
20
   10 - (4 - 3)
9
   (10 - 4) - 3
3
```
There isn't any confusion about these answers.

# Order of evaluation
What is the answer if the parentheses are left out?
```J
   10 - 4 - 3
9
```
J evaluates the sentence as:
```J
   10 - (4 - 3)
9
```
Most other languages would evaluate it as:
```J
   (10 - 4) - 3
3
```
In the absence of parentheses, J implicitly provides them from the right towards the left. Other languages provide them from the left towards the right. A longer sentence will make this visually clearer.
```J
   10 - 4 - 3 - 1
8
   10 - (4 - (3 - 1))	NB. J right-to-left
8
   ((10 - 4) - 3) - 1	NB. others left-to-right
2
```
Now consider a sequence of monadic verbs.
```J
   - - - 4
_4
```
Everyone knows how to parenthesize this, and every language does it the same.
```J
   - (- (- 4))
_4
```
The grouping is done right-to-left and in this case the other languages agree with J. J always parenthesizes from right-to-left, whereas other languages have different rules for different situations.

J has a right-to-left order of evaluation. Most other languages have a left-to-right order of evaluation for dyads, right-to-left for monads; and this is modified by the relative precedence of the verbs involved.

With nouns and verbs the J evaluation rule from J Dictionary section E is:
Execution proceeds from right to left, except that when a right parenthesis is encountered, the segment enclosed by it and its matching left parenthesis is executed, and its result replaces the entire segment and its enclosing parentheses.
There are things in J, other than nouns and verbs, that you have not yet met that complicate this rule by adding a few more. It is these additional classes that largely justify the J break with tradition and adoption of a right-to-left evaluation.To further quote from the J Dictionary section E:
One important consequence of these rules is that in an unparenthesized expression the right argument of any verb is the result of the entire phrase to its right.
This is due to the lack of verb precedence as well as right-to-left evaluation.

No verb precedence, right-to-left evaluation, and the rules for the other classes make the overall evaluation rules simple, reduce the need for parentheses, and make sentences easier for an experienced J user to read and write.

Read the following sentences, evaluate them in your head, and understand how the no precedence and right-to-left rules explain the answer.
```J
    2 * 4 + 5
18
   2 + 4 * 5
22
   2 - 4 - 5
3
   8 % 2 + 2
2
```
Remember: no verb precedence and right-to-left evaluation.

# Verb definition
The art of programming lies not so much in using the primitives, as in defining your own verbs, tailored to your requirements. In defining your own verbs you are extending the language to build an application that solves a particular set of problems.

Let's assume that the problem is to convert temperatures between Fahrenheit and centigrade. You need to define a verb that does that.

The following is a definition of the verb centigrade that will convert its argument from a Fahrenheit value to a centigrade value.
```J
   centigrade =. 3 : 0
t1 =. y - 32
t2 =. t1 * 5
t3 =. t2 % 9
)
```
At this point you want to do something that works, rather than deal with problems arising from typos, so transcribe it carefully.

In the ijx window enter the first line:
```J
   centigrade =. 3 : 0
```
Type it exactly as shown. There must be a blank between the 3 and the : . The 3 indicates that you are defining a verb and the 0 indicates that the definition is in the subsequent input lines.

After you enter the above line the caret is at the left margin and has not been indented the three spaces as it normally is. This indicates that the system is waiting for you to enter the rest of the definition.

Type in the lines following the definition of centigrade as shown. They are at the left margin, and so look like they might have been displayed by the system, but in fact they are your entries of the lines required to define the verb.

The final line that contains just the ) ends this special definition input mode. After you enter this final line, the system again indents the three spaces indicating that it is ready to execute a sentence.

If you entered the definition correctly, you should be able to experiment with your new verb.
```J
   centigrade 32	
0
   centigrade _40
_40
   centigrade 212
100
```
Let's look at the definition to understand how it works. The y in the first sentence of the definition is the name of the argument of the verb. When you execute the verb with an argument the first line will subtract 32 from the argument and define t1. When the first line is finished, execution proceeds to the next line, which defines t2 as the result of t1 times 5. Execution proceeds to the next line and defines t3 as t2 divided by 9. There are no more lines, so the execution of the verb is finished. The result of the verb is the last result that was evaluated.

We used `3 : 0` to define the verb. The phrase verb define is equivalent and some find it easier to read. However, it hides information and we will use the `3 : 0` form.
```J
   centrigrade =. verb define
. . .
)
```

# Monad and dyad definition
As discussed in the earlier section on ambivalence, all verbs had two definitions, a monad and a dyad. You have defined only a monad for centigrade. What about the dyad?
```J
   23 centigrade 32
|domain error
|   23     centigrade 32
```
Since you didn't provide a dyad definition, it is empty and this is treated as if the dyad had no arguments in its domain, and any arguments you give will cause a domain error.

Let's examine some simple examples of defining dyadic, monadic, and both cases.
```J
   monadminus =. 3 : 0
- y
)
   monadminus 5
_5
   5 monadminus 3
|domain error
|   5     monadminus 3
```
The above defines the monad of the verb named monadminus. Applying it monadically works and applying it dyadically fails.

In one-line definitions like this you can take a shortcut and make the definition on a single line and avoid entering the special input mode that needs to be ended with the `)`. The following is an equivalent way of doing the above definition:
```J
   monadminus =. 3 : '- y'
```
The string contains the single line that makes up the definition. It is provided directly as the right argument of : instead of the 0 used earlier.

So far you have defined just the monadic case of a verb. You can also define a verb with just a dyadic definition. Instead of 3 as the left argument to `:` use a 4 to define the dyadic case.
```J
   dyadminus =. 4 : 'x - y'
   5 dyadminus 3
2
   dyadminus 5
|domain error
|       dyadminus 5
```
In the monad case the `y` name is the right argument and in the dyad case x is the left argument and `y` is the right.

What if you want to define both cases of a verb?
```J
   minus =. 3 : 0
- y
:
x - y
)
```
The `:` by itself on a line separates the monad and dyad definitions.
```J
   3 minus 5
_2
   5 minus 3
2
   minus 5
_5
```

# Script file
When you close J you lose the definitions of all the names. What you execute in the ijx window affects the current session, but is not permanent. This is fine when experimenting, but when you start defining things like your centigrade verb you want to record the definition so that you can use it in another session.

Close J and restart it.
```J
   centigrade
|value error
```
You have a clean slate. The definition of centigrade, and all the other names you defined, in the previous session are lost.

At least the primitives are still there!
```J
   2 + 5
7
```
As you would expect, to maintain a permanent record of your definitions, you save them in files. Files with J sentences and definitions are called script files and you can edit them just as you would edit any other text file. Script files typically have a suffix of .ijs.

Remember: a script file is a source file for definitions.

Although you can use any text editor to work with script files, the J system provides a simple editor that is integrated in ways that make it convenient.

The **File|New ijs** menu command creates a new script file and a window for editing it. Do this now and you will see that your J session has both an ijx window and a new ijs window.

The ijs window is an edit window on the file with the name in its titlebar. Enter in an ijs window does not execute the line, it just moves to the start of a new line.

Type your centigrade definition into the ijs window.
```J
centigrade =: 3 : 0
t1 =. y - 32
t2 =. t1 * 5
t3 =. t2 % 9
)
```
**Be sure to use `=:` instead of `=.` in the first line**. The `=:` makes a global definition. If you use `=.` it is a local definition. This important difference is explained shortly.

So far you have just edited changes into the window. The file has not been changed and the verb is still not defined. You have to run the script in order to execute the sentences.

Do menu command **Run|Window** in the ijs window to save the changes to the file and then execute each of the sentences in the file. This is similar to your typing the contents of the file into the ijx window, except the sentences and results are not displayed. The only display in the ijx window is the system generated sentence that causes the file sentences to be executed. This sentence will be something like:
```J
   load'c:\j601\temp\1.ijs'
```
If an error is reported (output in the ijx window with a vertical bar on the left) then you have a typo in your script. Correct the text in the ijs window and run it again.

The sentences in the script file have been executed and centigrade is now defined. In the ijx window try using centigrade.
```J
   centigrade 32
0
```
The file created with **File|New** ijs is in the J temp directory and has a temporary format name (a number with an ijs suffix). If you close J now, it will ask if you want to delete that temporary file. If you replied no, you could restart and open that temporary file and run it to define centigrade. However, it would be better to resave it now with a more appropriate name in the J user directory. Use **File|Save As...**, go up one directory level and then to the the user directory, and set the file name as cf.ijs. The file name in the ijs window titlebar will change to the new name.

Close the cf.ijs window and erase your centigrade definition. You erase the definition of a name by using the utility verb erase with an argument that is the string of the name you want to erase. The result of 1 indicates the erase was successful.
```J
   erase 'centigrade'
1
   centigrade 212
|value error
|       centigrade 212
```
Use **File|Open** to open the cf.ijs window and use **Run|Window** to run the script to define centigrade.
```J
   centigrade 212
100
```
Let's add a definition for fahrenheit to the cf.ijs window. Type in the following after your centigrade definition. Again, be sure to use `=:` .
```J
fahrenheit =: 3 : 0
t1 =. y * 9
t2 =. t1 % 5
t3 =. t2 + 32
)
```
Use **Run|Window** to run the sentences in the cf.ijs script. Because these are the first changes to a permanent (non-temporary) file you are prompted to see if you want to save the changes to file. Reply yes, and then test your new verb.
```J
   fahrenheit 0
32
   fahrenheit 451
843.8
```
Close J and restart it.
```J
   centigrade
|value error
   fahrenheit
|value error
```
You can run the sentences in the cf.ijs file without opening the file for editing. Use **Run|File** and select your cf.ijs file. A line similar to
```J
   load'c:\j601\user\cf.ijs'
```
appears in the ijx window to run the sentences in the file and your verbs are now defined.
```J
   centigrade 32
0
   fahrenheit 100
212
```
The line that starts with load that appears in the ijx window is in fact the sentence that causes the sentences in the file to be executed. The menu command is just a short cut way of executing this sentence. The string is the full path name to the file to run. You can shorten this full path name to a relative path name when you type it manually.

To check this, close J, restart it, and verify that centigrade is undefined. In the ijx window execute the following sentence.
```J
   load'user\cf.ijs'
```
Now check that your verbs are defined.

Use **File|Open** to open your cf.ijs file for editing.

What if there is an error in the script? Let's add an intentional error to the script to see what happens. Add the line `foo 123` at the end of the script and run the script again.
```J
   load'c:\j601\user\cf.ijs'
|value error
|       foo 123
|[-13]
```
An error is reported and the execution of the sentences in the script stops. The number at the end of the error report is the line number in the script that had the error.

Remove the error from the script and run it again.

# Local
The verb centigrade uses names `t1`, `t2`, and `t3` in its definition, but if you refer to them outside the verb they are not defined.
```J
   centigrade 32
0
   t1
|value error
   t1 =. 123
   t1
123
   centigrade 212
100
   t1
123
```
The use of `t1` inside the definition of centigrade has not conflicted with your use of `t1` outside the definition. The verb centigrade does not define a `t1` outside of itself, as indicated by the value error, and setting a value into its `t1` does not change the value of `t1` outside the definition.

The `t1` used inside centigrade is a local name. A local name exists only inside the verb. The `t1` used outside centigrade is a global name. A name defined in the execution of a verb with the copula `=.` is a local name.

# Global
A name defined outside the execution of a verb is a global name.

In the previous section, the `t1` defined in the ijx window is a global name that is completely different from the `t1` defined inside the verb centigrade.

Let's try some experiments. Create a temporary script file with **File|New ijs** and type into it the definition:
```J
fooa =: 3 : 0   NB. =: is important
zzz + y
)
```
Run the script with **Run|Window**. In the ijx window:
```J
   fooa 5
|value error
|       zzz+y
```
Let's define the global `zzz` to see what happens. Defining it outside a verb means it is a global. In the ijx window:
```J
   zzz =. 23	NB. define global zzz
   fooa 5
28
```
The verb fooa uses the global `zzz`. So, a verb can use globals.

Edit the script to add foob and then run the script.
```J
foob =: 3 : 0
zzz =. 7
zzz + y
)
```
In the ijx window:
```J
   foob 3
10
   zzz
23
```
The verb foob uses its local `zzz` and ignores the global. So, a verb can use locals and ignore globals of the same name.

Inside a verb the copula `=.` defines a local name. Once a name is defined as a local, references to that name are to the local name.

What if you wanted to define a global name? The global copula `=:` (`=` with a colon inflection) defines a global name. Edit the script to add fooc and then run the script.
```J
fooc =: 3 : 0
gw =: y
lz =. y
)
```
In the ijx window:
```J
   fooc 3
3
   gw
3
   lz
|value error
   gw =. 24
   fooc 5
5
   gw
5
```
Defining gw with `=:` defines the global name.

In general, it is good practice to only define locals in a verb and to not define globals. This is an important part of what is sometimes called a functional style of programming. Verbs that define globals are said to have side effects and are more likely to cause bugs and make it harder to read the application to understand what is happening.

It is possible to define a verb that uses both the global and local definitions of a name and this is VERY bad practice.

# Debug global
Sometimes when trying to debug or better understand a verb it is useful to see the values of its local names or other intermediate results. A quick way of doing this is to add a line to the verb definition that does a global definition.

Open the cf.ijs file and add a line to centigrade to define global `gt1` as `t1`.
```J
centigrade =: 3 : 0   NB. =:
t1 =. y - 32
gt1 =: t1             NB. temp line for debugging info
t2 =. t1 * 5
t3 =. t2 % 9
)
```
Run the script and in the ijx window:
```J
   centigrade 124
51.1111
   t1
|value error
   gt1
92
```
After centigrade finished execution you can't see what value the local `t1` had, but you can see a copy of the value in `gt1`.

Remove the line from the script and run the script to redefine centigrade without the debug line.

# When =. and =: are the same
You have seen how `=.` and `=:` are different when used in a verb definition.

When you execute sentences in the ijx window you are not executing them inside a verb so the `=.` and `=:` have the same effect. In the ijx window:
```J
   a =. 123
   a
123
   a =: 234
   a
234
```
In the ijx window the `=.` and `=:` copulas are the same and it doesn't matter which you use to define a name as they both define the global name. The `=.` is easier to type and tends to be the one that is used. In a strict sense it would be better to explicitly use `=:` when defining a global name.

# When they aren't
You have seen that `=.` and `=:` in the ijx window are the same. And you have seen that inside a verb they are different. It is important to realize there is also a difference in scripts.

When you run a script, the load sentence is executed in the ijx window and the verb load executes the sentences in the script. So, the sentences in the script are executed in the load verb. This means that names defined with `=.` are defined as locals of the verb load. If you want to define a global in the script you must use `=:` . This is why the lines which define globals such as centigrade and fahrenheit in your script cf.ijs must use `=:` . If you used `=.` , they would be local to load and would disappear as soon as load finished execution.

Always think about whether a definition is global or local and use `=:` and `=.` accordingly.

# Locale
First of all, note that locale is a very different word from local, even though there is only one less letter in the latter.

A locale is a set of global names. There can be several locales, so there can be several sets of globals.

A global name in a locale is distinguished from the same name in other locales by qualifying the name with the addition of the locale name bracketed by `_` (underbar) characters. A name qualified by a locale is always a global name.
```J
   abc_def_ =: 2
```
The above sentence can be read as global abc in locale `def` is `2`.
```J
   abc_base_ =: 4
```
The above sentence can be read as global `abc` in locale base is 4.

If the locale name is elided, it is assumed to be base.
```J
   abc__   NB. the same as abc_base_
4
```
If a global name is not qualified with a locale name, then it is in the current locale. The base locale is the current locale unless it has been explicitly changed by executing a verb in a different locale. The following defines `abc` in the base locale:
```J
   abc =. 6
   abc_base_
6
   abc
6
```
Since the base locale is the current locale, the names `abc` and `abc_base_` are the same.

The name `abc_def_` is clearly different from `abc`, but so far there is no way of telling that anything special is going on. In what sense are `abc` and `foo` in the same (base) locale? And `abc` and `abc_def_` in different locales?

One way of distinguishing is to use the names utility verb that lists global names.
```J
   a =. 23
   b =. 24
   a_q_ =. 25
   w_q_ =. 26
   names 0	NB. 0 lists nouns
a abc b
```
Your names result may be different, but it will include all global nouns you have defined in the base locale. You should see the `a` and `b` that you defined above and note that you do not see the `w` that was defined in locale `q`.

To see the names defined in locale `q` you can do the following:
```J
   names_q_ 0	NB. names in locale q
a w
```
Nouns `a` and `w` are defined in the `q` locale.

Locales partition global names into different sets, and utilities, such as names, can work with globals in a particular locale.

The real power of locales comes into play with verbs defined in a locale. When a verb executes in a locale it executes with that locale, not the base locale, as the current locale.

Let's define a simple verb in the `q` locale to see how this works.
```J
   f_q_ =. 3 : 'a =: y'
```
This verb defines global a with its right argument. There can be many different locales, each with their own global `a`. But when `f_q_` executes, it executes in the `q` locale and the `q` locale is the current local, and global names it uses are from the `q` locale. Try the following experiments:
```J
   a =. 23	NB. define a in the base locale
   a_q_ =. 24	NB. define a in locale q
   f_q_ 100	NB. execute f in locale q
100
   a
23
   a_q_
100
```
Executing `f_q_` 100 defined global `a_q_` as 100. It did not affect the global `a` in the base locale.

If a verb explicitly references a name in a locale then that is the global that is affected. For example, define verb `g_q_` that defines a in the base locale. You will see that the `a` in the base locale is defined and the `a` in the `q` locale is not changed:
```J
   g_q_ =. 3 : 'a_base_ =: y'	NB. explicit locale name
   g_q_ 200
200
   a
200
   a__
200
   a_q_
100
```
Locales partition global names into separate sets. In particular, related nouns and verbs, say in a set of utilities, can be defined in their own locale. Their names don't conflict with names in the base or other locales. When you look at your application you can look at just the related globals that are in a particular locale. When a verb runs in a locale it uses globals from that same locale.

The names verb with an argument of 0 lists nouns, with 3 it lists verbs, and with 6 it lists locale names.
```J
   names_q_ 0
a w
   names_q_ 3	NB. verbs
f g
   names 6	NB. locale names
base j q z
```
The list of locale names is interesting. `base` and `q` you know about, but what about `j` and `z` ?

The globals in the `j` and `z` locales are defined when J starts up and runs the profile.ijs script. The j locale contains things which are useful in building an application and is discussed in the J Online Documentation.

The `z` locale is very interesting indeed.

# z locale
The `z` locale is the parent locale of all other locales.

If a name is not found in the current locale, and there is a definition for it in the `z` locale, then that definition is used as if it were in the current locale.

The `z` locale is for common utilities that you want to be available everywhere. From the `z` locale, they are available for execution in any locale as if they were in that locale, yet there is only a single copy, and the names in the z locale don't clutter up the names in the other locales.

The profile.ijs that runs when you start J defines many standard utilities in the `z` locale. You have used both the erase and the names verbs which are defined in the `z` locale. You can tell this by the following:
```J
   names 3	NB. verbs in the base locale
...
```
The above does not list names as a name, yet you are able to execute it. This is because when it is not found in the base locale, its definition from the `z` locale is used as if it were in fact defined in the base locale.
```J
   names_z_ 3	NB. verbs in z locale
...
```
The result is too long to list here. The verb names has a dyadic definition that takes a left argument which indicates the first letter of names to return.
```J
    'n' names_z_ 3
nameclass namelist names nc nl ...
```
# Script load
In addition to the utilities loaded with the standard profile, there are several additional scripts of standard utilities provided with the system. These standard utilities are documented in the J Online Documentation available from the J help menu. You could run these scripts directly, but you would need to remember the path to the script, as well as which locale to run them in. The standard profile provides utilities to make this easier for you. The scripts verb lists scripts that can be loaded with the load verb.
```J
   scripts ''
. . .
.... parts    plot     profile  scripts  stdlib ...
. . .
```
The scripts verb with an argument of 'v' lists the scripts with their full path.
```J
   scripts 'v'
. . .
compare  ~system\main\compare.ijs
 . . 
```
The ~system indicates the J system directory.

The convert script contains several conversion utilities.
```J
   load 'convert'
   toupper 'testing 1 2 3'
TESTING 1 2 3
   tolower 'Sir Richard'
sir richard
```

# Checkpoint B
At this point you should understand:

  - a text file that is a source of sentences is called a script file
  - a script file defines global names
  - how to create a new temporary script file
  - how to save a temporary script file as a permanent file
  - how to run a script file to execute its sentences
  - how to define a verb in a script file
  - how to define the monadic and dyadic cases of a verb
  - the difference between `=.` and `=:`
  - the difference between local and global
  - that a locale is a set of global names
  - that there can be more than one locale
  - that the base locale is the one you normally work with

Check your understanding by doing the following exercises:

  - create a new temporary script file
  - in the script define square as a monad that uses *: to square its argument
  - save the script in the user directory with the name square.ijs
  - run the script and test the verb square
  - close J, restart, use Run|File to run user\square.ijs and test it

# Debug - stepping through a verb
In an earlier section you added a debugging line to a verb definition that allowed you to see the results of intermediate steps when the verb was run. Sometimes you need more powerful tools than that.

Use `load` to load the debug utilities.
```J
   load 'debug'
```
Open your script file cf.ijs and run it.

Let's execute `centigrade`, but with a stop on each line so that you can take a look at exactly what is going on.
```J
   dbss 'centigrade *:*'
```
The dbss (Set Stop) argument requests a stop before executing all, indicated by `*:*`, lines in `centigrade`.
```J
   dbr 1
```
`dbr` with an argument of 1 requests that the system suspend execution when an error or stop occurs. When a verb is suspended it is halted in mid execution. You can examine definitions, change definitions, and you can resume execution of the suspended verb.
```J
   centigrade 212
|stop
|       t1=.y-32
|centigrade[0]
```
The error report (bars at the left margin) indicates execution stopped on line 0 of `centigrade` and shows the sentence from that line.

The execution of `centigrade` is suspended and the indent of six spaces, rather than three, indicates the suspension. The variable y is the argument.
```J
      y
212
```
The stop occurs before the line is executed, so `t1` has not been defined and if you try to look at it you will get a value error.

Use `dbrun` to continue execution. It will run the current line, and because stops are set on all lines it will then stop on the next line.
```J
      dbrun ''
|stop
|       t2=.t1*5
|centigrade[1]
      t1
180
      t1*5
900
```
`centigrade` is now stopped on line 1, and as you can see, you are able to check the value of local t1 that was defined in line 0. Step through the next lines and examine locals.
```J
      dbrun ''
|stop
|       t3=.t2%9
|centigrade[2]
      t2
900
      t2%9
100
      dbrun ''
100
```
You are no longer suspended in `centigrade` and you are back to the normal indent of three spaces.

Turn off the request for debug suspensions and reset to have no stops.
```J
   dbr 0
   dbss ''
```

# Debug - an error
Let's introduce an error into your `centigrade` verb to see how that looks and how you would find and fix it.

Open your cf.ijs script and edit the first line to have an error by adding quotes around the expression to the right of the copula.
```J
t1 =. 'y - 32'
```
Instead of t1 being defined as the result of `y - 32` , it will be defined as the string.

Run the script to make the new definition. Turn off debug suspension and request no stops and then run your buggy `centigrade`. Be sure to load the debug utilities if they are not already loaded.
```J
   dbr 0	NB. disable suspension
   dbss ''
   centigrade 212
|domain error
|   t2=.t1    *5
```
You are executing with suspension disabled (`dbr 0`) so execution did not suspend in centigrade and you have the normal 3 space indent.

If you look at the line in error it is clear that the 5 is a valid argument to times, so there must be something wrong with `t1`. But you don't know the value of `t1`. You could stare at the source for the error, but, in a complex situation, it might be quicker to use debug.

Enable suspension and rerun.
```J
   dbr 1	NB. enable suspension
   centigrade 212
|domain error
|   t2=.t1    *5
|centigrade[1]
```
There is a 6 space indent indicating suspension, and because `centigrade` is suspended you can look at the value of t1.
```J
      t1
y - 32
```
From the display of t1 it is clear that it is a string, not the number from the desired calculation. You can now look at the source to see where `t1` was defined and see that the quotes should not be there.

Edit the source to fix the definition by removing the quotes and run the script to redefine `centigrade`.

You want to run line 0 again to properly define `t1`. You can do this by using `dbjmp` to continue execution at line 0.
```J
      dbjmp 0
100
```
Since no stops are set and there are no other errors, line 0 of `centigrade` is executed, which sets a proper value into local `t1` and execution continues until finished.

# Comparative
The dyad = has a result of 1 if its left and right argument are equal, and a result of 0 if they are different.
```J
   23 = 34
0
   23 = 23
1
   a =. 'd'
   a = 'c'
0
   7 + a = 'c'
7
   7 + a = 'd'
8
```
Some programming languages treat the results of comparative primitives such as = as True and False values that are not numbers. In J the results of comparatives are just numbers.

There are several other comparative verbs: less-than `<` , less-or-equal `<:` , larger-than `>` , and larger-or-equal `>:` . These comparative primitives are sometimes called relationals.
```J
   7 < 8
1
   7 < 7
0
   7 <: 7
1
```

# Control structure
In centigrade the sentences in the definition are just executed sequentially, one after the other. To conditionally control which sentences are executed you use control structures.

Control structures are built with control words and sentences. The following is an example of a control structure:
```J
if. x = 'c'
 do. centigrade y
 else. fahrenheit y
end. 
```
The `if.` control word starts the control structure and the end. control word ends it. The result of the `x = 'c'` sentence is the test result and it determines which of the other sentences in the control structure are executed. If the test result is 1, then the sentence after the `do`. control word is executed. If the test result is any other value then the sentence after the `else`. control word is executed. In English: if the left argument equals the letter c, then execute `centigrade`, otherwise execute `fahrenheit`.

Use this capability to add a new verb to your cf.ijs script that will convert a number from Fahrenheit to centigrade or from centigrade to Fahrenheit depending on the value of the left argument. Open your cf.ijs script and add the following definition at the end.
```J
NB. convert f to c if x is 'c', otherwise c to f
convert =: dyad : 0
if. x = 'c'
 do. centigrade y
 else. fahrenheit y
end.
)
```
This defines the dyadic case of the verb. The dyad has a left argument with the name x and a right argument with the name `y` . The verb `convert` takes a left argument of `'c'` to convert a Fahrenheit value to centigrade. Any left argument other than `'c'` will convert a centigrade value to Fahrenheit.

Note that you use your verbs `fahrenheit` and `centigrade` just as you would use primitive verbs.

Run the script and test convert.
```J
   'c' convert  212
100
   'f' convert 100
212
```
Normally a sentence is a line in a script. However, with control words separating a line into several sentences it is possible to have more than one sentence on a line.

The following line is equivalent to the multiple lines used earlier.
```J
if. x = 'c' do. centigrade y else. fahrenheit y end.
```
Control structures are only allowed in definitions and you cannot type one directly into the ijx window for execution.

There are nine control structure patterns:
```J
if. T do. B end.
if. T do. B else. B1 end.
if. T do. B elseif. T1 do. B1 elseif. T2 do. B2 end.
try. B catch. B1 end.
while. T do. B end.
whilst. T do. B end.
for. T do. B end.
for_i. T do. B end.
select. T
 case. T0 do. B0
 case. T1 do. B1
 fcase.T2 do. B2
 case. T3 do. B3
end.
```
A control structure starts with `if.` , `try.` , `while.` , `whilst` , `for.` , `for_i.` , or `select.` and ends with a matching end. .

Words beginning with T or B denote a block of 0 or more sentences and can contain nested control structures.

The result of the last sentence in a T block determines which block is executed next and whether execution in the control structure is finished.

Often the T block is a single sentence that makes a simple test like the one in the example.

The `try.` control structure is an interesting one. It executes the B block of sentences, and if there are no errors it skips to the end of the structure. However, if there is an error, then the B1 block is executed.

The `while.` control structure executes the T block and if its result is not 0 then it executes the B block and continues this until the T block has a 0 result. If the T block is 0 the first time, then the B block is not executed.

The whilst. control structure is the same as while. except that the T block is skipped the first time. This means that the B block is always executed at least once.

In the for. structure, the B block is evaluated once for each item of the array A that results from evaluating the T block. In the for_i. form, the local name i is set to the value of an item on each evaluation of the B block and i_index is set to the index of the item. A break. goes to the end of the for. control structure, and continue. goes to the evaluation of B for the next item.

In the select. structure, the result R of T is compared to the elements of the result Ri of Ti , and the Bi block of the first case. or fcase. with a match is evaluated. Evaluation of the select. control structure then terminates for a case. , or continues with the next B(i+1) block for an fcase. (and further continues if it is an fcase.).

See the J Dictionary for more information on control structures.

# Checkpoint C
At this point you should understand:

  - that load `'debug'` loads debug utilities
  - the general idea of verb debugging
  - how control words create control structures by grouping sentences into blocks
  - what the T block test result is
  - how the test result determines which B block to execute
  - how the test result determines when control structure execution is finished
Check your understanding by doing the following exercises:

  - debug step through your convert verb
  - create a temporary script file and define a verb called `conv` that is similar to `convert`, but insists on a `'f'` argument to do the conversion to Fahrenheit and gives a string result indicating there was an error if the left argument is neither `'c'` nor `'f'`. Hint: use the control structure sketched out here:
    ```J
    if. x = 'c' do. ...
      elseif. x = 'f' do. ...
      elseif. 1 do. 'left arg not c or f'
    end.
    ```
    or try a `select.` structure.

  - create a temporary script file and define a dyad called plus that adds its left argument to its right. But, if there is an error, it should give a string result. Hints: use dyad `: 0; 4 plus 9` should return 13; `'a' plus 9` should return your error string (perhaps, `'there was an error'`); use a `try.` control structure to catch the error and give the string result.
