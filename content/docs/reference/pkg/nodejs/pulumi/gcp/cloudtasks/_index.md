---
title: "Module cloudtasks"
title_tag: "Module cloudtasks | Package @pulumi/gcp | Node.js SDK"
linktitle: "cloudtasks"
meta_desc: "Explore members of the cloudtasks module in the @pulumi/gcp package."
git_sha: "d3b2de3ae90cda70422191c8ff6c2cd143ff4724"
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->


> This provider is a derived work of the [Terraform Provider](https://github.com/terraform-providers/terraform-provider-google-beta)
> distributed under [MPL 2.0](https://www.mozilla.org/en-US/MPL/2.0/). If you encounter a bug or missing feature,
> first check the [`pulumi/pulumi-gcp` repo](https://github.com/pulumi/pulumi-gcp/issues); however, if that doesn't turn up anything,
> please consult the source [`terraform-providers/terraform-provider-google-beta` repo](https://github.com/terraform-providers/terraform-provider-google-beta/issues).





<h3>Resources</h3>
<ul class="api">
    <li><a href="#Queue"><span class="symbol resource"></span>Queue</a></li>
</ul>


<h3>Others</h3>
<ul class="api">
    <li><a href="#QueueArgs"><span class="symbol api"></span>QueueArgs</a></li>
    <li><a href="#QueueState"><span class="symbol api"></span>QueueState</a></li>
</ul>


<h2 id="resources">Resources</h2>
<h3 class="pdoc-module-header" id="Queue" data-link-title="Queue">
    <a href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L12">
        Resource <strong>Queue</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>class</span> <span class='nx'>Queue</span> <span class='kr'>extends</span> <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></code></pre>

> This content is derived from https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/cloud_tasks_queue.html.markdown.

<h4 class="pdoc-member-header" id="Queue-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L66"> <b>constructor</b></a>
</h4>


<pre class="highlight"><code><span class='kd'></span><span class='kd'>new</span> Queue(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args: <a href='#QueueArgs'>QueueArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</code></pre>


Create a Queue resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

<h4 class="pdoc-member-header" id="Queue-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L21">method <b>get</b></a>
</h4>


<pre class="highlight"><code><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, state?: <a href='#QueueState'>QueueState</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#Queue'>Queue</a></code></pre>


Get an existing Queue resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

<h4 class="pdoc-member-header" id="Queue-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L12">method <b>getProvider</b></a>
</h4>


<pre class="highlight"><code><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ProviderResource'>ProviderResource</a> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></code></pre>

<h4 class="pdoc-member-header" id="Queue-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L32">method <b>isInstance</b></a>
</h4>


<pre class="highlight"><code><span class='kd'>public static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): obj is Queue</code></pre>


Returns true if the given object is an instance of Queue.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

<h4 class="pdoc-member-header" id="Queue-appEngineRoutingOverride">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L42">property <b>appEngineRoutingOverride</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>appEngineRoutingOverride: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/gcp/types/output/#QueueAppEngineRoutingOverride'>QueueAppEngineRoutingOverride</a> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</code></pre>

Overrides for task-level appEngineRouting. These settings apply only to App Engine tasks in this queue

<h4 class="pdoc-member-header" id="Queue-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L12">property <b>id</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</code></pre>

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

<h4 class="pdoc-member-header" id="Queue-location">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L46">property <b>location</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>location: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The location of the queue

<h4 class="pdoc-member-header" id="Queue-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L50">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>name: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The queue name.

<h4 class="pdoc-member-header" id="Queue-project">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L55">property <b>project</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>project: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.

<h4 class="pdoc-member-header" id="Queue-rateLimits">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L62">property <b>rateLimits</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>rateLimits: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/gcp/types/output/#QueueRateLimits'>QueueRateLimits</a>&gt;;</code></pre>

Rate limits for task dispatches. The queue's actual dispatch rate is the result of: * Number of tasks in the queue *
User-specified throttling: rateLimits, retryConfig, and the queue's state. * System throttling due to 429 (Too Many
Requests) or 503 (Service Unavailable) responses from the worker, high error rates, or to smooth sudden large
traffic spikes.

<h4 class="pdoc-member-header" id="Queue-retryConfig">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L66">property <b>retryConfig</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>retryConfig: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/gcp/types/output/#QueueRetryConfig'>QueueRetryConfig</a>&gt;;</code></pre>

Settings that determine the retry behavior.

<h4 class="pdoc-member-header" id="Queue-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L12">property <b>urn</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>urn: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</code></pre>

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.



<h2 id="apis">Others</h2>
<h3 class="pdoc-module-header" id="QueueArgs" data-link-title="QueueArgs">
    <a href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L146">
        interface <strong>QueueArgs</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>QueueArgs</span></code></pre>

The set of arguments for constructing a Queue resource.

<h4 class="pdoc-member-header" id="QueueArgs-appEngineRoutingOverride">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L150">property <b>appEngineRoutingOverride</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>appEngineRoutingOverride?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/gcp/types/input/#QueueAppEngineRoutingOverride'>QueueAppEngineRoutingOverride</a>&gt;;</code></pre>

Overrides for task-level appEngineRouting. These settings apply only to App Engine tasks in this queue

<h4 class="pdoc-member-header" id="QueueArgs-location">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L154">property <b>location</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>location: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The location of the queue

<h4 class="pdoc-member-header" id="QueueArgs-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L158">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The queue name.

<h4 class="pdoc-member-header" id="QueueArgs-project">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L163">property <b>project</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>project?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.

<h4 class="pdoc-member-header" id="QueueArgs-rateLimits">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L170">property <b>rateLimits</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>rateLimits?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/gcp/types/input/#QueueRateLimits'>QueueRateLimits</a>&gt;;</code></pre>

Rate limits for task dispatches. The queue's actual dispatch rate is the result of: * Number of tasks in the queue *
User-specified throttling: rateLimits, retryConfig, and the queue's state. * System throttling due to 429 (Too Many
Requests) or 503 (Service Unavailable) responses from the worker, high error rates, or to smooth sudden large
traffic spikes.

<h4 class="pdoc-member-header" id="QueueArgs-retryConfig">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L174">property <b>retryConfig</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>retryConfig?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/gcp/types/input/#QueueRetryConfig'>QueueRetryConfig</a>&gt;;</code></pre>

Settings that determine the retry behavior.

<h3 class="pdoc-module-header" id="QueueState" data-link-title="QueueState">
    <a href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L112">
        interface <strong>QueueState</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>QueueState</span></code></pre>

Input properties used for looking up and filtering Queue resources.

<h4 class="pdoc-member-header" id="QueueState-appEngineRoutingOverride">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L116">property <b>appEngineRoutingOverride</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>appEngineRoutingOverride?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/gcp/types/input/#QueueAppEngineRoutingOverride'>QueueAppEngineRoutingOverride</a>&gt;;</code></pre>

Overrides for task-level appEngineRouting. These settings apply only to App Engine tasks in this queue

<h4 class="pdoc-member-header" id="QueueState-location">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L120">property <b>location</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>location?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The location of the queue

<h4 class="pdoc-member-header" id="QueueState-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L124">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The queue name.

<h4 class="pdoc-member-header" id="QueueState-project">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L129">property <b>project</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>project?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.

<h4 class="pdoc-member-header" id="QueueState-rateLimits">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L136">property <b>rateLimits</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>rateLimits?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/gcp/types/input/#QueueRateLimits'>QueueRateLimits</a>&gt;;</code></pre>

Rate limits for task dispatches. The queue's actual dispatch rate is the result of: * Number of tasks in the queue *
User-specified throttling: rateLimits, retryConfig, and the queue's state. * System throttling due to 429 (Too Many
Requests) or 503 (Service Unavailable) responses from the worker, high error rates, or to smooth sudden large
traffic spikes.

<h4 class="pdoc-member-header" id="QueueState-retryConfig">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/{{< param git_sha >}}/sdk/nodejs/cloudtasks/queue.ts#L140">property <b>retryConfig</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>retryConfig?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/gcp/types/input/#QueueRetryConfig'>QueueRetryConfig</a>&gt;;</code></pre>

Settings that determine the retry behavior.
