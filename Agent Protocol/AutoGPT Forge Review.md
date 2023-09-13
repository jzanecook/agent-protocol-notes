## Unorganized Notes
- The Forge in the dedicated repository hasn't been changed in a week, whereas the Forge in the AutoGPT repository has been updated recently.
- The README for the forge still references the e2b sdk rather than the Agent Protocol.
- It is a fresh implementation of the Agent Protocol
- The CI/CD Workflow works well, although the current testing suite is not necessarily complete
	- See [[Testing Suite Issues]]
- The current CI for the Forge is not passing, although I believe merwane is working on that currently.
- **This SDK is Compliant**
- (External) The benchmark is biased towards Code Generation
- The added Makefile is unnecessary
	- [Link to Makefile](https://github.com/Significant-Gravitas/Auto-GPT-Forge/blob/master/forge/Makefile)
	- The purpose of this is to copy the agent SDK to/from the AutoGPT system, but we would likely rather have the SDK in a package manager format
	- It also appears to be outdated as it references folders that no longer exist.
- The Dockerfile looks great
	- However, why is ffmpeg a dependency? Am I missing something?
	- May also consider creating a `docker-compose.yml` to make it even easier.
- There is an extension to the protocol for benchmarking that adds the following routes:
	- `/skill_tree`
	- `/agent/challenges`

## Summary
Overall the Forge is a great place to point people to go to get started with using the Agent Protocol, provided that there are no major discrepancies between the forge that's available in the `Auto-GPT` repo and the `Auto-GPT-Forge` repo.

If we were to go with Plan A, some minor changes would be made to remove dead code and comb over it all making sure there are no inherent biases in the system towards any specific type of agent.

Additionally, the existing CI/CD pipeline for the forge works well and could be a good starting point should we ensure that our own SDK exists as a reference implementation. The only potential issue with it is that the compliance checker is not fully complete.