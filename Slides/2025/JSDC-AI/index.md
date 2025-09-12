---
title: Use SvelteFlow to Create AI Workflow Visualized Node-Edge Graph GUI Editor
---

<div class="slide">

## Use SvelteFlow to Create AI Workflow Visualized Node-Edge Graph GUI Editor

<img src="https://langgraph-gui.github.io/cover.webp" width="700">

</div>


<div class="slide">

## What I want

like dify, Coze, n8n.....

and self-host, more flexibity, use langgraph

* dify
  * <img src="https://framerusercontent.com/images/7IPPObp2xkFVLH1IyW9QvFQ0a2I.gif" width="600">
* coze
  * <img src="https://pbs.twimg.com/media/GP5rEiZaEAAUqWu?format=jpg&name=4096x4096" width="600">
* n8n
  * <img src="https://raw.githubusercontent.com/n8n-io/n8n/master/assets/n8n-screenshot-readme.png" width="600">

</div>

<div class="slide">

## Similar Base libs

<img src="./crew-ai.webp" width="300"><img src="https://www.js-craft.io/wp-content/uploads/2025/03/langchain-vs-langgraph.webp" width="300">

But all of these not have official GUI, we need create by ourself.

</div>


<div class="slide">

## Why xyflow

xyflow is mature js library (svelteflow, reactflow)

<img src="https://user-images.githubusercontent.com/2857535/279644026-a01c231c-6c6e-4b41-96e0-a85c75c9acee.svg#gh-dark-mode-only">

* use Node to represent Edges
<iframe class="my-iframe" width="700" height="200" src="dataflow.html" style="background-color: white; display: inline;"></iframe>

* node design

<img src="./node_in_ts.webp" width="350">

</div>


<div class="slide">

## Choose ReactFlow

<img src="https://user-images.githubusercontent.com/3797215/156259138-fb9f59f8-52f2-474a-b78c-6570867e4ead.svg" height="300">

* React have large ecosystem and community
* Graph GUI with node edge design
* flexibity enough for make it as editor

</div>


<div class="slide">

## The Jourery of ReactFlow

LangGraph-GUI 1.0 using reactflow

* Hard to make SSOT
  * hard to sync Redux and React Context
  * data update flow cannot align SSOT design
  * not only nodes, but also edges need update seperatly
* Code lines more longer
* most js libs use signals now but react not

<img src="./reactflow.webp">

</div>

<div class="slide">

## Why SvelteFlow

<img src="https://svelteflow.dev/opengraph-image.jpg" height="300">

* Svelte 5 using signals
  * code numbers usually fewer than react
  * easy to pass computed runes
* SvelteFlow 1.0 highly affinity svelt 5 rune, signals
* fewer and more beautiful lines

</div>


<div class="slide">

## Final Design
[LangGraph-GUI-Svelte](https://github.com/LangGraph-GUI/LangGraph-GUI-Svelte)

* Nodes are SSOT
  * edges is readonly, nodes update will trigger edges
  * no need redux, just use writable

</div>



<div class="slide">

## Svelte Elegant

[sample code](https://github.com/LangGraph-GUI/LangGraph-GUI-Svelte/blob/b56130696bc4e4202f3a4ffa013ef1a8d73aee35/src/routes/graph/flow/graphs.store.svelte.ts)

signal chain: **Node** --> **Edge** --> **SvelteFlow**

<img src="./currentEdges.webp">

<img src="./SvelteFlowTypes.webp">


</div>


<div class="slide">

## Simple Demo

<img src="../COSCUP/extend-demo.gif">

</div>


<div class="slide">

## END

<p style="font-size: 3em;">Thank You</p>

* Reference
  * reactflow, svelteflow websites
  * https://docs.crewai.com/en/introduction
  * https://www.js-craft.io/blog/langchain-vs-langgraph/
  * https://framerusercontent.com/images/7IPPObp2xkFVLH1IyW9QvFQ0a2I.gif
  * https://pbs.twimg.com/media/GP5rEiZaEAAUqWu?format=jpg&name=4096x4096
  * https://raw.githubusercontent.com/n8n-io/n8n/master/assets/n8n-screenshot-readme.png

</div>

<script src="https://posetmage.com/cdn/js/EmbedYoutubeVideo.js">
