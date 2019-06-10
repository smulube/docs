---
title: Create a New Project
weight: 5
menu:
  quickstart:
    parent: kubernetes
    identifier: kubernetes-create-project
---

Let's get started with a new project in a new directory.

{{< langchoose nogo >}}

<div class="language-prologue-javascript"></div>

```bash
$ mkdir quickstart && cd quickstart
$ pulumi new kubernetes-javascript
```

<div class="language-prologue-typescript"></div>

```bash
$ mkdir quickstart && cd quickstart
$ pulumi new kubernetes-typescript
```

<div class="language-prologue-python"></div>

```bash
$ mkdir quickstart && cd quickstart
$ pulumi new kubernetes-python
```

> If this is your first time running `pulumi new` (or most other `pulumi` commands), you will be prompted to login to the [Pulumi service](https://app.pulumi.com). The CLI works in tandem with the Pulumi service to deliver a reliable experience, and is free for individual use, with [additional features available for teams](https://www.pulumi.com/pricing/). Hitting enter at the prompt will open a web browser allowing you to sign in or sign up. Alternatively, you may [login]({{< relref "/reference/cli/pulumi_login.md" >}}) or [logout]({{< relref "/reference/cli/pulumi_logout.md" >}}) explicitly if you prefer. See the [FAQ]({{< relref "/reference/faq.md#can-i-use-pulumi-without-depending-on-pulumi-com" >}}) for more information.

[TODO SCREENSHOT OF NEW PROJECT PROMPTS]

TODO As part of describing the `pulumi new` prompts,  explain what projects and stacks are in 1-2 sentences each. Until then, here's some standin-in content: What are [projects]({{< relref "/reference/project.md" >}}) and [stacks]({{< relref "/reference/stack.md" >}})? Pulumi projects and stacks are a way to organize Pulumi code. You can consider a Pulumi Project to be analogous to a GitHub repo: a single place for code — and a Stack to be an instance of that code which has separate configuration. For instance, Project Foo may have multiple stacks for Dev, Test, Prod, or perhaps for different cloud configurations (e.g. geographic region). Please [see this guide]({{< relref "/reference/organizing-stacks-projects.md" >}}) for some best practices on organizing your Pulumi projects and stacks.

{{% lang nodejs %}}
After some dependency installations from `npm`, you'll see some files have been generated:
{{% /lang %}}

{{% lang python %}}
You'll see some files have been generated:
{{% /lang %}}

[TODO SCREENSHOT OR SNIPPET OF `ls`]

Let’s look at some of those.

- `Pulumi.yaml` defines the [project]({{< relref "/reference/project.md" >}}).
- `Pulumi.dev.yaml` is the [configuration file]({{< relref "/reference/config.md" >}}) for the stack we initialized.
- {{< langfile >}} is the Pulumi program that defines our stack resources. Let's examine it.

{{< langchoose nogo >}}

```javascript
"use strict";
const k8s = require("@pulumi/kubernetes");

const appLabels = { app: "nginx" };
const deployment = new k8s.apps.v1.Deployment("nginx", {
    spec: {
        selector: { matchLabels: appLabels },
        replicas: 1,
        template: {
            metadata: { labels: appLabels },
            spec: { containers: [{ name: "nginx", image: "nginx" }] }
        }
    }
});
exports.name = deployment.metadata.apply(m => m.name);
```

```typescript
import * as k8s from "@pulumi/kubernetes";

const appLabels = { app: "nginx" };
const deployment = new k8s.apps.v1.Deployment("nginx", {
    spec: {
        selector: { matchLabels: appLabels },
        replicas: 1,
        template: {
            metadata: { labels: appLabels },
            spec: { containers: [{ name: "nginx", image: "nginx" }] }
        }
    }
});
export const name = deployment.metadata.apply(m => m.name);
```

```python
import pulumi
from pulumi_kubernetes.apps.v1 import Deployment

app_labels = { "app": "nginx" }

deployment = Deployment(
    "nginx",
    spec={
        "selector": { "match_labels": app_labels },
        "replicas": 1,
        "template": {
            "metadata": { "labels": app_labels },
            "spec": { "containers": [{ "name": "nginx", "image": "nginx" }] }
        }
    })

pulumi.export("name", deployment.metadata["name"])
```

This Pulumi program creates an NGINX deployment and exports the name of the deployment.

Next, we'll deploy the stack.

{{< get-started-stepper >}}