[[Testing Suite Issue - GET Request Only.png]]

Reference the above image, the testing suite as it is now does not make any POST requests, only GETing the routes with IDs taken from the examples in the spec.

Originally, there were two tests as part of the suite; one was a more biased test that would task the agent to write some text to a file which was removed, and the other was the contract test. We removed the first test to remove the bias, but apparently that was the only one making POST requests, so far as I've seen.

Additionally, even with just the GET requests, the Agent Protocol SDKs for either Python or JS/TS seem to not be valid implementations of the spec, with one returning with Status Code 500 instead of 404 and the other returning with only text instead of a structured JSON object. They also do not have functioning pagination, at least as far as the test is concerned.

[[Testing Suite]] [[Agent Protocol]] [[Python SDK]] [[Typescript/Javascript SDK]]