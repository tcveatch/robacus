"ROBACUS" evokes a robotic abacus, a computer-human collaboration
system. 

Robacus was authored by Dr. Tzuo "Joe" Ching (PhD, UC Berkeley,
1972??) in his 1970's, 1980's work modelling nuclear reactors.

Recognizing the intractibility of the network of mutual dependencies
and the complexity of the math that would be required to answer urgent
questions about these most complex and extreme machines ever made by
humans, Dr. Ching built a software program that contains a user
interview system that extracts from the user a description of the
problem and then, recursively, its components and their dependencies,
so that the needed calculations can be made by a diligent,
comprehensive, and error-free, partly computer-generated, analysis of
what could be a very complex system.  Computer-driven calculations and
random simulations (Monte Carlo methods) rather than pure math were
emphasized in order to resolve issues too complex for the human mind.

As example and proof, as I understand it, Dr. Ching used this program to quickly and
effectively model the details of the Three Mile Island nuclear plant
*during* its meltdown so as to help to bring the unfolding disaster
under control.  Let me merely point out that shortly thereafter, he bought a
large apartment complex in Berkeley, and now enjoys the life of Riley.
Clearly something worked, grandiosity
notwithstanding.  It is incumbent on us to figure out what it was he
actually achieved.

On the one hand, his prolific writings and surprising opinions, which
may seem often outlandish, shocking, or strange at a first impression,
provide a useful alternative window on many things that we might not
normally question (browse around in html-files/\* or
generated-html/\*). Much suffers in translation.  But there are
insights in there worth pulling out, in addition to the software
archived here.

Since his original work, he has used this quite general-purpose
program in all kinds of unrelated explorations, from quantitative
modeling of a poulty pandemic (see ./\*-files/ep????), to the design
and analysis of a novel approach to table tennis technique, (see
./pongfu-files).  More, the thousand relics of an active intellectual
career may be found in the robacus filesystem, because the included
programs made it easy to generate web pages, documentation, inputs as
well as outputs, logs, and data files.  The form in which I received
them was a flat filesystem in the robacus/ directory, which at this
writing contained 3846 files.  Too huge to browse!

As a service to Joe, my crazy brilliant friend, and to you who may
wish to learn something from him, I have put this
robacus directory of his into some kind of navigable order by sorting
the files into categories like html, fortran, perl, log, data, etc.,
files.  See below.

One category, which I have called nuclear-files, is not included in
the public distribution I'm putting on github, despite the internal
notes found in these files saying there is no restriction on
distribution.  What I've posted is evidently unrestricted and safe to post,
but please let me know of any questions or issues!

Below you will find the categories I used, and what kinds
of things may be found there.  To enter into and make sense of this
archive, I would take start from this README, then wander
through the howto-files which give context for most of the other
files.  On one track, please try to understand, or compile and use, robacus
itself.  On another track, you could spend quite a long time browsing
the html-files, getting familiar with the products of Joe's strong
mind.

Speaking of the code, remember that it goes back to the time when
computer variables and filenames were all 6 characters.  We're talking
FORTRAN code from probably 1966, probably on IBM 360's or God knows
what kinds of computers.  Some of it was made to run on Cray
supercomputers, probably in the 1980's.  There are programs in here
for manipulating decks of IBM cards.  Old School.  

Point being, you may want to learn to deal with 6 letter identifiers,
which are surprisingly informative, and also frustratingly
uninformative, just as often.  In short, please get comfortable with
sentences like DESCRI PROBLE TO MODEL, okay?  Joe seems to like these
as it puts Chinese speakers on a level playing field with English
speaking natives.

But don't dismiss the contents due to their age.  Many of these
programs are career-sized achievements by groups of the best and
brightest, brought together to solve the most urgent problems of the
nuclear age, where the world is under threat from nuclear accidents,
even nuclear war.  They were damn smart and they concieved,
implemented, proved correct, and effectively used methods found here
to solve problems of the highest complexity, urgency and value.  If
so, we should not lose, and will profit by understanding, what they
have done.  For that reason I bring you "ROBACUS".

