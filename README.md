


# STACKOVERFLOW 

### Context

- Stack Overflow is the largest online community for programmers to learn, share their knowledge, and advance their careers.

### Inspiration



What is the percentage of questions that have been answered over the years?

What is the reputation and badge count of users across different tenures on StackOverflow?

What are 10 of the “easier” gold badges to earn?

Which day of the week has most questions answered within an hour?


### Content

- Updated on a quarterly basis, this BigQuery dataset includes an archive of Stack Overflow content, including posts, votes, tags, and badges. 
- This dataset is updated to mirror the Stack Overflow content on the Internet Archive, and is also available through the Stack Exchange Data Explorer.


Fork this kernel to get started with this dataset.

Acknowledgements

Dataset Source: https://archive.org/download/stackexchange

https://bigquery.cloud.google.com/dataset/bigquery-public-data:stackoverflow

https://cloud.google.com/bigquery/public-data/stackoverflow

Banner Photo by Caspar Rubin from Unplash.


# JULIA 

## WHY JULIA?

- Julia is relatively new high-level free/open-source language for numerical computing in the same spirit, with a rich set of built-in types and libraries for working with linear algebra and other types of computations, with a syntax that is superficially reminiscent of Matlab's. 
- Basically, we are using Julia because, unlike Matlab or Python or R, it scales better to real computational problems — you can write performance-critical "inner loops" in Julia, whereas similar tasks in other high-level languages often require one to drop down to C or similar low-level languages.
- Julia is a high-level dynamic programming language designed to address the needs of high-performance numerical analysis, and scientific computing is rapidly gaining popularity amongst the data scientists. 
- It is a newer language, also capable of general purpose programming as well and hasn’t been around as long as R or Python.
- Due to its faster execution, Julia has become a perfect choice for dealing with complex projects containing high volume data sets. For many basic benchmarks run 30 times quicker than Python and regularly run somewhat quicker than C code. 
- If you like Python’s syntax while you have a massive amount of data, then Julia is the next programming language to learn.
- A joint effort between Jupyter and Julia communities, it gives a fantastic program based graphical notebook interface to Julia. People, who are searching for the best performance parallel computing language focused on numerical computing, Julia is a perfect language for them.


## UTILIZING JULIA 
- We thank you for being a Julia user. Julia Computing has decided to sunset JuliaBox on May 31, 2020. If you are a paid JuliaBox user, you will no longer be able to log in and you will not be charged for JuliaBox after that date. 
- An alternative is to download the JuliaPro package, which includes Julia, IJulia, the Juno IDE based on the Atom editor, and a number of packages pre-installed.


## ECOSYSTEM 


### General Purpose

Build, Deploy or Embed Your Code
Julia lets you write UIs, statically compile your code, or even deploy it on a webserver. It also has powerful shell-like capabilities for managing other processes. It provides Lisp-like macros and other metaprogramming facilities.

Julia has foreign function interfaces for C/Fortran, C++, Python, R, Java, and many other languages. Julia can also be embedded in other programs through its embedding API. Specifically, Python programs can call Julia using PyJulia. R programs can do the same with R's JuliaCall, which is demonstrated by calling MixedModels.jl from R.

### Data Science

Interact with your Data
The Julia data ecosystem lets you load multidimensional datasets quickly, perform aggregations, joins and preprocessing operations in parallel, and save them to disk in efficient formats. You can also perform online computations on streaming data with OnlineStats.jl. Whether you're looking for the convenient and familiar DataFrames, or a new approach with JuliaDB, Julia provides you a rich variety of tools. The Queryverse provides query, file IO and visualization functionality. In addition to working with tabular data, the JuliaGraphs packages make it easy to work with combinatorial data.

Julia can work with almost all databases using JDBC.jl and ODBC.jl drivers. In addition, it also integrates with the Hadoop ecosystem using Spark.jl, HDFS.jl, and Hive.jl.

### Juno IDE

A flexible IDE for the 21st century

Juno provides the flexibility of a traditional IDE with the convenience of a notebook in a hybrid canvas programming style. It includes a number of powerful editing features such as auto-completion, real-time feedback, unicode symbols and operators, to name a few. Juno is an extension to the popular Atom editor with all the capabilities provided by Atom. More details about Juno can be found at junolab.org.


### Machine Learning
Scalable Machine Learning
Julia provides powerful tools for deep learning (Flux.jl and Knet.jl), machine learning and AI. Julia’s mathematical syntax makes it an ideal way to express algorithms just as they are written in papers, build trainable models with automatic differentiation, GPU acceleration and support for terabytes of data with JuliaDB.

