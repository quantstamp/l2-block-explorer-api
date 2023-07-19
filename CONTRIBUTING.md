# Contribution Guidelines

This repository presents a standard for APIs that power L2 block explorers. Like other areas in the Ethereum and Web3 communities, L2s are evolving rapidly. Therefore, the standard must continue to evolve in order to keep up with innovations in L2 block explorers. This will require input and feedback from a variety of individuals in the community.

Any contribution, from writing whole sections to simply correcting spelling and grammar mistakes, will be greatly appreciated. To provide feedback, please open a pull request following the guidance outlined in this document. Please note that these are just guidelines, not rules. Use your best judgment and feel free to propose changes to anything in this repository, including the contribution guidelines. 

**Table of Contents**

- [Code of Conduct](#code-of-conduct)
- [Pull Requests](#pull-requests)
- [File Structure](#file-structure)
- [Documentation Styleguide](#documentation-styleguide)

## Code of Conduct

We take our community seriously and hold ourselves and other contributors to high standards of communication. By participating and contributing to this project, you agree to uphold our [Code of Conduct](./CODE_OF_CONDUCT.md). 

## Pull Requests

Pull requests are the primary mechanism used for proposing and accepting contributions. We recommend creating a [topic branch](https://www.git-scm.com/book/en/v2/Git-Branching-Branching-Workflows#Topic-Branches) and then sending a pull request to the `main` branch from that topic branch. Once the pull request is received, our team will review it as soon as possible. We may ask for changes to be made before the pull request can be merged. Once the changes are addressed, we will merge the topic branch into the main branch.

## File Structure
During the development of the standard, we created the following file structure. We encourage any new contributions to follow this structure in order to preserve consistency.
- The `README.md` file contains the following information:
    - **Section 1:** This section describes the requirements and specifications of the API standard. The information in this section adheres to the following conventions:
        - **Section 1.4.1** contains the "base requirements". These are requirements that ALL L2 block explorers must support.
        - **Section 1.4.2** contains the "extension requirements". These extensions are optional and will only be enabled depending on the nature of the block explorer.
        - The requirements for these sections are presented in tables. Each requirement is assigned a unique identifier, has a description, and is labeled as either `Core` (required if the extension is enabled) or `Optional`.
        - **Section 1.2** presents a diagram with the extension dependency graph. This diagram must be updated if a new extension is added.
    - **Section 2:** This section describes the methodology that our team used to generate the standard. It is unlikely that this section will need to be updated, except for correcting any spelling or grammar mistakes.
- The `l2-specification/` folder contains information, such as architecture and transaction model, about the L2 protocols that our team reviewed to develop and validate the standard. As with Section 2 of the `README.md` file, we do not expect many changes, except to address any potential errors.
- The `open-api/` folder contains an OpenAPI skeleton implementation of our API standard. This might need to be updated if there are changes to the requirements in Section 1. 

## Documentation Styleguide

- Use [GitHub-flavored markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#GitHub-flavored-markdown).
- It's important to keep in mind that people from different backgrounds might read the standard. Therefore, we cannot assume that everyone will understand all the terms used in the document. If a new or complex term is introduced, be sure to define it using a footnote as shown below:
    - This is a new concept<sup>[[1]](#test-concept)</sup> used somewhere in the document.
    - <a id="test-concept"></a> **Concept**. This is where we define the concept.