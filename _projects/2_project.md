---
layout: page
title: Optimal Route API
description: REST API using .NET 6 (C#) that calculates the optimal route between two cities.
img: assets/img/proj-route.png
importance: 1
category: software
github: https://github.com/norians/OptimalRouteAPI
---

This project implements a REST API in .NET 6 (C#) to compute the shortest route between two cities based on a set of weighted road connections.
The solution explores all valid paths using an iterative depth-first search (DFS) strategy and selects the route with the minimum total travel time.

The focus of the project is on algorithmic clarity, backend design, and correctness, rather than heavy optimization, making the logic easy to reason about and extend.

Highlights:
- Graph traversal with iterative DFS
- Route evaluation based on accumulated weights
- Clean service-oriented backend design
- Dependency Injection and SOLID principles
- .NET 6 REST API
- Deterministic and testable logic

Request:
{% raw %}

```json
{
  "cities": ["A", "B", "C", "D"],
  "roads": [
    {"from": "A", "to": "B", "time": 10},
    {"from": "B", "to": "C", "time": 15},
    {"from": "A", "to": "C", "time": 30},
    {"from": "C", "to": "D", "time": 5},
    {"from": "B", "to": "D", "time": 25}
  ],
  "origin": "A",
  "destination": "D"
}
```

{% endraw %}


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj-route-diagram.png" title="diagram" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Graph-based route evaluation showing alternative paths and the selected optimal route.
</div>

Response:
{% raw %}

```json
{
  "route": ["A", "B", "C", "D"],
  "totalTime": 30
}
```

{% endraw %}



