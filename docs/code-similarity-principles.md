

# Code Similarity Overview

The Code Similarity search in ARCAD Transformer Microservices involves finding and comparing pieces of code to identify similarities. This process starts by extracting pseudocode from a source, then searching the repository to locate other instances of similar code.

The goal of this feature is to fully understand the impact of specific code by determining if it appears elsewhere in the codebase and, if it does, pinpointing its exact location(s).

## Code Similarity Workflow

When you launch a Code Similarity search, the process follows these steps:

| Step     | Description                                                                            |
|----------|----------------------------------------------------------------------------------------|
| **1.**   | Extract the pseudocode from the selected start and end sequence in the source code.    | 
| **2.**   | Search the entire repository for blocks of code similar to the extracted pseudocode.   |
| **3.**   | List all source files and members that contain similar code.                           |

The overall Code Similarity analysis ensures that the code being searched matches the behavior of the original pseudocode, ensuring consistency and accuracy in the results.

> [!Note]  
> The Code Similarity analysis mainly focuses on the code within the source repository, excluding external factors.

Converting source code to pseudocode helps in identifying similar code within the repository.  
This conversion follows specific rules to ensure consistency in the code.

## Working with Pseudocode

This feature, part of the ARCAD Transformer Microservices product, enables the analysis of *RPGLE* and *SQLRPGLE* source code to generate pseudocode representations of the analyzed sources.  
Pseudocode can be generated in two ways:

- At the **application** repository level, which creates pseudocode for all relevant sources within the repository.
- At the **version** level, which generates pseudocode for sources within a specific version.

> **Important**  
> As of now, only *RPGLE* and *SQLRPGLE* sources are supported for pseudocode generation; other source types are not compatible.

By generating pseudocode from a given block of source code, you can find similar code by comparing the pseudocode with the entire content of the repository to identify matches.

This whole process is facilitated by the `AGENPSCSRC` command.

> **Reference**  
> For additional information, refer to the integrated help of the `AGENPSCSRC` command using *F1*.

## Parameters for Code Similarity Matches

The Code Similarity process requires the following parameters to be specified:

- **Minimum Percentage of Matching**: Specifies the threshold for how much code needs to match.
- **Minimum Number of Components**: Sets the minimum number of code components that must be similar for a match to be considered.

> **Reference**  
> For more information about these parameters, refer to the [Launching Code Similarity Analysis](analyze-code.md) section.

This approach ensures a thorough and accurate identification of similar code across the entire repository.

> **Reference**  
> For additional information, refer to the integrated help of the `ASCNSEQSRC` command using *F1*.

The conversion of source code to pseudocode helps identify similar code in the repository.

> **Reference**  
> The pseudocode generation is based on rules to verify the consistency of the source code. These rules are defined in the tables in the [Code Conversion](appendix.md).
