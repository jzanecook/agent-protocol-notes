### Overview
<small>September 12th, 6:30 PM PST</small>

- Decide Current Plan for Agent Protocol v1.0
- Discuss Existing Pull Requests
- Review RFC/Spec
- Discuss Introductory/Explanatory Video Ideas



---
### About the Agent Protocol SDK

#### Plan **A**<small>utoGPT-Forge</small>
>Adapt the Forge into our own SDK

#### Plan **B**<small>uilding Automagically</small>
>Building the SDK automagically from OpenAPI Server Generator

#### Plan **C**<small>lean and Lean</small>
>Removing any SDKs and keeping only the spec and potentially any instructional material



---
## Plan A<small>utoGPT-Forge</small>
Reference [[AutoGPT Forge Review]]

| Pros | Cons |
| ---- | ---- |
| Should be relatively quick to implement a streamlined "dummy" example agent as well as release an example implementation of an SDK | We would be dropping the JS/TS SDK |
| | Potential Issues with AutoGPT's competitor agents? |

## Plan B<small>uilding Automagically</small>
Reference [[OpenAPI SDK Generators Review]]

| Pros | Cons |
| ---- | ---- |
| Would be an automated system based off of the spec | Potentially unnecessary, see [[Criticism of Generator Usage]] |

## Plan C<small>lean and Lean</small>

| Pros | Cons |
| ---- | ---- |
| Significantly less to maintain | Relies on third party implementations which could be out of spec |

## Overall Best Plan
<small>By Ziggy's Opinion</small>

1. Structure the Agent Protocol repository so that it is only the spec
2. Split the repository so that the spec, RFC, and documentation site are in separate repositories
3. Remove the existing (non-compliant) SDKs
4. Follow a structure similar to GraphQL
	- Reference [[GraphQL Repository Structure]]
	- Also Reference [[GraphQL SDK List]] for an idea of what the agent protocol site could look like in the future, keeping a list of compliant SDKs made internally as reference or externally as full packages.

---
# Discussion about Pull Requests
[Linked Here](https://github.com/AI-Engineers-Foundation/agent-protocol/pulls)



---
# Review RFC/Spec
#### Initial Questions
- Does the spec include any potential biases towards any specific form of agent?
	- e.g. Code builders, Image generators, Building automation, Physics simulation, etc.
- Does the spec make sense to a newcomer (with instructional material)?
- Does the RFC comply with the spec or vice versa?


# Introductory/Explanatory Video Discussion

#### Initial Idea
Create an Introductory Video where we create an agent to add something to the video, or as an instructional piece to use. The video should be have elements of an infographic to help visualize the protocol in an easy to understand format.


---
[[Agent Protocol]]