# Software developed by RIKEN R-CCS

RIKEN R-CCS ([http://www.r-ccs.riken.jp/en/](http://www.r-ccs.riken.jp/en/)) is a research center for computational science and computer science for simulations with supercomputers. Some software developed by RIKEN R-CCS are hosted by GitHub.  (RIKEN R-CCS is formerly named as RIKEN AICS, renamed in April 2018).

Some projects have independent GitHub organizations (incomplete list):
* [Fiber Miniapp Suite](http://fiber-miniapp.github.io)
* [https://github.com/avr-aics-riken](https://github.com/avr-aics-riken)
* [https://github.com/pf-aics-riken](https://github.com/pf-aics-riken)
* [Evidence-Based performance Tuning (EBT-HPC)](https://github.com/ebt-hpc)
* [https://github.com/crest-cassia](https://github.com/crest-cassia)
* [XcalableMP Specification](https://github.com/XcalableMP/Specification)
* [Omni compiler](https://github.com/omni-compiler/omni-compiler)
* [Extrae](https://github.com/bsc-performance-tools/extrae) 

The projects under RIKEN-RCSS:

{% for repository in site.github.public_repositories %}
  * [{{repository.name}}]({{repository.html_url}}): {{repository.description}}
{% endfor %}

## Incomplete list of software developed by RIKEN R-CSS (including software just ported to K computer)

|Name|Description|
|----|----|
|Carp|Carp is software to parallelize computation for any possible combination of two records in dataset. The software users do not need to write any parallel program, but write just sequential programs. All parallelizing tasks are done by the Carp software.|
|EARTH on K|EARTH on K is a derivative version of EARTH (Effective Aggregation Rounds with Throttling) optimization framework towards high performance MPI-IO. EARTH on K is optimized to achieve high performance MPI-IO using a local file system (LFS) of the K computer.|
|NetCDF|NetCDF is a set of software libraries and self-describing, machine-independent data formats that supports the creation, access, and sharing of array-oriented scientific data. We provide NetCDF library and related libraries (HDF5, Parallel netCDF and Szip) on the K computer compute hosts and frontends.|
|PRDMA （Persistent Remote DMA）	|The PRDMA library provides a fast implementation of MPI Persistent Communication primitives to reduce the communication latency and to improve the overlap between computation and communication over an RDMA-enabled interconnect.|
|MUMPS|MUMPS(MUltifrontal Massively Parallel sparse direct Solver) is a package for solving sparse linear systems using the direct method. MUMPS supports MPI parallel procedures.|
|Omni compiler|Omni compiler is a compiler for parallel programming languages XcalableMP, XcalableACC, OpenACC.|
|Scalasca|Scalasca is a software tool that supports the performance optimization of parallel programs by measuring and analyzing their runtime behavior. The analysis identifies potential performance bottlenecks - in particular, those concerning communication and synchronization – and offers guidance in exploring their causes.|
|EigenExa|EigenExa is a high performance eigenvalue solver, which is developed as a successor of EigenK. It is tuned up on the K computer. As EigenK does, EigenExa also solves a standard eigenvalue problem for a dense real symmetric matrix, and it performs very fast even with large-scale parallel computations and small scale problems.|
|EigenK|EigenK is an eigenvalue solver, which is developed to work on the K computer efficiently. EigenK solves a standard eigenvalue problem for a dense real symmetric matrix. EigenK performs large-scale parallel computation and small scale problem faster than the existing eigenvalue solvers do.|
|KMATH_RANDOM|A library of random number generator by the Mersenne Twister, a high-quality pseudorandom number generator, for a distributed parallel processing environment. Available for Fortran 90, C, and C++.|
|CCA/EBT (Code Comprehension Assistance for Evidence-Based performance Tuning)|For improving the performance of an application, we have to comprehend the application's source code. In order to facilitate comprehension of source code written in Fortran, this utility analyzes its syntactic/semantic structures and then provides outline views of loop-nests and call trees decorated with source code metrics.|
|Extrae|Extrae is the package devoted to generate Paraver trace-files for a post-mortem analysis. MPI applications written in Fortran, C, or C++ can be analyzed in detail using the trace files with Paraver.|
|Eclipse PTP for K and FX10 computers|This software is necessary for using Eclipse PTP IDE with K and FX10 computers. It consists of 2 packages:(1) Target System Configurations necessary for submitting jobs to K and FX10 computers, (2) LML DA Driver for PJM to be installed on K and FX10 user home directory to enable Eclipse PTP monitoring feature.|
|TAU|TAU Performance System is a portable profiling and tracing toolkit for performance analysis of parallel programs written in Fortran, C, C++. It supports performance instrumentation, measurement, analysis and visualization. Application profiles show the exclusive and inclusive time spent in each function, how many times each function was called, how many profiled functions did each function invoke, and what the mean inclusive time per call was. Application traces show when and where event occured in terms of the process that executed it and the location in the source code.|
|Xcrypt|Xcrypt is a scripting language that enables us to easily write a script to manage a number of concurrently running jobs. It provides a unified interface that handles differences in system interfaces of various supercomputers ; users do not need to learn each interface. Furthermore, Xcrypt has a mechanism that allows users to add various useful features as modules ; some important features are integrated in Xcrypt as standard modules.|
|OACIS (Organizing Assistant for Comprehensive and Interactive Simulations)|OACIS runs as a web server on Mac or Linux to manage simulation executions and their results. After a user sets simulation parameters, OACIS creates shell script files for these parameters and submits them to the specified remote hosts. After these jobs are finished, the results are automatically downloaded and stored in the specified directory.|
|NTChem|NTChem is a high-performance software package for the molecular electronic structure calculation for general purpose on the K computer. It is a comprehensive new software of ab initio quantum chemistry made in AICS from scratch. NTChem contains not only standard quantum chemistry approaches but also our own original approaches. NTChem is expected to be a useful tool in various computational studies for large and complicated molecular systems. |
|2D-DMRG	|The 2D-DMRG is developed to study quantum lattice systems. The 2D-DMRG is optimized to perform high performance massively parallel computings on the K-computer. Although the DMRG method is used to study one-dimensional systems, the 2D-DMRG can be used for higher dimensional systems. Also, the 2D-DMRG can be employed to investigate an arbitrary shape of systems and many kinds of quantum lattice models. *Website is in Japanese|
|GENESIS	|GENESIS is a high performance molecular dynamics and modeling software. It consists of two simulators, ATDYN and SPDYN. SPDYN shows high speed and good scalability on massively parallel computers. ATDYN is capable of multi-scale simulations using coarse grained models and all atom models. Generalized ensemble simulations including replica-exchange molecular dynamics and replica-exchange umbrella sampling methods are available.|
|FDPS (Framework for Developing Particle Simulators)	|FDPS is an application-development platform. It helps researchers to develop software for particle simulations which run efficiently on massively parallel computers such as K computer. By using FDPS, researchers without much experience in tuning or parallelization can develop applications which run efficiently on tens of thousands of nodes.|
|SCALE	|A Library for weather and climate simulations, and an atmospheric large-eddy simulation model using the library. These are developed with co-design by researchers of computational and computer sciences to achieve high performance in massive parallel computer systems.|
|Apache Spark	|Spark is a big data processing framework developed by Apache Software Foundation. It has been built to use on K computer as well as R language on K computer. The installation also includes scripts to use Spark as a job on K.|
|KMR (K Map-Reduce)	|KMR（K Map-Reduce）is a high-performance map-reduce library designed to ease programming on data processing on the K computer. It is based on the popular framework in the cloud computing, but its execution is much efficient by exploiting the power of supercomputers.|
|llvm-sparc64fx	|Patched LLVM compiler for using Fujitsu extensions of SPARC64.|
|CIOlib	|This CIO library provides following functions for the Cartesian structured data.- Management of distributed files - Restart from previous calculated data (standard) - Restart from previous calculated data of the number of different process - Restart from previous coarse data with interpolation - Staging helper - File converter utility|
|CPMlib	|CPMlib is a C++ class library to efficiently assist the development of unsteady physical simulators. This library provides functions such as the management of partitioned subdomains by domain decomposition method and wrapper functions for neighbor and global communications.|
|Cutlib	|This Cut Information library provides functions to calculate intersection between polygon face and background grid, and to manage generated information. Both Cartesian and Octree grid data structure can be utilized for the background grid. Previous version is available as public software.|
|FFV-C	|FFV-C is a 3D unsteady thermal flow simulator developed to execute high- performance simulation of fluid flow around complex geometries by using Cartesian grid. One of the major features of this simulator is the automation of the grid generation process, widely recognized as a difficult task in fluid flow analysis, which makes it possible to reduce considerably the large-scale simulation time. Another worth noting feature is the fine-tuning implementation which contributes for a weak scaling performance of over 90%, using the full computational nodes of the K computer. The FFVC has continuously being developed to aggregate functionalities for assisting real-world design tasks in the engineering fields.|
|HIVE	|HIVE is a visualization framework designed to be user-friendly, functional and convenient in a highly parallel environment. It can perform parallel rendering using multiple nodes on the K computer. It is being developed to be portable to many different computing platforms, be capable of executing in both local and remote mode, be highly scalable, be flexible for aggregating new functionalities, and be easily portable and maintainable. It is currently available as a Beta version for Mac and Linux in the binary package format.|
|KFoundation	|A collection of original general-purposed C++ APIs, developed at AICS. Included APIs are: (1) Automatic memory management with flat time-complexity performance, and enhanced stability and debugging features; (2) Object serialization/deserialization API that turns enabled objects to and from XML, JSON, etc.; (3) Broad range of I/O streams including network I/O;  (4) Multi-level multi-channel logger; (5) Exceptions with printable/serializable stack trace; (6) Range Arithmetic for facilitation of distributed stencil computation, (7) Thread, Mutex, Condition and Java-like System classes.|
|libKnoRBA	|C++ library for creating KnoRBA agents. The Knowledge Request-Broker Architecture or KnoRBA technology is the world’s first distributed programming environment that uses “agent” in place of “object” as general-purposed programming component model. Its purpose is to offer a higher level of abstraction, and with it higher autonomy, portability, flexibility, extensibility, and stability. Agents created using this library can be executed using KnoRBA Agent Runtime Environment (ARE) on a cluster or any distributed system.|
|PMlib	|This Performance Monitor library records arithmetic performance of a user code during its execution and reports the summary. The PMlib is able to use for both serial and parallel environments including hybrid (OpenMP & MPI) code.|
|Polylib	|Polylib is a C++ class library to keep and to manage polygon data, and has following functions: - Load and save polygon data. The file format is STL - Management of polygon data on distributed parallel environment - Search and retrieve polygon data - Grouping by input parameter file (text parser format) - Data movement and migration between subdomains|
|TextParser	|Text Parser library enables us to handle YAML like simple parameter structure instead of a heavy XML parsing library.|
|K-scope	|K-scope is a source code analysis tool with graphical user interface for Fortran 90 and FORTRAN 77, which visualizes program structures such as loop, branch and procedure call as bottleneck. By the K-scope, application performance engineer can understand overview of source codes for starters. (This software is Java application for Commodity-PC, not the K-computer.)|
|Performance Analysis tool by once, "1PAtool"	|This software is the tool on the K computer to display the results of the basic performance analysis and time breakdown analysis that are output as profile results by Precision PA visibility function.|
|Waiting for the K	|This tool calculates a waiting time of a job on the K computer.|
