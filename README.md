# Topic: Optimist Score by Flipside

[Optimism](https://www.optimism.io/) is a L2 EVM Blockchain using Optimistic rollups as its scaling solution. Optimism's native token, OP, was launched in May of 2022. 

Late in 2022, Optimism Foundation approached Flipside, requesting that Flipside contriubute to their new [Attestation Station](https://community.optimism.io/docs/governance/attestation-station/). The idea being that users should be able to attest to their on or off chain behaviors to an on-chain contract in a peer-to-peer manner. 

In response to this request, Flipside created the [Optimist Score](https://science.flipsidecrypto.xyz/optimist/) as a way to attest to an address' on-chain behaviors. With minimal marketing for this tool, Flipside recieved over 30,000 attestations. We want to take a look at what motivated this many people to use a very simple attestation tool!

# Reproduce Analysis

All analysis is reproducible using the R programming language. You'll need (1) an shroomDK API key to copy our SQL queries and extract data from the [FlipsideCrypto data app](https://next.flipsidecrypto.xyz/); and (2) renv to get the exact package versions we used.

## shroomDK

shroomDK is an R package that accesses the FlipsideCrypto REST API; it is also available for Python. You pass SQL code as a string to our API and get up to 1M rows of data back!

Check out the [documentation](https://docs.flipsidecrypto.com/shroomdk-sdk/get-started) and get your free API Key today.

## renv

renv is a package manager for the R programming language. It ensures analysis is fully reproducible by tracking the exact package versions used in the analysis.

`install.packages('renv')`

## Instructions

To replicate this analysis please do the following:

1.  Clone this repo.
2.  Save your API key into a .txt file as 'api_key.txt' (this exact naming allows the provided .gitignore to ignore your key and keep it off github).
3.  Open the `R PROJECT NAME HERE` R Project file in your R IDE (we recommend, RStudio).
4.  Confirm you have renv installed.
5.  Restore the R environment using `renv::restore()` while in the `R PROJECT NAME HERE` R Project.
6.  You can now run `SPECIFY .R FILE(s) and/or .Rmd FILE(s) HERE`

If any errors arise, double check you have saved your API key in the expected file name and format.
