---
layout: project
title: "Exploring Artist Data with Sigma.js"
date: 2014-02-08 11:56:00
categories: project
tags: javascript python sigmajs networkx graphviz numpy
op-quote: ""
op-quote-sp: ""
project-href: ""
link-title: "View on Github"
---

## Testing out the data visualization library [Sigma.js](http://sigmajs.org/)

<div id="graph-container"></div>
<!-- START SIGMA IMPORTS -->
<script src="../scripts/sigma-js/sigma.core.js"></script>
<script src="../scripts/sigma-js/conrad.js"></script>
<script src="../scripts/sigma-js/utils/sigma.utils.js"></script>
<script src="../scripts/sigma-js/utils/sigma.polyfills.js"></script>
<script src="../scripts/sigma-js/sigma.settings.js"></script>
<script src="../scripts/sigma-js/classes/sigma.classes.dispatcher.js"></script>
<script src="../scripts/sigma-js/classes/sigma.classes.configurable.js"></script>
<script src="../scripts/sigma-js/classes/sigma.classes.graph.js"></script>
<script src="../scripts/sigma-js/classes/sigma.classes.camera.js"></script>
<script src="../scripts/sigma-js/classes/sigma.classes.quad.js"></script>
<script src="../scripts/sigma-js/captors/sigma.captors.mouse.js"></script>
<script src="../scripts/sigma-js/captors/sigma.captors.touch.js"></script>
<script src="../scripts/sigma-js/renderers/sigma.renderers.canvas.js"></script>
<script src="../scripts/sigma-js/renderers/sigma.renderers.webgl.js"></script>
<script src="../scripts/sigma-js/renderers/sigma.renderers.def.js"></script>
<script src="../scripts/sigma-js/renderers/webgl/sigma.webgl.nodes.def.js"></script>
<script src="../scripts/sigma-js/renderers/webgl/sigma.webgl.nodes.fast.js"></script>
<script src="../scripts/sigma-js/renderers/webgl/sigma.webgl.edges.def.js"></script>
<script src="../scripts/sigma-js/renderers/webgl/sigma.webgl.edges.fast.js"></script>
<script src="../scripts/sigma-js/renderers/webgl/sigma.webgl.edges.arrow.js"></script>
<script src="../scripts/sigma-js/renderers/canvas/sigma.canvas.labels.def.js"></script>
<script src="../scripts/sigma-js/renderers/canvas/sigma.canvas.hovers.def.js"></script>
<script src="../scripts/sigma-js/renderers/canvas/sigma.canvas.nodes.def.js"></script>
<script src="../scripts/sigma-js/renderers/canvas/sigma.canvas.edges.def.js"></script>
<script src="../scripts/sigma-js/renderers/canvas/sigma.canvas.edges.arrow.js"></script>
<script src="../scripts/sigma-js/middlewares/sigma.middlewares.rescale.js"></script>
<script src="../scripts/sigma-js/middlewares/sigma.middlewares.copy.js"></script>
<script src="../scripts/sigma-js/misc/sigma.misc.animation.js"></script>
<script src="../scripts/sigma-js/misc/sigma.misc.bindEvents.js"></script>
<script src="../scripts/sigma-js/misc/sigma.misc.drawHovers.js"></script>
<!-- END SIGMA IMPORTS -->
<script src="../scripts/sigma-js/plugins/sigma.parsers.json/sigma.parsers.json.js"></script>
<script>
  sigma.parsers.json('../scripts/data/coords_formatted.json', {
    container: 'graph-container'
  });
</script>
