# Apophenia-Engine
Home of an evovling history generation tool for fictional nations. Presently, it only works for fantasy worlds, but can accomidate any fantasy world with any level of magic.

The Apophenia Engine is a semi-procedural semi-random text generation program which creates histories for fictional univerces. It creates many files, the most important of which are the timeline.csv and the worldhistory.rtf. In leyman's terms, once configured for a world and run, this program creates a spreadsheet with a timeline of history in the form of short blurbs of what happened in a given year, and a much longer document detailing the events in full, with cultural and political information for reach nation included. It also creates many other helpful files which both drive the program's choices and decisions, and also serve as lists of what each nation has for your future needs.

It also creates a multi-paragraph preocedualy generated descripotion of every major settlment within the nation. These get unique names created via a markov chain-liek process with the names being appropriate to the culture that founded the settlment. This is achieved by the creation of langauge files which get tagged with cultures/species.

The program works in 50 year cycles, as this is a good chunk of time to focus on to get a few important historicla figures and see a generation grow up, have children, and retire. The program reads from a list of supplied nations, and will generate 50 years of events for them, with the number of events per cycle fully configerable by you. It only generates the events which are ment to be big important things that shaped the nation or culture. Many things are possible at present, including natural disasters, the founding of new towns, the discovery of new kingdoms, making new friends, making new enamies, discovering fantastical materials and creatures, the creation of regions each nation owns, and more.

These generated moemtns in history are very basic by design. They give you a who, what, and when, but are not too specific. This is to allow you to use each generated moment as a writing prompt if/when you want to expand on that event.

There are some limts. Presently, the program cannot generate events involving more than one nation at a time. There are some bugs in the code I have not yet been able to find, so sometimes a veriable will not update resulting in odd generations (these can be easily fixed by manualy editing the output file and do not effect generation other than putting the wrong word somewhere, as far as I can tell). As I only know Batch, this is written in Batch and thus is slow and only runs on windows (I would be intrested in being shown how to make parts of this program in python. I do not want to learn all of python, as I have no intrest in anythign but this type of text generation. I will happily learn the Python needed for this, but I cannot find tutorials for just this sort of thing).

Generating a history starting with 7 nations and spanning 5 cycles takes ~15 minutes on my computer, which uses an AMD Ryzan 5 3600. The first cycle takes substancial longer than subsequent cycles as the first cycle a nation exists within requires the program generate a lot of supporting information for the nation. Up to three new nations can be created per cycle, this is to slow the rate at which the program coudl otherwise expodentialy grow in terms of time per cycle.

The most major limitation of the program is the random crash I have yet to lock down. The Apophenia Engine can resume generation after a crash, but it cannot resume from anywhere other than the beginning of a cycle (I may be able to improve this). This mean sif it crashes, you can simply continue from the start of the cycle after the one it crashed on. I may shortly update the program so you can erace the generated history from the partialy compleat cycle, and recreate everything that happened then if you so wish.

Feedback, advice, tips, and assistance with this project are more than welcome. If you develop anything that works with it, please let me know. It's designed in a way to be infintly expandable.
