
---
title: "DatabaseFirewall"
title_tag: "Resource DatabaseFirewall | Package Digital Ocean"
meta_desc: "Explore the DatabaseFirewall resource of the Digital Ocean package, including examples, input properties, output properties, lookup functions, and supporting types. Provides a DigitalOcean database firewall resource allowing you to restrict"
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Provides a DigitalOcean database firewall resource allowing you to restrict
connections to your database to trusted sources. You may limit connections to
specific Droplets, Kubernetes clusters, or IP addresses.

{{% examples %}}
{{% /examples %}}



## Create a DatabaseFirewall Resource {#create}
{{< chooser language "javascript,typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/#DatabaseFirewall">DatabaseFirewall</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/#DatabaseFirewallArgs">DatabaseFirewallArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">DatabaseFirewall</span><span class="p">(resource_name, opts=None, </span>cluster_id=None<span class="p">, </span>rules=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewDatabaseFirewall<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/v2/go/digitalocean/?tab=doc#DatabaseFirewallArgs">DatabaseFirewallArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/v2/go/digitalocean/?tab=doc#DatabaseFirewall">DatabaseFirewall</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Digitalocean/Pulumi.Digitalocean.DatabaseFirewall.html">DatabaseFirewall</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Digitalocean/Pulumi.DigitalOcean.DatabaseFirewallArgs.html">DatabaseFirewallArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
  
    <dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>
      The unique name of the resource.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/#DatabaseFirewallArgs">DatabaseFirewallArgs</a></span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd>
  
    <dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span>
    </dt>
    <dd>
      Bag of options to control resource&#39;s behavior.
    </dd>
  

</dl>

{{% /choosable %}}

{{% choosable language python %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>resource_name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type">
            <a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">ResourceOptions</a>
        </span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
  
    <dt
        class="property-optional" title="Optional">
        <span>ctx</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span>
    </dt>
    <dd>
      Context object for the current deployment.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>
      The unique name of the resource.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/v2/go/digitalocean/?tab=doc#DatabaseFirewallArgs">DatabaseFirewallArgs</a></span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd>
  
    <dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span>
    </dt>
    <dd>
      Bag of options to control resource&#39;s behavior.
    </dd>
  

</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
  
    <dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>
      The unique name of the resource.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/dotnet/Pulumi.Digitalocean/Pulumi.DigitalOcean.DatabaseFirewallArgs.html">DatabaseFirewallArgs</a></span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd>
  
    <dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>
    </dt>
    <dd>
      Bag of options to control resource&#39;s behavior.
    </dd>
  

</dl>

{{% /choosable %}}

## DatabaseFirewall Resource Properties {#properties}

To learn more about resource properties and how to use them, see [Inputs and Outputs]({{< relref "/docs/intro/concepts/programming-model#outputs" >}}) in the Programming Model docs.

### Inputs

The DatabaseFirewall resource accepts the following [input]({{< relref "/docs/intro/concepts/programming-model#outputs" >}}) properties:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The ID of the target database cluster.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#databasefirewallrule">List&lt;Pulumi.<wbr>Digital<wbr>Ocean.<wbr>Inputs.<wbr>Database<wbr>Firewall<wbr>Rule<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}A rule specifying a resource allowed to access the database cluster. The following arguments must be specified:
- `type` - (Required) The type of resource that the firewall rule allows to access the database cluster. The possible values are: `droplet`, `k8s`, `ip_addr`, or `tag`.
- `value` - (Required) The ID of the specific resource, the name of a tag applied to a group of resources, or the IP address that the firewall rule allows to access the database cluster.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The ID of the target database cluster.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#databasefirewallrule">[]Database<wbr>Firewall<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}A rule specifying a resource allowed to access the database cluster. The following arguments must be specified:
- `type` - (Required) The type of resource that the firewall rule allows to access the database cluster. The possible values are: `droplet`, `k8s`, `ip_addr`, or `tag`.
- `value` - (Required) The ID of the specific resource, the name of a tag applied to a group of resources, or the IP address that the firewall rule allows to access the database cluster.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The ID of the target database cluster.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#databasefirewallrule">Database<wbr>Firewall<wbr>Rule[]</a></span>
    </dt>
    <dd>{{% md %}}A rule specifying a resource allowed to access the database cluster. The following arguments must be specified:
- `type` - (Required) The type of resource that the firewall rule allows to access the database cluster. The possible values are: `droplet`, `k8s`, `ip_addr`, or `tag`.
- `value` - (Required) The ID of the specific resource, the name of a tag applied to a group of resources, or the IP address that the firewall rule allows to access the database cluster.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>cluster_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The ID of the target database cluster.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#databasefirewallrule">List[Database<wbr>Firewall<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}A rule specifying a resource allowed to access the database cluster. The following arguments must be specified:
- `type` - (Required) The type of resource that the firewall rule allows to access the database cluster. The possible values are: `droplet`, `k8s`, `ip_addr`, or `tag`.
- `value` - (Required) The ID of the specific resource, the name of a tag applied to a group of resources, or the IP address that the firewall rule allows to access the database cluster.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}






### Outputs

All [input](#inputs) properties are implicitly available as output properties. Additionally, the DatabaseFirewall resource produces the following output properties:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>id</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>id</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>

</dl>
{{% /choosable %}}







## Look up an Existing DatabaseFirewall Resource {#look-up}

Get an existing DatabaseFirewall resource's state with the given name, ID, and optional extra properties used to qualify the lookup.
{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/#DatabaseFirewallState">DatabaseFirewallState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/#DatabaseFirewall">DatabaseFirewall</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>cluster_id=None<span class="p">, </span>rules=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetDatabaseFirewall<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/v2/go/digitalocean/?tab=doc#DatabaseFirewallState">DatabaseFirewallState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/v2/go/digitalocean/?tab=doc#DatabaseFirewall">DatabaseFirewall</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Digitalocean/Pulumi.Digitalocean.DatabaseFirewall.html">DatabaseFirewall</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Digitalocean/Pulumi.Digitalocean..DatabaseFirewallState.html">DatabaseFirewallState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>resource_name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Optional">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

The following state arguments are supported:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The ID of the target database cluster.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#databasefirewallrule">List&lt;Pulumi.<wbr>Digital<wbr>Ocean.<wbr>Inputs.<wbr>Database<wbr>Firewall<wbr>Rule<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}A rule specifying a resource allowed to access the database cluster. The following arguments must be specified:
- `type` - (Required) The type of resource that the firewall rule allows to access the database cluster. The possible values are: `droplet`, `k8s`, `ip_addr`, or `tag`.
- `value` - (Required) The ID of the specific resource, the name of a tag applied to a group of resources, or the IP address that the firewall rule allows to access the database cluster.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The ID of the target database cluster.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#databasefirewallrule">[]Database<wbr>Firewall<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}A rule specifying a resource allowed to access the database cluster. The following arguments must be specified:
- `type` - (Required) The type of resource that the firewall rule allows to access the database cluster. The possible values are: `droplet`, `k8s`, `ip_addr`, or `tag`.
- `value` - (Required) The ID of the specific resource, the name of a tag applied to a group of resources, or the IP address that the firewall rule allows to access the database cluster.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The ID of the target database cluster.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#databasefirewallrule">Database<wbr>Firewall<wbr>Rule[]</a></span>
    </dt>
    <dd>{{% md %}}A rule specifying a resource allowed to access the database cluster. The following arguments must be specified:
- `type` - (Required) The type of resource that the firewall rule allows to access the database cluster. The possible values are: `droplet`, `k8s`, `ip_addr`, or `tag`.
- `value` - (Required) The ID of the specific resource, the name of a tag applied to a group of resources, or the IP address that the firewall rule allows to access the database cluster.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>cluster_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The ID of the target database cluster.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#databasefirewallrule">List[Database<wbr>Firewall<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}A rule specifying a resource allowed to access the database cluster. The following arguments must be specified:
- `type` - (Required) The type of resource that the firewall rule allows to access the database cluster. The possible values are: `droplet`, `k8s`, `ip_addr`, or `tag`.
- `value` - (Required) The ID of the specific resource, the name of a tag applied to a group of resources, or the IP address that the firewall rule allows to access the database cluster.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Supporting Types


<h4 id="databasefirewallrule">Database<wbr>Firewall<wbr>Rule</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/types/input/#DatabaseFirewallRule">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/types/output/#DatabaseFirewallRule">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/v2/go/digitalocean/?tab=doc#DatabaseFirewallRuleArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/v2/go/digitalocean/?tab=doc#DatabaseFirewallRuleOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Value</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Created<wbr>At</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The date and time when the firewall rule was created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Uuid</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}A unique identifier for the firewall rule.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Value</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Created<wbr>At</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The date and time when the firewall rule was created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Uuid</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}A unique identifier for the firewall rule.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>value</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>created<wbr>At</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The date and time when the firewall rule was created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>uuid</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}A unique identifier for the firewall rule.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>value</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>created_<wbr>at</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The date and time when the firewall rule was created.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>uuid</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}A unique identifier for the firewall rule.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}









<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-digitalocean">https://github.com/pulumi/pulumi-digitalocean</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
	<dt>Notes</dt>
	<dd>This Pulumi package is based on the [`digitalocean` Terraform Provider](https://github.com/terraform-providers/terraform-provider-digitalocean).</dd>
</dl>

