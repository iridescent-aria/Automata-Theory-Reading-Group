---
aliases:
---
# Basic Automata Theory Crash Course

- Intent: introduce first years to basic ideas in automata theory, revise this stuff for anybody else who wants it as well.
- Time: 1 hr

Material:
- What is TCS?
	- Formal mathematical models of computers
	- What can we / can't we compute?
	- Decision problems as languages, machines as deciding membership in a language
- Why automata?
- What is an automaton?
	- Lots and lots of examples
	- DFAs - _regular_ languages
	- Certain specific patterns are the regular languages; looking at this more language theoretically / syntactically gives us regular expressions
	- These two are the same - no proof though :(
	- DFAs = constant space decision algorithms. Explain this connection.
- Graph theoretic properties
	- Reachability, universality
	- Pumping lemma
- Nondeterminism
	- _Makes guesses_.
	- NFAs: same thing except with nondeterminism
	- Example use-cases: maze solving, reachability in (x3, /2) system
	- Aside: P vs NP is this.
	- Amazing fact: NFAs = DFAs.
		- Will prove this: call on the intuition of constant space programs.
		- Especially use the above problems (the problems are reachability in 'large' systems, the NFA -> DFA thing is just reachability in 'small' systems)
- Myhill-Nerode and minimal automata
	- DFAs / regular languages are very finite objects
	- When you're in a state in a DFA / constant space program, the rest of your behavior is entirely determined
	- So if two words reach the same state, they will have the same behavior afterwards as well.
	- Define an equivalence!
	- Can do this language theoretically as well
	- The point: a language is regular iff its MN equivalence has finitely many classes (exercise, but the point is to motivate the equivalence enough that this is an easy exercise).
- Conclusion and Verification
	- Recap
	- Verification: make a model of the program (which is often some type of automaton) and check reachability and such things


# List of Potential Topics

- Automata Models (Shubh)
	- AFAs
	- 2NFAs
	- PDAs
	- Turing Machines
- Intro to timed automata (ask Srivathsan?)
	- Intent: this is a fun model to work with that also has a lot of practical uses
- Automata and monoids (Arnab potentially)
	- Intent: intro to algebraic automata theory
- Tree automata
	- Intent: I just want to know what these are lol
- Concurrency and Automata
	- Intent: intro to concurrency via fun automata theory
- Automata Learning 1 (me probably):
	- Intent: present Angluin's $L^{*}$ algorithm and show that learning automata is a thing
- Literally Everything is Regular
	- Intent: Show that there are so, so, so many characterizations of regular languages
	- Material:
		- Recap: DFAs, NFAs, regexes, MN-equivalence, all characterize regular languages
		- Alternating automata are regular
		- 2-way NFAs are regular
		- MSO describes regular languages
- VASSes (Shubh or me probably)
	- Intent: introduce people (maybe targeted at PhDs and faculty) to VASSes, survey results / ideas and show that these things are simple but super hard to work with

- Intro to Logic
	- Intent: introduce logic to first years / others who haven't had a formal intro to logic

- Logic and Automata
	- Intent: applications of logic / system specification type ideas to automata
	- Material:
		- Logic as a way to specify properties
		- How do we specify automata with this language?
		- MSO and FSMs
		- LTL and Buchi automata
		- (probably too much but) MTL / MITL and TAs