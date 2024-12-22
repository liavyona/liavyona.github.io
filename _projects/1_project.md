---
layout: page
title: AIaC
description: Artificial Intelligence Infrastructure-as-Code Generator
img: assets/img/aiac.svg
importance: 1
category: work
related_publications: false
---

# AIaC: AI-Powered Infrastructure as Code

AIaC (Artificial Intelligence Infrastructure-as-Code) is an innovative project that leverages the power of AI to generate infrastructure code. This tool bridges the gap between natural language requirements and production-ready infrastructure code.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/aiac-arch.jpg" title="AIaC Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/aiac-demo.jpg" title="AIaC Demo" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: High-level architecture of AIaC showing the integration between AI models and IaC generators. Right: Demo of AIaC converting natural language to infrastructure code.
</div>

## Core Features

AIaC represents a significant advancement in infrastructure automation, offering:
- Natural language to IaC conversion
- Multi-cloud provider support
- Best practices integration
- Real-time code generation

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/aiac-workflow.jpg" title="AIaC Workflow" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The AIaC workflow: from natural language input to generated infrastructure code.
</div>

## Technical Stack

The project combines cutting-edge technologies:
- Generative AI Models
- Infrastructure as Code frameworks
- Cloud Provider APIs
- DevOps tooling

You can try AIaC today at [aiac.dev](https://aiac.dev). The code is simple to use - just describe your infrastructure needs, and AIaC will generate the corresponding code.

Here's an example of AIaC in action:

{% raw %}
```bash
# Example input
aiac "create an nginx deployment with 3 replicas"

# Generated output
apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-deployment
spec:
  replicas: 3
  selector:
    matchLabels:
      app: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
      - name: nginx
        image: nginx:latest
        ports:
        - containerPort: 80
```
{% endraw %}

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/aiac-results.jpg" title="AIaC Results" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/aiac-stats.jpg" title="AIaC Statistics" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Example results from AIaC showing various infrastructure configurations. Right: Usage statistics and accuracy metrics.
</div>

The project was developed between December 2022 and March 2023, focusing on making infrastructure code generation more accessible and reliable through AI technology.
