I had some difficulty getting these to work properly, however I also only had a short period of time to spend on it and I'm sure that there is a more advanced way if I do more research.

The [python-fastapi](https://openapi-generator.tech/docs/generators/python-fastapi) generator is in beta, and would not function right off the bat. So I switched to using the [python-flask](https://openapi-generator.tech/docs/generators/python-flask) version.

The python-flask version was able to get running with no issues, but failed to pass the testing suite, which tells me that there is something wrong with its current implementation, whether that is the generation or the spec.

[[Python SDK]]