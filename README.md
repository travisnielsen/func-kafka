# Sample Azure Function for Kafka

This is based on sample provided in the [Kafka extension documentation](https://github.com/Azure/azure-functions-kafka-extension/blob/dev/samples/javascript/README.md). It is assumed you have a local development enviornment that includes the Azure Functions Core Tools.

In your local development environemnt, first run: , `npm install`, `npm run build`, and `func extensions install` to ensure all dependencies are in-place locally. Next, create your Docker image using the following command:

```bash
docker build -t [your-docker-id]/func-kafka:0.0.1 .
```

Finally, you can run the container locally:

```bash
docker run -p 8080:80 -it [your-docker-id]/func-kafka:0.0.1
```
