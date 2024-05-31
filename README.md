# MORPC GitHub Organization

This organization contains code intended for use by the Mid-Ohio Regional Planning Commission.

As of May 2024, the organizations is maintained by Adam Porr, Research & Data Officer

## Suggested naming conventions

The following naming conventions have been applied to some of the existing repositories.  It is not mandatory to adhere to these conventions for new repositories.

  - Repositories created by MORPC are prepended by `morpc-` to differentiate them from repositories forked from upstream repositories created by third-parties.
  - Some repositories have been structured as modules to be conducive to pipelining.  Sometimes one of the following suffixes is applied to hint at the function of the module and its stage in the pipeline.  As of May 2024, this is a weak and emerging standard.  Additional suffixes are likely needed for contexts not described by the existing suffixes.  A typical pipeline might consist of `fetch` > `standardize` > `summarize` and then perhaps `profile`.
    - fetch - Fetches a third-party dataset from a remote source and stores a local copy with as high fidelity as possible
    - standardize - Transform a dataset into a standard form (typically a long form "fact table").  The output typically contains the same data as the input, just in a different form.
    - summarize - Summarize a dataset according to user-specified parameters, usually by time period, geography period, or attribute grouping.  Output data is fundamentally different than the input due to the summarization.
    - profile - Combine several sets of disparate data (usually summarized data) to construct a holistic picture of something (perhaps a specific place).  Conceptually similar to the profiles offered on data.census.gov.
