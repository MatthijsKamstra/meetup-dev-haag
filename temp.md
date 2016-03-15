<!--





| |  |  |
|--|--|--|
| Flash | Bytecode | Games, Desktop, Mobile |
| Neko | Bytecode | Web, CLI |
| JavaScript | Source&nbsp;code | Games, Web, Desktop |
| ActionScript&nbsp;3 | Source&nbsp;code | Games, Mobile |
| PHP | Source&nbsp;code | Web |
| C++ | Source&nbsp;code | Games, Desktop, Mobile, CLI |
| Java | Source&nbsp;code | Desktop, Mobile, CLI |
| C# | Source&nbsp;code | Desktop, Mobile |
| Python | Source&nbsp;code | Web, Desktop, CLI |



## The Haxe Language

- Strictly typed
- Type inference
- Object Oriented
- String interpolation
- Iterators
- Array comprehension
- Pattern matching
- Conditional compilation
- Externs



- Data structures
- Math
- Regular expressions
- JSON & XML
- HTTP
- ZIP
- Cryptography
- Unit testing
- File I/O
- File system
- MySQL & SQLite
- Native processes
- Target-specific APIs
- Networking (C++)
- DOM & Cookies (JS)
- Sessions (PHP)



- Compiles to target language or bytecode
- Single front-end parses Haxe to AST
- Multiple back-ends translate AST to specific targets
- Written in OCaml
- Dead code elimination
- Code completion
- Function inlining
- Resource embedding
- Metadata



-->


Haxe Features

- Familiar AS3/C/Java-style syntax. <!-- .element: class="fragment fade-in b" data-fragment-index="1" -->
- Memory management via garbage collection. <!-- .element: class="fragment fade-in b" data-fragment-index="2" -->
- Strict type safety, with a powerful type inference engine. <!-- .element: class="fragment fade-in b" data-fragment-index="3" -->
- Many modern features like: <!-- .element: class="fragment fade-in b" data-fragment-index="4" -->
	- lambdas/closures <!-- .element: class="fragment fade-in b" data-fragment-index="5" -->
	- generics <!-- .element: class="fragment fade-in b" data-fragment-index="6" -->
	- abstract data types (GADT's) <!-- .element: class="fragment fade-in b" data-fragment-index="7" -->
	- reflection <!-- .element: class="fragment fade-in b" data-fragment-index="8" -->
	- metadata <!-- .element: class="fragment fade-in b" data-fragment-index="9" -->
	- and a powerful macro system for language extension <!-- .element: class="fragment fade-in b" data-fragment-index="10" -->

::note::

From Waneck: https://github.com/proletariatgames/unreal.hx







What is Haxe?
First release in April 2006
Open source language
Strictly typed
Developed by Nicolas Cannasse
(Well known in Flash community thanks to MTASC compiler)



Why Haxe is cool?
Cross-platform OOP language
Good syntax
Provides good API for extending language
Generates sources for target language
Big community
Haxelib - repository for your Haxe libs
online REPL try.haxe.org


::slide::

# History
The **ECMAScripts**

- ECMAScript 3
  - 1st widely implemented Javascript
- ECMAScript 4
  - Failed as a Javascript spec
  - Implemented in ActionScript 3
- ECMAScript 5
  - 2nd widely implemented Javascript
- ECMAScript 6
  - Hot off the presses
  - Now called ES2015



::slide::

So ... **Haxe**?

inspired by AS3 <!-- .element: class="fragment fade-in b" data-fragment-index="1" -->

so, quite ECMAScript-ish <!-- .element: class="fragment fade-in b" data-fragment-index="2" -->

also has elements of OCaml & Java <!-- .element: class="fragment fade-in b" data-fragment-index="3" -->

take Javascript, and add types <!-- .element: class="fragment fade-in b" data-fragment-index="4" -->

Typescript, anyone? <!-- .element: class="fragment fade-in b" data-fragment-index="5" -->

::note::

- Haxe is *not* ECMAScript compliant, it is more of a fork/ branch
	- See [this article](http://jcward.com/Haxe+Notes+For+ECMA+Coders+Object+Literal+Notation) which enumerates one of the more obvious differences
- For a Javascript / ActionScript developer, similar enough for most of it to feel familiar
- ES6/ ES7 features are not planned to be implemented, whoever, many of them have already been included
	- There are macros for this, if you *really* want to


::slide::

Focus

- Due to roots, very centred around Game Dev
- LudumDare: Dominated by HaxeFlixel
- This is beginning to change now




::slide::

... and now, the **killer** feature! <!-- .element: id="cross-compile" -->

::slide::

# Cross-compile

![Haxe targets: iOs, Android, HTML5, Neko, NodeJs, Flash, C++, Python, Csharp, PHP, Java](img/haxe-targets.png)


::slide::

Most languages: Language + Standard Lib <!-- .element: class="fragment fade-in b" data-fragment-index="1" -->

Haxe: Those, plus cross platform APIs <!-- .element: class="fragment fade-in b" data-fragment-index="2" -->

Transpiles to natively compile-able code <!-- .element: class="fragment fade-in b" data-fragment-index="3" -->

VMs or run times are <!-- .element: class="fragment fade-in b" data-fragment-index="4" -->
***optional*** <!-- .element: class="fragment fade-in b" data-fragment-index="5" -->

::slide::

Awesome - right now:

- HTML+JS
- C++ --> iOS
- C++ --> Android NDK
- Java ( --> Android SDK )
- Flash

::slide::

Awesome - eventually:

- PlayStation
- Xbox

[announcement by Lars Doucet](http://www.fortressofdoors.com/openfl-for-home-game-consoles/)

::slide::

Auto-magic tooling

```bash
haxelib install openfl
haxelib run openfl setup
# Unleash the dragons!
openfl setup android
# {android,ios,html5,flash,linux,mac,windows,blackberry,tizen}
```

(Same feeling as `npm i -g react-native-cli` for the first time)

::note::

- OpenFL is one of the more popular haxelibs out there
- It's a framework, used primarily to compile games (Flash API) that run many target devices







::slide::

Andy Li's [talk at a recent London Meetup](http://youtube.com/watch?v=7__Unc5D130):

> There are over 300 transpile to Javascript languages/ platforms ...
> It is a balancing act, where you maximise the pros and minimise the cons ...
> Haxe has a very good value proposition from this point of view

(I'm paraphrasing)

::slide::

| Pros | Cons |
| :--- | :--- |
| Static type checking + type inference | Lose the flexibility of object literals |
| Idiomatic JS                          | `==` instead of `===` |
| non-JS targets as well                | Transpile adds extra build step |
| Functional programming                | Classes everywhere |
| Compile-time optimisation             |  |
| Super fast compiler                   |  |
| Mature - 2005                         |  |
| Macros                                |  |

::note::

- Haxe itself ensures strict equality, however the JS it outputs uses `==` instead of `===`
- Haxe satisfies both sides of the camp in the functional vs OOP thing, so it really is your preference
- On the matter of being used to interpreted languages. Haxe as a language has proven itself to be very extensible. JS devs who prefer to write Coffeescript might enjoy [Raxe](https://raxe.rocks/), which is Haxe with ruby-inspired syntax

::slide::

| JS only | JS + Android + iOS |
| :---: | :----: |
| Typescript   | Haxe |
| Coffeescript | PhoneGap|
| many more... | React Native |
|              | NativeScript |
|              | Emscripten |
|              | GWT & LLVM |
|              | ... many more |

::slide::

Cross-compilation is ***the reason*** to try Haxe


