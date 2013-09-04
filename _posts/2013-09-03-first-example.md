---
title: First
layout: default
---

# First

<script type="text/javascript">
var dataset = [5,10,15,20,25];
d3.select('#right-col').selectAll()
  .data(dataset)
  .enter()
  .append('p')
  .text(function (d) { return d;})
  .style("color", function (d) {
    if (d > 15) return "red";
    else return "black";
  });
</script>