You might even be able to compile and run it (I'd love to see a port to WebAssembly,
which would enable it to be executed on any modern platform.)  If you are
able, please try!  ... Or, please give me some guidance as to how I might begin

If something should be in a different place, or if you can improve the
understandability or utility of these files, please send me the changes
and I'll try to put them to use.  Thank you!

 - Tom Veatch (contact information at tomveatch.com)
------------------------------------------------------------------------

README			This file

robacus.tgz     Download then run 'tar zxf robacus.tgz' to unpack the following:

howto-files/		Look at these first, to make sense of the rest.

fortran-code/		Here are the code bases Joe inherited and built upon,
			as well as Joe's code itself.
			I think rolupd is the key program, but it's 50k lines!

DESCRI_PROBLE-files	Inputs to robacus, answering the question,
 			"Describe the problem to be modelled".

PROC-files		I think these are sequences of system commands to drive
			program runs, which might include tape reader/writers,
			grabbing data files from wherever, and
			feeding them through programs in some ancient computer
			environment.  I identified them by searching for ".PROC,"

abbreviation-files/	Robacus builds solutions from components, and uses
			internal as well as external names to keep
			track of them and their mutual dependencies.
			I'm guessing components can enumerate their
			subcomponents so that an abbreviation file
			seemingly merely listing computer names within
			computer names, actually defines the structure
			of the solution to a complex problem.  These
			names are specified in lots of problem
			specific abbreviation files, which I gathered
			together here, for now.  Maybe a better place
			or use can be found...

data-files/		I have no idea what these data files describe.  

empty-files/		I'd delete all these but maybe something depends on their
			existence, despite their having nothing in them.

generated-csh/		A million small csh programs, perhaps auto-generated.a

generated-html/
html-files/		Joe's Web Of Opinions are found in these .html files.
			Dismiss nothing lightly; he has thought deeply.

log-files/		Some of these are outputs recording compute jobs,
			some might actually be inputs but aren't clearly labelled.
			I couldn't extract much usefulness from them since
			I don't know the questions much less the outline of the
			answers.

			Next are directories containing lots of files with names
			sharing the same prefix, eg., m071??.  Probably they
			are related to the same project(s).  Many are similar,
			perhaps they are different runs with slightly different
			data, trying to get better answers to the same problem.
			Myself, I'd have to be pretty bored and open minded to get
			very deep into these.

ed-files/		A guess: mostly stored editor command sequences like emacs macros)
m071-files/		gcc headers and libraries for a system-specific compilation project.
mc1-files/		Files relating to a Liquid Metal Reactor modelling project.
na-files/		na1*, nai* might be different projects.
op1-files/		JAPAN NUCLEAR CRISIS, pongfu, etc.
opi-files/		??
or-files/		ORIGEN
pf1-files/		pongfu, mostly, I think.

media-files/		I did the sorting of files here in bash and emacs, so I 
			didn't see, but moved to here, all the files I couldn't read.

scripts/		Executeable scripts, mostly of the csh variety, for local
			convenience within Joe's then-available
			computing environment.  Lots of scripts to put
			files onto ftp servers, to run other programs; Joe's
			bashrc and profile are also here.

perl-scripts/		The scripts written in Perl are here, doing a lot of the
			same stuff as the csh scripts above.  But see e.g., addlin
			which seems to generate structured html files.  

pongfu-files/		Files related to Joe's interest in table tennis mechanics.

nuclear-files/		I haven't put these on github.

so.libraries/
binaries/		Some programs are needed to build robacus like gcc, f2c, etc.
			Last time robacus worked it was in mageia, a linux variety,
			which it seems pointless to reconstruct.  Instead let's try
			to build it with modern toolchains; that's the whole point of
			a github project! Therefore I have not posted these
			out-of-date binaries and libraries, which are quite likely
			to not work in a modern system (I get "exec format error"
			in Ubuntu on Windows.)  
