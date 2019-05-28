The BabyBench is the 'hello-world' example to demonstrate and test the functionality of SQALPEL. It is based on the [TPC-H](tpc.org) benchmark defined by the Transaction Processing Counsel. Babybench uses the rather limited scale-factor 1, which means a database of about 1GB. The results we get from running experiments on such a tiny database is **not** indicative for the performance when we scale up to a multi -GB database.
#### Database schema
The database is described in TPC-H. Beware that most database systems use a slightly different type system and syntax. Being aware of the consequences in terms of performance is crucial

##### Auxiliary structures
To speed up processing of database queries, a good choice of search accelerators may help.

#### Baseline queries
The 22 TPC-H queries cover a wide spectrum of functionality. Often Q1 and Q6 are used to assess raw performance of a system in distributed settings. It merely requires a fast scan following by aggregation to just a few   tuples. Q13 is of interest, because it relies on string matching. An often overlooked functionality requirement and a good target to use special instructions. In the experiments reported, you will notice which queries are a  tumbling stone.

#### Evaluation context
The results assembled in for BabyBench project are purposely limited to 'out-of-the-box' use of database systems on a  common desktop platform. That is, no special arrangements are made beyond those commonly used. For example, indices are not created upfront,  system properties are aligned with the host environment,

#### Hardware platforms
The experiments are all ran on the same hardware platform, an Intel I7 desktop machine with 16 GB of RAM and a 1 TB SSD for storage.

#### Disclaimers
The results presented in this project are derived for scientific purposes and commentaries only. They do not reflect the best-of-breed solution for your anticipated application environment,  but offers a starting point to make such an analysis. The quality of the results depend largely on the contributors of the experiments. Any questionable result should be addressed to the contributors directly  or the project owner.
