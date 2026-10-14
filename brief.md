Version: NAFATH-V3
Track: Networking 

## Overview
A trustworthy AI assistant for a public service must provide accurate, secure, and useful information to the public. Software engineering helps developers maintain reliable systems and manage updates safely. Artificial intelligence allows the assistant to understand questions and generate helpful answers. Mobile security protects people who access public services through smartphones. Networking enables secure communication between users, servers, and government systems. Cybersecurity helps prevent attacks, protect information, and reduce unauthorized access. Data management supports responsible handling of personal information and helps maintain privacy. These six areas work together to improve service quality and public trust. A reliable assistant must also communicate its limitations and avoid presenting uncertain information as fact. For Networking, understanding IPv6 addressing is important because connected services need reliable communication as the number of devices and systems continues to grow.
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
IPv6 uses 128-bit addresses, while IPv4 uses 32-bit addresses. This means IPv6 can provide far more unique addresses for phones, computers, sensors, and other connected devices. As more devices join the internet, IPv6 helps prevent address shortages and supports reliable connections. For a public-service AI app, supporting IPv6 helps it stay available as demand grows, though both IPv4 and IPv6 traffic still need to be securely configured.

Resource: RFC 8200: Internet Protocol, Version 6 (IPv6) Specification - https://www.rfc-editor.org/rfc/rfc8200

## Cybersecurity
Prompt injection is an attack where user prompts alter an LLM-based system’s behavior, potentially causing it to ignore instructions, reveal sensitive information, or misuse its permissions. Direct injections use malicious commands in the user’s message, while indirect injections hide them in retrieved external content. To reduce the risk, validate and filter inputs and retrieved content, and limit the system’s tools, APIs, and permitted actions. OWASP classifies this as LLM01:2025 Prompt Injection.

Resource: OWASP Top 10 for LLM Applications - https://genai.owasp.org/llm-top-10/

## Data
When storing chat logs, anonymisation changes personal data so people can no longer be identified, either from the data alone or when combined with other information. Pseudonymisation replaces direct identifiers, such as names, with codes or reference numbers, but people may still be identified using separately held information. Therefore, pseudonymised chat logs remain personal data, while effectively anonymised chat logs fall outside data-protection law.

Resource: Introduction to anonymisation - https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/data-sharing/anonymisation/introduction-to-anonymisation/

## Misconception in My Track
A common misconception is that IPv6 is simply IPv4 with a larger address space. In fact, RFC 8200 states that IPv6 increases the IP address size from 32 bits to 128 bits. This change supports more levels of addressing hierarchy, a much greater number of addressable nodes, and simpler autoconfiguration of addresses. IPv6 also improves multicast routing scalability by adding a scope field to multicast addresses and introduces anycast addresses, which send a packet to any one node in a group. However, adopting IPv6 does not automatically make a network secure or remove the need for IPv4; networks still require correct configuration and appropriate security controls. The evidence is in RFC 8200, Section 1, “Introduction,” under “Expanded Addressing Capabilities.”
## Open Question
Which IPv6 transition strategy best fits the agency's existing network?
