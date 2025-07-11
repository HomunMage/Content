# use SvelteFlow to create AI workflow visualized node-edge graph GUI editor

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

## What I want (LangGraph)

<img src="https://www.js-craft.io/wp-content/uploads/2025/03/langchain-vs-langgraph.webp" width="500">

</div>


<div class="slide">

## LangGraph-GUI

<img src="https://langgraph-gui.github.io/cover.webp" width="600">

repo: [https://github.com/LangGraph-GUI/LangGraph-GUI](https://github.com/LangGraph-GUI/LangGraph-GUI)

</div>


<div class="slide">

## My Design


* use Node to represent Edges
<iframe class="my-iframe" width="700" height="200" src="dataflow.html" style="background-color: white; display: inline;"></iframe>

* node design

<img src="./node_in_ts.webp" width="350"><img src="./node_in_json.webp" width="450">


</div>


<div class="slide">

### make SSOT
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

## END

Thank You

</div>


<div class="slide">

## Reference
* reactflow, svelteflow websites
* https://www.js-craft.io/blog/langchain-vs-langgraph/
* https://framerusercontent.com/images/7IPPObp2xkFVLH1IyW9QvFQ0a2I.gif
* https://pbs.twimg.com/media/GP5rEiZaEAAUqWu?format=jpg&name=4096x4096
* https://raw.githubusercontent.com/n8n-io/n8n/master/assets/n8n-screenshot-readme.png

</div>



