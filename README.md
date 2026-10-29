# Hi there 👋 I'm Massimo Nocentini

I'm a researcher and software developer from Tuscany, Italy, with a PhD in Computer Science from the
[University of Florence](https://www.unifi.it/). I work on graph algorithms and large-scale network
analysis, and I spend a lot of time with programming languages: Scheme, Smalltalk, Lua, Rust and C.

- 🌐 Homepage and blog: **[massimo-nocentini.github.io](https://massimo-nocentini.github.io/)** ([RSS](https://massimo-nocentini.github.io/index.xml))
- 📄 Curriculum vitae et studiorum: [online](https://massimo-nocentini.github.io/about/), [LaTeX sources](https://github.com/massimo-nocentini/curriculum-vitae)
- ✉️ massimo.nocentini@gmail.com · massimo.nocentini@unifi.it

## What I work on

- **Graphs and networks.** Research fellow at [DiSIA](https://www.disia.unifi.it/) (2024–2026, *Graphs and applications*, with Prof. Andrea Marino):
  graph models of the Bitcoin transaction network, algorithms for graphs with large diameter, and crowding estimation
  in public transport via temporal graphs.
- **Relational and logic programming.** µKanren and miniKanren in Python, Smalltalk and Scheme, plus
  *Kanren Light*, a logic programming system built on HOL Light (with Prof. Marco Maggesi).
- **Combinatorics.** My PhD (2019, advisor Prof. Donatella Merlini) studied Riordan arrays,
  generating functions and the OEIS, with symbolic and logic tools.
- **Software development.** Freelance since 2019 on Pharo Smalltalk and microservice architectures. Before that I spent
  years in industry on .NET, C# and PostgreSQL.

## Publications

- A. Bernasconi, D. Di Francesco Maesa, M. Loporchio, A. Marino, **M. Nocentini**, L. Ricci.
  [*Systematizing Graph Models for Bitcoin and Designing Algorithms for Large-Distance Analysis*](https://doi.org/10.1109/TNSE.2026.3743291),
  IEEE Transactions on Network Science and Engineering, 2026.
- D. Bubboloni, C. Catalano, M. Fanfani, A. Marino, P. Nesi, **M. Nocentini**.
  *Public Transport Crowding Estimation via Temporal Graphs*, submitted.
- M. Maggesi, **M. Nocentini**. *Kanren Light: A Dynamically Semi-Certified Interactive Logic Programming System*,
  miniKanren 2020 workshop ([code](https://github.com/massimo-nocentini/kanren-light)).
- D. Merlini, **M. Nocentini**. [*Functions and Jordan canonical forms of Riordan matrices*](https://doi.org/10.1016/j.laa.2018.12.011),
  Linear Algebra and its Applications 565, 2019.
- D. Merlini, **M. Nocentini**. [*Algebraic generating functions for languages avoiding Riordan patterns*](https://cs.uwaterloo.ca/journals/JIS/VOL21/Merlini/merlini5.html),
  Journal of Integer Sequences 21, 2018.
- **M. Nocentini**, D. Merlini. *Crawling, (pretty) printing and graphing the OEIS*, DiSIA working paper, 2018
  ([code](https://github.com/massimo-nocentini/oeis-tools)).

Theses: [PhD](https://github.com/massimo-nocentini/PhD-thesis) ([defense slides](https://github.com/massimo-nocentini/massimo-nocentini.github.io/releases/download/PhD-defense/talk.pdf)),
[master](https://github.com/massimo-nocentini/master-thesis) (*Patterns in Riordan arrays*).

## Selected projects

**Graphs, in Rust and C**
- [igraph-rs](https://github.com/massimo-nocentini/igraph-rs): Rust bindings for [igraph](https://igraph.org/) ([post](https://massimo-nocentini.github.io/post/2026-01-12-igraph-rust-bindings/))
- [webgraph-clib-rs](https://github.com/massimo-nocentini/webgraph-clib-rs): a C library over [webgraph-rs](https://github.com/vigna/webgraph-rs) compressed graphs;
  [webgraph-foreign-algorithms-rs](https://github.com/massimo-nocentini/webgraph-foreign-algorithms-rs) runs igraph and rustworkx algorithms on them
- [avgdist-rs](https://github.com/massimo-nocentini/avgdist-rs): a sampling algorithm to estimate the average distance in graphs with a large diameter
- [utxo2webgraph-rs](https://github.com/massimo-nocentini/utxo2webgraph-rs), [utxoscope-rs](https://github.com/massimo-nocentini/utxoscope-rs): Bitcoin UTXO graphs ([post](https://massimo-nocentini.github.io/post/payments-graph/))
- [dag-rs](https://github.com/massimo-nocentini/dag-rs): DAG algorithms (semiring DP, dominators, reachability, transitive reduction, width) on webgraph DAGs,
  validated on the Bitcoin Payment Graph (2.18·10⁹ nodes, 8.64·10⁹ arcs)
- [coloring-bt-transactions-rs](https://github.com/massimo-nocentini/coloring-bt-transactions-rs): where did a Bitcoin transaction's coins come from? Colouring transactions by the blocks they descend from ([docs](https://massimo-nocentini.github.io/coloring-bt-transactions-rs/))
- [graph-tool-rs](https://github.com/massimo-nocentini/graph-tool-rs): a work-in-progress Rust port of [graph-tool](https://graph-tool.skewed.de), moving its runtime failures to compile time
- [non-layered-tidy-trees.c](https://github.com/massimo-nocentini/non-layered-tidy-trees.c): drawing non-layered tidy trees in linear time, also [in Rust](https://github.com/massimo-nocentini/non-layered-tidy-trees-rs)
- [libpq-rs](https://github.com/massimo-nocentini/libpq-rs), [judy-rs](https://github.com/massimo-nocentini/judy-rs): bindings for PostgreSQL's libpq ([post](https://massimo-nocentini.github.io/post/2026-01-23-libpq-rs/)) and Judy arrays

**Scheme and relational programming**
- [aux.scm](https://github.com/massimo-nocentini/aux.scm): auxiliary definitions and macros for CHICKEN Scheme (streams, nondeterminism, [HANSEI](https://massimo-nocentini.github.io/post/2026-02-05-scm-testsuite-hanseitest/), monads, unit testing),
  now with λProlog-style higher-order logic programming in µKanren (`(aux kanren lambda)`) and ports of
  Pie from *The Little Typer* and J-Bob from *The Little Prover*; its test suites are [on the blog](https://massimo-nocentini.github.io/categories/scheme/)
- [concurrent.scm](https://github.com/massimo-nocentini/concurrent.scm): Concurrent ML for CHICKEN Scheme ([post](https://massimo-nocentini.github.io/post/cml/))
- [wolfram.scm](https://github.com/massimo-nocentini/wolfram.scm): talking to the Wolfram Engine from Scheme
- [microkanrenpy](https://github.com/massimo-nocentini/microkanrenpy), [microkanrenst](https://github.com/massimo-nocentini/microkanrenst), [kanren-light](https://github.com/massimo-nocentini/kanren-light): µKanren in Python, Smalltalk and OCaml/HOL Light

**Pharo Smalltalk**
- [pharo-vm](https://github.com/massimo-nocentini/pharo-vm/tree/pharo-12): a fork of the Pharo 12 VM with a WebAssembly port that runs stock Pharo 12–15 images
  in node and [in the browser](https://massimo-nocentini.github.io/pharo-vm/) (console, notebook, Morphic world, Iceberg over libgit2),
  a SimdJSONPlugin with drop-in replacements for NeoJSON's reader and writer, and faster LargeIntegers ([post](https://massimo-nocentini.github.io/post/smalltalk/))
- [Containers-*](https://github.com/massimo-nocentini?tab=repositories&q=Containers-&language=smalltalk): persistent and classic data structures
  (skip lists, splay, leftist and binomial heaps, red-black sets, union-find, [SBRAL](https://massimo-nocentini.github.io/post/sbral/), …),
  collected in the [Booklet-DSst](https://github.com/massimo-nocentini/Booklet-DSst) booklet
- [srfi-41st](https://github.com/massimo-nocentini/srfi-41st) (streams), [delimcc.st](https://github.com/massimo-nocentini/delimcc.st) (delimited continuations),
  FFI bindings to [Lua](https://github.com/massimo-nocentini/liblua.st), [tree-sitter](https://github.com/massimo-nocentini/libtreesitter.st), [Wolfram](https://github.com/massimo-nocentini/wolfram.st) and [poppler](https://github.com/massimo-nocentini/libpoppler.st)

**Knuth, literate programming and Lua**
- [sgb.cweb](https://github.com/massimo-nocentini/sgb.cweb), [bdd-zdd.cweb](https://github.com/massimo-nocentini/bdd-zdd.cweb), [SAT.cweb](https://github.com/massimo-nocentini/SAT.cweb), [simpath.cweb](https://github.com/massimo-nocentini/simpath.cweb): working through Knuth's programs ([post](https://massimo-nocentini.github.io/post/2026-01-25-sgb/))
- [exactcover.lua](https://github.com/massimo-nocentini/exactcover.lua) (dancing links), [toposort.lua](https://github.com/massimo-nocentini/toposort.lua), and Lua bindings for [curl](https://github.com/massimo-nocentini/curl.lua), [cairo](https://github.com/massimo-nocentini/cairo.lua) and [PostgreSQL](https://github.com/massimo-nocentini/pgsql.lua)

## Talks

- *Dancing Links: an educational pearl*, [ESUG 2019](https://esug.github.io/2019-Conference/conf2019.html), Cologne
- *Relational Programming in Smalltalk*, ESUG 2018, Cagliari ([slides](https://github.com/massimo-nocentini/microkanrenst/releases/download/v1.0/esug.pdf))
- *Modular Catalan triangle*, 2nd International Symposium on Riordan Arrays and Related Topics, 2015, Lecco
