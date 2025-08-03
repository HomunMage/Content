---
title: Selfhosted Visualizing AI Workflows with LangGraph-GUI & CrewAI-GUI
---


<div class="slide">

## Selfhosted Visualizing AI Workflows with LangGraph-GUI & CrewAI-GUI


<img src="https://langgraph-gui.github.io/cover.webp" style="height: 400px;"><img src="https://raw.githubusercontent.com/LangGraph-GUI/CrewAI-GUI-Qt/refs/heads/main/frontend.webp" style="height: 400px;">



</div>

<div class="slide">

## Why Starting the repo

* Want support local GPU, ex: Ollama
* Most solutions cannot do custmize of the software itself
* Want support LangGraph
* Want selfhost with Docker Compose and Kubernetes
* dify
  * <img src="https://framerusercontent.com/images/7IPPObp2xkFVLH1IyW9QvFQ0a2I.gif" width="600">
* coze
  * <img src="https://pbs.twimg.com/media/GP5rEiZaEAAUqWu?format=jpg&name=4096x4096" width="600">
* n8n
  * <img src="https://raw.githubusercontent.com/n8n-io/n8n/master/assets/n8n-screenshot-readme.png" width="600">


</div>



<div class="slide">

## Why not CrewAI

pros:
CrewAI is freidnly for begineer understand about AI Agent concept

cons:
* crewAi too many hidden steps, and abstract too many layer, 
* update will deprecate old code

<img src="crewai-fail.webp" width="600">



</div>

<div class="slide">

## Why not LangChain

<img src="abadon-langchain.webp" width="600">

LangChain's tool actually just single usage, cannot combine with other component, only demo example code can work

any change, combine to other bricks will fail

and also have similar problem like CrewAI, too many abstract layer, update break laster version code



</div>

<div class="slide">

## LangGraph

better decouple design, just care about graph,

you can replace any LLM handler, any agent



</div>

<div class="slide">

## Design of LangGraph-GUI

use json to tranmit for frontend, backend

easy to change any side, such frtonend proting from ReactFlow to SvelteFlow

backend and change any framework also

you can extend the json by the ```ext: ``` feilds


</div>




<div class="slide">

## END

Thank You

</div>




<script src="https://posetmage.com/cdn/js/EmbedYoutubeVideo.js">
