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

The project was developed from December 2022, focusing on making infrastructure code generation more accessible and reliable through AI technology.
