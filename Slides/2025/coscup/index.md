---
title: Selfhosted Visualizing AI Workflows with LangGraph-GUI & CrewAI-GUI
---

<div class="slide">

## Self-hosted AI Workflow Visualization with LangGraph-GUI & CrewAI-GUI


<img src="https://langgraph-gui.github.io/cover.webp" style="height: 400px;"><img src="https://raw.githubusercontent.com/LangGraph-GUI/CrewAI-GUI-Qt/refs/heads/main/frontend.webp" style="height: 400px;">

* Interactive, local-first GUIs for building and monitoring AI pipelines
* Fully customizable: swap models, agents, and frameworks
* Deployable via Docker Compose or Kubernetes

</div>


<div class="slide">

## LangGraph-GUI Demo


</div>


<div class="slide">

## Motivation & Goals

1. **Local GPU Support** (e.g., Ollama)
2. **Full Customization** of UI and backend logic
3. **LangGraph Compatibility** for flexible graph-based workflows
4. **Easy Deployment** with Docker Compose and Kubernetes

* Other similar software
  * dify
    * <img src="https://framerusercontent.com/images/7IPPObp2xkFVLH1IyW9QvFQ0a2I.gif" width="600">
    * https://framerusercontent.com/images/7IPPObp2xkFVLH1IyW9QvFQ0a2I.gif
  * coze
    * <img src="https://pbs.twimg.com/media/GP5rEiZaEAAUqWu?format=jpg&name=4096x4096" width="600">
    * https://pbs.twimg.com/media/GP5rEiZaEAAUqWu
  * n8n
    * <img src="https://raw.githubusercontent.com/n8n-io/n8n/master/assets/n8n-screenshot-readme.png" width="600">
    * https://raw.githubusercontent.com/n8n-io/n8n/master/assets/n8n-screenshot-readme.png


</div>


<div class="slide">

## First attempts - CrewAI-Qt

<img src="../JSDC-LLM//crew-ai.webp" height="200">

Build CrewAI-GUI with pyside6

<img src="./crewai-gui.gif">


</div>

<div class="slide">

## Why Not CrewAI?

<img src="../JSDC-LLM//crew-ai.webp" height="200">

* **Pros:** 
  * Beginner-friendly introduction to AI agents
  * LangGraph, LangChain resource not friendly to green hands
* **Cons:**

  * Abstracts too many steps (limited visibility)
  * Frequent updates may breaks existing code

<img src="crewai-fail.webp" width="600">

</div>


<div class="slide">

## Why Not LangChain?

* **Modularity:** Tool usage is isolated, hard to combine
* **Fragility:** Breaking changes across versions
* **Abstraction:** Layers obscure data flow
<img src="abadon-langchain.webp" width="600">
[why we no longer use LangChain for building our AI agents](https://octomind.dev/blog/why-we-no-longer-use-langchain-for-building-our-ai-agents)

</div>


<div class="slide">

## Why Choose LangGraph

* **Graph-Centric Design**: Focus on nodes and edges
* **Model-Agnostic**: Plug in any LLM or agent
* **Composable**: Mix-and-match components seamlessly

* Learning Resource:
  * [LangGraph-GUI/LangGraph-learn](https://github.com/LangGraph-GUI/LangGraph-learn)

</div>



<div class="slide">

## Design of LangGraph-GUI

1. **JSON Contract**: text based, easy to decouple
2. **Frontend Agnostic**: ReactFlow, SvelteFlow, or custom
3. **Backend Flexible**: Python, etc.
4. **Extensible**: Add custom properties via `ext:` fields

</div>




<div class="slide">

## python backend

flask -> fastapi

Flask is friendly to beginner

FastAPI is better performance


</div>



<div class="slide">

## Thank You!


</div>