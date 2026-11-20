# AI-Powered Penetration Testing Harness

An experimental, AI-driven harness designed to coordinate existing penetration testing tools through the [Model Context Protocol (MCP)](https://modelcontextprotocol.io/). The project investigates how AI-assisted tool orchestration can help identify security vulnerabilities in web applications.

> **Project status:** Research and design. A proof of concept (PoC) is planned; the functionality described below is a project goal, not a claim that a working scanner is already available.

## Overview

AI-assisted development has made it easier to build web applications, but a functioning application is not necessarily a secure one. Identifying vulnerabilities often requires security knowledge and an understanding of how an application behaves.

This project explores whether an AI-driven harness can automate the use of existing penetration testing tools, interpret their outputs, and support the reporting of potential vulnerabilities. The intended result is a proof of concept demonstrating how these components can work together in a controlled testing environment.

## Project Objectives

- Design an AI-driven harness for coordinating penetration testing activities.
- Investigate how MCP servers can expose existing security tools to an AI-driven system.
- Evaluate existing penetration testing tools for suitability within the proposed architecture.
- Select web application vulnerability categories for testing, using the [OWASP Top 10](https://owasp.org/www-project-top-ten/) as a starting point.
- Develop and test a proof of concept in an authorized, isolated environment.

## Proposed Architecture

The architecture is still being researched. The diagram below illustrates the **intended high-level concept**, not a finalized implementation.

```text
             AI-Driven Harness
                     |
                     v
              MCP Interface
                     |
                     v
         Existing Pentesting Tools
                     |
                     v
         Authorized Test Application
                     |
                     v
          Findings and Test Output
```

The harness is intended to coordinate tool usage through MCP. Which tools, AI model, and MCP server design will be used has not yet been determined.

## Research Questions

The project is guided by the following main question:

> How can an AI-driven harness be designed to control existing penetration testing tools through the Model Context Protocol (MCP) to identify vulnerabilities in web applications?

The research covers four areas:

1. Designing the AI-driven harness.
2. Identifying the technical requirements for MCP-based tool integration.
3. Comparing existing penetration testing tools and selecting suitable options.
4. Selecting web application vulnerabilities to use when testing the proposed architecture.

## Scope

**In scope**

- AI-assisted orchestration of existing penetration testing tools.
- MCP-based integration between the harness and those tools.
- Web application security testing informed by the OWASP Top 10.
- A proof of concept evaluated in a controlled environment.

**Out of scope**

- Training or developing a new AI model.
- Creating new penetration testing tools from scratch.
- Claiming coverage of every vulnerability category or guaranteeing vulnerability detection.

The exact vulnerability categories and tool integrations will be selected during the research phase.

## Roadmap

- [x] Define the research problem, objectives, and scope.
- [ ] Research MCP, AI-driven harness design, existing tools, and vulnerability categories.
- [ ] Design the architecture and select integrations.
- [ ] Build the proof of concept.
- [ ] Test selected vulnerability scenarios in a controlled environment.
- [ ] Evaluate results and finalize the research documentation.

## Getting Started

The project is not yet available as a runnable application. Installation instructions, configuration requirements, and usage examples will be added once the proof of concept has been implemented.

## Responsible Use

This project is intended for security research and testing on systems where explicit authorization has been granted. Do not use it against third-party applications or infrastructure without permission. Automated results may contain errors and should be reviewed before being treated as confirmed vulnerabilities.

## References

- [Model Context Protocol — Official Documentation](https://modelcontextprotocol.io/)
- [OWASP Top 10](https://top10.owasp.org/2025/)
- [OWASP SAMM — Security Testing](https://owaspsamm.org/model/verification/security-testing/)

---

*Personal Research Project (PRP) — Cybersecurity.*
