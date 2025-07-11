---
title: use SvelteFlow to create AI workflow visualized node-edge graph GUI editor
---


<div class="slide">

## use SvelteFlow to create AI workflow
<p style="font-size: 2em;"> visualized node-edge graph GUI editor</p>


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

<img src="./crew-ai.webp" width="400">

<img src="https://www.js-craft.io/wp-content/uploads/2025/03/langchain-vs-langgraph.webp" width="500">

</div>





<div class="slide">

## My Design


* use Node to represent Edges
<iframe class="my-iframe" width="700" height="200" src="dataflow.html" style="background-color: white; display: inline;"></iframe>

* node design

<img src="./node_in_ts.webp" width="350">


</div>


<div class="slide">

## make SSOT
* hard to sync Redux and Context
* data update flow cannot align SSOT design
* not only nodes, but also edges need update seperatly

### Conclusion
redux is not affinity with React

</div>

<div class="slide">

## Why SvelteFlow

<img src="https://svelteflow.dev/opengraph-image.jpg" height="200">

* Svelte 5 is signals design
  * code numbers usually fewer than react
  * easy to pass computed runes
* SvelteFlow 1.0 highly affinity svelt 5
  * use rune, signals features

</div>


<div class="slide">

## Simple Demo

  
  <div class="embed_youtube" yt-title="simple demo" yt-url="QpJ37k8yquA" yt-width="700">demo
  </div>
  

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
