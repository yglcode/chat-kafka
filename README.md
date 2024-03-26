### chat-kafka

[GPTScript](https://github.com/gptscript-ai/gptscript) is great to glue together various system (admin) utilities and DevOps tools, just as what shell scripts did, although written in human languages.

chat-kafka a thin wrapper over [kaf](https://github.com/birdayz/kaf), provides a set of tools and a vocabulary of words and sentences for gptscript to "talk" to kafka broker cluster, such as "connect to broker at localhost:9092", "create a topic A", "send message to topic A", etc. Check out [examples/data-pipeline.gpt](https://github.com/yglcode/chat-kafka/blob/main/examples/data-pipeline.gpt) for more examples, which is a demo data pipeline: start local broker in docker, create topics, ingest log data, data transformation and aggregation.

To run the example, you need:
1. install gptscript and set up OpenAI token as instructed in gptscript project.
2. have docker installed.
3. clone this repo
4. cd examples; gptscript data-pipeline.gpt
