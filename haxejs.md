
<!-- .slide: data-background="img/logo/haxe-logo-vertical-big.png" data-background-size="700px" -->

::note::

Welcome to my presentation!
And thank you for having me.

::slide::

# Haxe for js

nodejs, c++, php, flash, java, IOS, Android, html5 & more<!-- .element: class="fragment" data-fragment-index="1" -->

::slide::

<!-- .slide: data-background="#027D81" -->

#Who?

::subslide::

## Matthijs Kamstra
aka [mck]  
[@matthijskamstra](https://twitter.com/matthijskamstra)  

<!--
[*speaker notes*](haxejs.md)
-->

::subslide::

<!-- .slide: data-background="img/logo/FONK_Logo_Dark_01.png" data-background-size="800px" data-background-color="#0C0F22"-->

::note::

#Dayjob

::subslide::

# fonk.amsterdam

#### Creative Developer

~~ActionScript 3~~  <!-- .element: class="fragment" data-fragment-index="1" -->  

Web <!-- .element: class="fragment" data-fragment-index="2" -->  

Lab <!-- .element: class="fragment" data-fragment-index="3" -->  

Java / Android <!-- .element: class="fragment" data-fragment-index="4" -->  

::subslide::

<!-- .slide: data-background="img/slides/I_am_Grumm_the_Screamer_Red.jpg" data-background-size="1000px" data-background-color="#ffffff"-->

::note::

#Other/Night job


::subslide::

# Papertoy designer/engineer


::subslide::

<!-- .slide: data-background="img/slides/papertoy_glowbots.jpg" data-background-size="500px" -->

::subslide::

fun/art projects/tools

- Twitter account i-am-grumm  <!-- .element: class="fragment" data-fragment-index="1" -->  
- Backend for Grumm.nl  <!-- .element: class="fragment" data-fragment-index="2" -->  
- Tweening engine go  <!-- .element: class="fragment" data-fragment-index="3" -->  
- Svg lib <!-- .element: class="fragment" data-fragment-index="4" -->  
	- Vector generated patterns <!-- .element: class="fragment" data-fragment-index="5" -->  
	- Cricut patterns <!-- .element: class="fragment" data-fragment-index="6" -->  
	- Complex static website generator (CyberMonk) <!-- .element: class="fragment" data-fragment-index="7" -->  
	- Simple static website generator (ButterFly) <!-- .element: class="fragment" data-fragment-index="8" -->  
- Documentation : HaxeJS / HaxeNode <!-- .element: class="fragment" data-fragment-index="9" -->  
- Playrr (Youtube/Spotify radio app)  <!-- .element: class="fragment" data-fragment-index="10" -->  
- Paperart Bugs <!-- .element: class="fragment" data-fragment-index="11" -->  
- Markdown/html presentation tool Slidrr <!-- .element: class="fragment" data-fragment-index="12" -->  

::note::

- Twitter account [i am grumm](https://twitter.com/i_am_grumm)    
- Backend for [Grumm.nl](http://www.grumm.nl/)    
- Tweening engine [go](http://matthijskamstra.github.io/go/)    
- Svg lib   
	- Vector generated patterns   
	- Cricut patterns   
	- Complex static website generator (CyberMonk)   
	- Simple static website generator [ButterFly](https://github.com/ashes999/butterfly/)   
- Documentation : 
	- [HaxeJS](http://matthijskamstra.github.io/haxejs/) 
	- [HaxeNode](http://matthijskamstra.github.io/haxenode/)   
- [Playrr (Youtube/Spotify radio app)](http://matthijskamstra.github.io/playrr/)    
- [Paperart Bugs](https://twitter.com/MatthijsKamstra/status/701512108106719233)   



::slide::

<!-- .slide: data-background="#027D81" -->

#What?

::subslide::

<!-- .slide: data-background="img/logo/haxe-logo-vertical-big.png" data-background-size="700px" -->

::subslide::

###Let's talk about Haxe (baby)!

What is Haxe?<!-- .element: class="fragment" data-fragment-index="1" -->  

Why should I use it?<!-- .element: class="fragment" data-fragment-index="2" -->  

What problem does it solve?<!-- .element: class="fragment" data-fragment-index="3" -->  

All that glitters is not gold<!-- .element: class="fragment" data-fragment-index="4" -->  

Summary<!-- .element: class="fragment" data-fragment-index="5" -->  

Q&A<!-- .element: class="fragment" data-fragment-index="6" -->  



::slide::

<!-- .slide: data-background="#AB1574" -->

#What is Haxe?


::subslide::

the cross-platform toolkit

> Haxe is an open source toolkit based on a modern, high level, strictly typed programming language, <!-- .element: class="fragment" data-fragment-index="1" --> 

> a cross-compiler, <!-- .element: class="fragment" data-fragment-index="2" --> 

> a complete cross platform standard library and ways to access each platform's native capabilities. <!-- .element: class="fragment" data-fragment-index="3" --> 

source: [haxe.org](http://haxe.org/)

::note::

the cross-platform toolkit

Haxe is an **open source** toolkit based on a modern high level strictly typed programming language, a state-of-the-art light-speed cross-compiler, a complete cross-platform standard library, and ways to access to each platform's native capabilities

*from the mothership, but what does it solve?*

::subslide::

<!-- .slide: data-background="img/knife3.jpg" data-background-size="800px" data-background-color="#FFFFFF" -->


::subslide::

##What is the Haxe toolkit

- Cross-platform development toolkit <!-- .element: class="fragment fade-in b" data-fragment-index="1" -->
 	- Runs on Windows, Mac & Linux <!-- .element: class="fragment fade-in b" data-fragment-index="2" -->
- The Haxe Programming Language <!-- .element: class="fragment fade-in b" data-fragment-index="3" -->
- The Haxe Cross-Compiler <!-- .element: class="fragment fade-in b" data-fragment-index="4" -->
- The Haxe standard library <!-- .element: class="fragment fade-in b" data-fragment-index="5" -->
- Haxe Additional Tools <!-- .element: class="fragment fade-in b" data-fragment-index="6" -->

::note::
It is strictly typed and very easy to learn if you are already familiar with Java, C++, PHP, AS3 or any similar object oriented language.

The Haxe Compiler is responsible for translating the Haxe programming language to the target platform native source code or binary.

General purpose: Array/Map/String/Date Timer/Template/Unit/crypto
System: C++ C# Java Neko PHP - Filesystem/db/File
Target specific: Each Haxe target has a distinct sub-directory containing target-specific APIs. These can only be accessed when compiling to the given target.

Macros / IDE integration

haxelib

::subslide::

### A Brief History of Haxe

- Created by Nicolas Cannasse <!-- .element: class="fragment" data-fragment-index="1" -->
- Haxe predecessor MTASC started in 2001<!-- .element: class="fragment" data-fragment-index="2" -->
- Dev started at Motion Twin in October 2005<!-- .element: class="fragment" data-fragment-index="3" -->
- First beta released February 2006<!-- .element: class="fragment" data-fragment-index="4" -->
- Initial support for AVM and Neko VM targets<!-- .element: class="fragment" data-fragment-index="5" -->
- New language targets created by contributors<!-- .element: class="fragment" data-fragment-index="6" -->
- Haxe Foundation formed November 2012<!-- .element: class="fragment" data-fragment-index="7" -->
- World Wide Haxe Conference (WWX) held annually in Paris by Silex Labs<!-- .element: class="fragment" data-fragment-index="8" -->

::note::

[@ncannasse](https://twitter.com/ncannasse)
Motion Twin creates primairily games


::subslide::

### Timeline

- 2005: haXe 1.0-alpha (Flash/Neko)
- 2006: haXe 1.0 (JavaScript)
- 2007: haXe 1.12 (ActionScript 3)
- 2008: haXe 2.0 (PHP)
- 2009: haXe 2.04 (C++)
- 2012: Haxe 2.09
- 2012: Haxe 2.10 (Java & C#)
- 2013: Haxe 3.0
- 2015: Haxe 3.2 (Python)
- 2016: Haxe 3.x (Lua?)


::subslide::

<!-- .slide: data-background="img/knife3.jpg" data-background-size="800px" data-background-color="#FFFFFF" -->

::subslide::

# WRITE ONCE,<br>TARGET MANY

::subslide::

<!-- .slide: data-background="img/logo/all-targets-big.png" data-background-size="1000px" -->

::note::

The C++ target allows you to target major mobile platforms at native speed.


::subslide::

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

::note::

Source code! not VM

::slide::

<!-- .slide: data-background-image="img/cute/cutebabypanda.jpg" -->

::note::

I promised a panda.
https://twitter.com/MatthijsKamstra/status/703934883454910466



::slide::

<!-- .slide: data-background="#AB1574" -->

#Why should I use it?

::note::

code talks, so lets dive into it


::subslide::

## The Haxe Language

- Strictly typed <!-- .element: class="fragment fade-in b" data-fragment-index="1" -->
- Type inference <!-- .element: class="fragment fade-in b" data-fragment-index="2" -->
- Object Oriented <!-- .element: class="fragment fade-in b" data-fragment-index="3" -->
- String interpolation <!-- .element: class="fragment fade-in b" data-fragment-index="4" -->
- Iterators <!-- .element: class="fragment fade-in b" data-fragment-index="5" -->
- Array comprehension <!-- .element: class="fragment fade-in b" data-fragment-index="6" -->
- Pattern matching <!-- .element: class="fragment fade-in b" data-fragment-index="7" -->
- Conditional compilation <!-- .element: class="fragment fade-in b" data-fragment-index="8" -->
- Externs <!-- .element: class="fragment fade-in b" data-fragment-index="9" -->

::note::

http://haxe.org/documentation/introduction/language-features.html


::subslide::

# Strictly typed *

```
var doingTalk : Bool = true;
var minutes : Int = 30;
var subjects : Array<String> = [
	"The Haxe Language",
	"The Haxe Cross-Compiler",
	"haxelib"
];
var version : Map<String,String> = [
	"haxe" => "3.1.3",
	"neko" => "2.0.0"
];
```
<!-- .element: class="fragment fade-in b" data-fragment-index="1" -->

::note::

- compile time vs runtime time checking


::subslide::

# Type inference

```
var doingTalk = true;
var minutes = 30;
var subjects = [
	"The Haxe Language",
	"The Haxe Cross-Compiler",
	"haxelib"
];
var version = [
	"haxe" => "3.1.3",
	"neko" => "2.0.0"
];
```
<!-- .element: class="fragment fade-in b" data-fragment-index="1" -->


::note::

- http://haxe.org/manual/type-system-type-inference.html
> Whenever a type other than Dynamic is unified with a monomorph, that monomorph becomes that type: it morphs into that type. Therefore it cannot morph into a different type afterwards, a property expressed in the mono part of its name.


::subslide::

# Object Oriented

```
class GuineaPig {
	var name : String;
	var age : Int;
	public function new(name, age) {
		this.name = name;
		this.age = age;
	}
}
var pig1 = new GuineaPig("Maisie", 1);
var pig2 = new GuineaPig("Tilly", 2);
```
<!-- .element: class="fragment fade-in b" data-fragment-index="1" -->


::subslide::

# String interpolation

```
var x = 1;
var y = 2;
trace('$x + $y = ${x + y}');
// Outputs: 1 + 2 = 3
var lang = "haxe";
trace('Welcome to ${lang.toUpperCase()}!');
// Outputs: Welcome to HAXE!
```
<!-- .element: class="fragment fade-in b" data-fragment-index="1" -->


::subslide::

# Iterators
```
var guineaPigs = [
	"Maisie",
	"Tilly"
];
for (guineaPig in guineaPigs) {
	trace(guineaPig);
}
for (i in 0...guineaPigs.length) {
	trace(guineaPigs[i]);
}
```
<!-- .element: class="fragment fade-in b" data-fragment-index="1" -->


::note::

Iterating over a set of values, e.g. the elements of an array, is very easy in Haxe courtesy of iterators.

Not the classic c-style for loop
but there is a macro for that!
```
// js
// (classic C-style for-loop)
for (i = 0; i < 100; i++) {
}
for each (value in items) {
}
for (propertyName in object) {
}
```
<!-- .element: class="fragment fade-in b" data-fragment-index="1" -->


::subslide::

# Array comprehension
```
var numbers = [for (i in 0...10) i];
trace(numbers);
// Outputs 0,1,2,3,4,5,6,7,8,9
var oddNumbers = [
	for (i in numbers)
		if (i % 2 == 1) i
];
trace(oddNumbers);
// Outputs: 1,3,5,7,9
```
<!-- .element: class="fragment fade-in b" data-fragment-index="1" -->

::note::

Create and populate arrays quickly using for loops and logic.

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Array_comprehensions

ECMAScript 6
http://ariya.ofilabs.com/2013/01/es6-and-array-comprehension.html

http://haxe.org/manual/lf-array-comprehension.html

::subslide::

#Pattern matching
```
var myStructure = {
	name: "haxe",
	rating: "awesome"
};
var value = switch(myStructure) {
	case { name: "haxe", rating: "poor" }:
		throw false;
	case { rating: "awesome", name: n }:
		n;
	case _:
		"no awesome language found";
}
trace(value); // haxe
```
<!-- .element: class="fragment fade-in b" data-fragment-index="1" -->

::note::

Structure matching


::subslide::

# Conditional compilation
```
var target:String;
#if js
	target = "JavaScript";
#elseif cpp
	target = "C++";
#else
	target = "Unknown";
#end
trace(target);
```
<!-- .element: class="fragment fade-in b" data-fragment-index="1" -->

::note::

Conditional Compilation allows compiling specific code depending on compilation parameters.


::subslide::

# Externs
```
extern class Math {
	static var PI(default, null):Float;
	static function floor(v:Float):Int;
}
var pi = Math.floor(Math.PI);
$type(pi); // Int
```
<!-- .element: class="fragment fade-in b" data-fragment-index="1" -->

::note::

Externs can be used to describe target-specific interaction in a type-safe manner.
A common example from the *Haxe Standard Library* is the Math class,

The Haxe Standard Library comes with many externs for the Flash and JavaScript target. They allow accessing the native APIs in a type-safe manner and are instrumental for designing higher-level APIs. 

http://haxe.org/manual/lf-externs.html


::subslide::

# Who uses Haxe?

::subslide::

> Haxe is used worldwide by both independent developers and large corporate teams.

::subslide::

<!-- .slide: data-background="img/slides/who-uses-haxe.png" data-background-size="800px" data-background-color="#ffffff" -->

::subslide::

<!-- .slide: data-background="img/logo/fbi.png" data-background-size="600px" data-background-color="#ffffff" -->


::note::

Reverse engineered: the Flash code the FBI used to unmask some dark net pedophiles on Tor

https://twitter.com/elsassph/status/615942366478864384


::subslide::

<!-- .slide: data-background="img/logo/all-targets-big.png" data-background-size="1000px" -->

::note::

Why should you use it?

freedom to choose!

Uncle Bob story!


::slide::

<!-- .slide: data-background-image="img/cute/puppy.jpg" -->


::slide::

<!-- .slide: data-background="#AB1574" -->

#What problem does it solve?


::subslide::

<!-- .slide: data-background="img/slides/Plan-Design-Develop.png" data-background-size="900px" data-background-color="#FAFAF6" -->

::note::

short version of (agile team) most processes


::subslide::

# Developers

::note::

tribe of developers, they are a team,
a strong group, 
but are they?

::subslide::


<!-- .slide: data-background="img/slides/right.gif" -->

::subslide::

## Front-end

&

## Back-end


::subslide::


<!-- .slide: data-background="img/slides/staredown.jpg" data-background-size="900px" -->

::subslide::

##вы будете моя резиновая утка?

&

##내 고무 오리 것인가?

google translate<!-- .element: class="fragment fade-in b" data-fragment-index="1" -->

::note::

Russian & Korean


::subslide::

![](img/slides/rubberduck_small.png)

"Will you be my rubber duck?"<!-- .element: class="fragment fade-in b" data-fragment-index="1" -->

::note::

The name is a reference to a story in the book The Pragmatic Programmer in which a programmer would carry around a rubber duck and debug their code by forcing themselves to explain it, line-by-line, to the duck.

::subslide::

<!-- .slide: data-background="img/slides/no_pokemon_giphy.gif" data-background-size="900px" data-background-color="#000000" -->

::note::

Personal experience: not a difficult question...

busy, no time, ...

::subslide::

<!-- .slide: data-background="img/slides/comfortzone.jpg" data-background-size="800px" data-background-color="#FAF9F7" -->

::note::


::subslide::

<!-- .slide: data-background="img/slides/Comfort-Zone-Model.jpg" data-background-size="900px" data-background-color="#FFFFFF" -->


::subslide::


<!-- .slide: data-background="img/slides/howtofix.gif"  -->

::note::

how to fix it?

::subslide::

## what if both speak the same language

::subslide::

## आप मेरे रबर बतख हो सकता है?

&

## आप मेरे रबर बतख हो सकता है?

::note::

Hindi

::subslide::

<!-- .slide: data-background="img/slides/happy_super.gif" -->

::subslide::

# Plan

::subslide::

<!-- .slide: data-background="img/slides/happy_evil.gif"-->

::subslide::

# Manager

::subslide::

<!-- .slide: data-background="img/slides/happy_manager.gif" -->

::subslide::

# Everybody

::subslide::

<!-- .slide: data-background="img/slides/happy_dance.gif" -->



::subslide::

> “Use only that which works, and take it from any place you can find it.” 

_Bruce Lee, Tao of Jeet Kune Do_

::slide::

<!-- .slide: data-background-image="img/cute/cutepig.jpg" -->

::slide::

<!-- .slide: data-background="#AB1574" -->

#All that glitters is not gold

::subslide::

> “A developer who is not optimistic shouldn't be a developer.” 

_Harry Triguboff_


::subslide::

# Haxe shortcomings

::subslide::

# IDE

(other then Windows)

::note::

- Not-so-good IDE support:
	- Good support in Flash-/Haxe-Develop (Windows only)
	- Limited support in IntelliJ IDEA for all platforms
	- Few other IDEs like FDT
- Verbosity (i.e. no short lambdas)
- Written in OCaml :)

Not IDE, but editors:
- atom, virtual studio code, bracket, sublime text

::subslide::

# Documentation 

::note::

api documentation is beter, 
but examples are limited
haxejs / haxenode documentation

::subslide::

# Visibilty

::note::

Games... and the rest?

Presentation / talks

::subslide::

# Presentation

::note::

website, information, 

::subslide::

# simpler

::note::

- Haxe installer
- editor installer
- language installer
- how to start
- learn from internet
- not a lot of developers
- books?

::subslide::

# Run like 1-man show

::note::

Haxe Foundation

- Core contributors to the compiler and the language spec
- See @glazou's
  [critique of the Haxe foundation](http://www.silexlabs.org/quaxe-infinity-and-beyond/)
  - Controversy alert: Run like 1-man show
- Could learn from the iojs/node foundation

- Daniel Glazman sits on one of W3C's committees, and so his opinion carries a lot of weight
- However, this talk was very polarising amongst the Haxe community, and many of them reject his point of view
- His point that large corporations will only invest in technologies that appear to be governed by a stable committee (or another corporation) still should be considered though, and seeing how NodeJs foundation has recruited comapnies to sit on its board
- Read "Regarding Haxe Foundation" in
  [this heated discussion](https://groups.google.com/d/msg/haxelang/i8iXdpK8oAc/qgUmBo5sYPEJ)

::subslide::

# diversity

::note::

need more vocal people from other targets

::slide::

<!-- .slide: data-background-image="img/cute/cute-4.jpg" -->

::slide::

<!-- .slide: data-background="#AB1574" -->

# Summary 

::subslide::

- Familiar AS3/C/Java-style syntax. 
- Strict type safety, with a powerful type inference engine.
- 9 compilation targets
- reduced language/platform lock-in
- open source
- started 10 years ago
- modern language and compiler features
- a fast optimizing compiler
.


::subslide::

## Resources

- Haxe Website - [haxe.org](http://haxe.org)
- Manual -[haxe manual](http://haxe.org/manual)
- API Reference - [api.haxe.org](http://api.haxe.org)
- haxelib - [lib.haxe.org](http://lib.haxe.org)
- Try Haxe - [try.haxe.org](http://try.haxe.org)
- Learn Haxe in Y Minutes - [learnxinyminutes haxe](http://learnxinyminutes.com/docs/haxe)
- Haxe Roundup - [haxe.io](http://haxe.io)

::note::

online REPL try.haxe.org

> REPL stands for Read Eval Print Loop and it represents a computer environment like a window console or Unix/Linux shell where a command is entered and system responds with an output in interactive mode. Node.js or Node comes bundled with a REPL environment.


::slide::

<!-- .slide: data-background-video="video/thats_all_folks.mp4,video/thats_all_folks.webm" -->
# the end!

::slide::

<!-- .slide: data-background="#AB1574" -->

#Q&A





