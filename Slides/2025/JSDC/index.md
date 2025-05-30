# LangGraph-GUI by SvelteFlow (ReactFlow)

<div class="slide">

## LangGraph-GUI

<img src="https://langgraph-gui.github.io/cover.webp" width="600">

</div>


<div class="slide">

## What I want

like dify, Coze, n8n.....

and self-host, more flexibity, use langgraph

</div>

<div class="slide">

## Why Choose ReactFlow


<img src="https://user-images.githubusercontent.com/3797215/156259138-fb9f59f8-52f2-474a-b78c-6570867e4ead.svg" height="300">

* Graph GUI with node edge design
* flexibity enough for make it as editor
* large community support

</div>


<div class="slide">

## The Jourery of ReactFlow

[LangGraph-GUI-reactflow](https://github.com/LangGraph-GUI/LangGraph-GUI-reactflow)

### Hard to make SSOT
* need redux, useContext both exist, hard to sync by order
* data update flow cannot align SSOT design
* not only nodes, but also edges need update seperatly

### Conclusion
ReactFlow is not affinity with React

</div>

<div class="slide">

## Why SvelteFlow

<img src="https://svelteflow.dev/opengraph-image.jpg" height="300">

* Svelte 5 is signals design
  * code numbers usually fewer than react
  * easy to pass computed runes
* SvelteFlow 1.0 highly affinity svelt 5
  * use rune, signals features

</div>


<div class="slide">

## Final Design
[LangGraph-GUI-Svelte](https://github.com/LangGraph-GUI/LangGraph-GUI-Svelte)

* Nodes are SSOT
  * edges is readonly, nodes update will trigger edges
  * no need redux, just use writable

</div>



<div class="slide">

## End

Thank you.

</div>

