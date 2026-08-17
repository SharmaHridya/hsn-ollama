FROM ollama/ollama:latest
# Pull model at build time so it's baked into the image
RUN (ollama serve &) && sleep 5 && ollama pull qwen2.5:3b
EXPOSE 11434
ENTRYPOINT ["ollama", "serve"]