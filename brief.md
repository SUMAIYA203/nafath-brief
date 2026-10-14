Version: NAFATH-V3
Track: Networking 

## Overview
A trustworthy AI assistant for a public service must provide accurate, secure, and useful information to the public. Software engineering helps developers maintain reliable systems and manage updates safely. Artificial intelligence allows the assistant to understand questions and generate helpful answers. Mobile security protects people who access public services through smartphones. Networking enables secure communication between users, servers, and government systems. Cybersecurity helps prevent attacks, protect information, and reduce unauthorized access. Data management supports responsible handling of personal information and helps maintain privacy. These six areas work together to improve service quality and public trust. A reliable assistant must also communicate its limitations and avoid presenting uncertain information as fact. 
## Software
Software uses Semantic Versioning to indicate changes to an API. It consists of three numbers: MAJOR.MINOR.PATCH. MAJOR version is incremented when backward-incompatible changes are introduced to the public API. MINOR version is incremented when new features are added in a backward-compatible manner. PATCH version is incremented when backward-compatible bug fixes are made. This system helps developers and users know the impact of each release and plan updates more effectively. Therefore, precise versioning is essential for maintaining a reliable API.

Resource: Semantic Versioning 2.0.0 - https://semver.org/spec/v2.0.0.html
## AI
Retrieval-Augmented Generation (RAG) combines a pre-trained language model with an external, searchable knowledge source, such as a dense index of documents. Before or while generating an answer, the system retrieves relevant passages and uses them as context. This helps reduce incorrect answers because the model can ground its response in up-to-date, specific evidence rather than relying only on knowledge stored in its parameters. RAG can also make responses more factual and support provenance by identifying the retrieved sources.

Resource: Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks - https://arxiv.org/abs/2005.11401
## Mobile
iOS App Transport Security (ATS) helps protect connections made through Apple networking systems, including URLSession, by using TLS encryption by default. If an app attempts to connect to an HTTP endpoint, ATS blocks the insecure cleartext connection and generates a runtime error. If an older server does not support TLS, developers can add a narrowly scoped ATS exception for that specific domain in Info.plist, though Apple recommends avoiding unencrypted connections whenever possible.

Resource: Fine-tune your App Transport Security settings - Apple Developer - https://developer.apple.com/news/?id=jxky8h89 

## Networking

## Cybersecurity

## Data

## Misconception in My Track

## Open Question