Julia's rich machine learning and statistics ecosystem includes capabilities for generalized linear models, decision trees, and clustering. You can also find packages for Bayesian Networks and Markov Chain Monte Carlo.

### Parallel Computing

Parallel and Heterogeneous Computing
Julia is designed for parallelism, and provides built-in primitives for parallel computing at every level: instruction level parallelism, multi-threading and distributed computing. The Celeste.jl project achieved 1.5 PetaFLOP/s on the Cori supercomputer at NERSC using 650,000 cores.

The Julia compiler can also generate native code for various hardware accelerators, such as GPUs and Xeon Phis. Packages such as DistributedArrays.jl and Dagger.jl provide higher levels of abstraction for parallelism.


### Plotting
There are several plotting packages available for Julia. 
If you followed the installation instructions, above, you already have one full-featured Matlab-like plotting package installed: PyPlot, which is simply a wrapper around Python's amazing Matplotlib library.
- There are several plotting packages available for Julia. If you followed the installation instructions, above, you already have one full-featured Matlab-like plotting package installed: PyPlot, which is simply a wrapper around Python's amazing Matplotlib library.

### Scientific Domains

Rich Ecosystem for Scientific Computing
Julia is designed from the ground up to be very good at numerical and scientific computing. This can be seen in the abundance of scientific tooling written in Julia, such as the state-of-the-art differential equations ecosystem (DifferentialEquations.jl), optimization tools (JuMP.jl and Optim.jl), iterative linear solvers (IterativeSolvers.jl), a robust framework for Fourier transforms (AbstractFFTs.jl), a general purpose quantum simulation framework (Yao.jl), and many more, that can drive all your simulations.

Julia also offers a number of domain-specific ecosystems, such as in biology (BioJulia), operations research (JuliaOpt), image processing (JuliaImages), quantum physics (QuantumBFS, QuantumOptics), nonlinear dynamics (JuliaDynamics), quantitative economics (QuantEcon), astronomy (JuliaAstro) and ecology (EcoJulia). With a set of highly enthusiastic developers and maintainers from various parts of the scientific community, this ecosystem will only continue to get bigger and bigger.

### Visualization 

Data Visualization and Plotting
Data visualization has a complicated history. Plotting software makes trade-offs between features and simplicity, speed and beauty, and a static and dynamic interface. Some packages make a display and never change it, while others make updates in real-time.

Plots.jl is a visualization interface and toolset. It provides a common API across various backends, like GR.jl, PyPlot.jl, and PlotlyJS.jl. Users who prefer a more grammar of graphics style API might like the pure Julia Gadfly.jl plotting package. VegaLite.jl provides the Vega-Lite grammar of interactive graphics interface as a Julia package. For those who do not wish to leave the comfort of the terminal, there is also UnicodePlots.jl.

# CASSANDRA

## Tell Me About Cassandra

* Cassandra, or more specifically [Apache Cassandra](https://cassandra.apache.org), is an open-source distributed NoSQL database.  Cassandra delivers outstanding performance due to its distributed node design.  
* This design leads to a linear increase in both read and write performance as more nodes are added.  
* Another benefit to the design is that each node is identical because data is replicated across all nodes, meaning no single node represents a point of failure.  
* Based on Cassandra’s design, the CAP theorem would indicate that Cassandra focuses on the A and P guarantees – A for Availability and P for Partition tolerance – while sacrificing Consistency.

<< CAP THEOREM DIAGRAM>> 

* Cassandra shares some design qualities with popular NoSQL databases such as [Amazon’s DynamoDB](https://aws.amazon.com/dynamodb/) and [Google’s Big Table](https://cloud.google.com/bigtable/). 
* Cassandra is a Column store database like Google’s Big Table.  

[KUBERNETES.md](https://github.com/joemccann/dillinger/blob/master/KUBERNETES.md)

- However, Cassandra is also similar to Amazon’s DynamoDB in that it uses a key-value system in which the keys point to column families that represent the structure of the stored data.  
- Unlike Big Table and DynamoDB, Cassandra takes a different approach to query its data.  Cassandra employs a query language that shares many similarities to SQL called the Cassandra Query Language.  CQL helps ease the onboarding of developers who are already familiar with SQL with.  Let’s take a look at the CQL syntax.


In computer programming, create, read, update, and delete[1] (CRUD) are the four basic functions of persistent storage.[2] Alternate words are sometimes used when defining the four basic functions of CRUD, such as retrieve instead of read, modify instead of update, or destroy instead of delete. CRUD is also sometimes used to describe user interface conventions that facilitate viewing, searching, and changing information; often using computer-based forms and reports. 





# TABLEAU

