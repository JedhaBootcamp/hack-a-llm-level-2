# Hack a LLM - Level II

This is a simple exercise to practice basic LLM hacking technics.

## To run the code 

### Directly from source

```bash
git clone https://github.com/JedhaBootcamp/hack-a-llm-level-2
cd ./hack-a-llm-level-2
docker build . -t jedha/hack-a-llm-level-2
docker run -d \
    --name hack-a-llm-level-2 \
    -p 80:80 \
    -e OPENAI_API_KEY=YOUR_API_KEY \
    -e OPENAI_MODEL=YOUR_MODEL \
    -e PORT=80 \
    --restart=always \
    jedha/hack-a-llm-level-2
```

### From docker hub (Discontinued)

```bash
docker run -d \
    --name hack-a-llm-level-2 \
    -p 80:80 \
    -e OPENAI_API_KEY=YOUR_API_KEY \
    -e OPENAI_MODEL=YOUR_MODEL \
    --restart=always \
    jedha/hack-a-llm-level-2
```

## Don't forget

* Make sure `OPENAI_API_KEY` is set for the code to run. 
