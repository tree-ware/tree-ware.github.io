---
template: reveal.html
---

<section>
    <h1>Tree-Ware Introduction</h1>
    <p>Accelerate your software development!</p>
</section>

<section>
    <h1>The Problem</h1>
    <section>Companies struggle with feature velocity</section>
    <section>They use a lot of open-source software to speed up their development</section>
    <section>But that alone is <b>NOT</b> sufficient!</section>

    <section>Every feature requires a lot of cross-cutting aspects to be implemented</section>
    <section>UI for user-input and feature-metrics</section>
    <section>APIs for user input and feature metrics</section>
    <section>RBAC for the APIs</section>
    <section>Caching</section>
    <section>Storage for user input and feature metrics</section>
    <section>Full-text search</section>
    <section>Rolling up of feature metrics across space & time</section>
    <section>And a lot more such cross-cutting aspects</section>

    <section>There is open-source software for each of the above, but they need to be glued together for each feature</section>

    <section>New features require glue-logic for cross-cutting aspects</section>
    <section>New cross-cutting aspects require updates in existing features</section>

    <section>
        <p>The initial rush-to-market results in</p>
        <p>many of the cross-cutting aspects being left out</p>
        <p>and inconsistently implemented features</p>
    </section>
    <section>Inconsistent feature implementations make it hard to add new cross-cutting aspects</section>
</section>

<section>
    <h1>The Solution</h1>
    <section>
        <h2>tree-ware</h2>
        An end-to-end declarative open-source framework
    </section>
    <section>
        <p><b>End-to-end</b></p>
        <p>UIs, APIs, load-balancers, caches, databases, compute-pipelines, devices</p>
    </section>
    <section>
        <p><b>Declarative</b></p>
        <p><b>System-wide</b> schema specified by developers</p>
    </section>
    <section>
        <p><b>Open-source</b></p>
        <p><a href="https://github.com/tree-ware">https://github.com/tree-ware</a></p>
    </section>
    <section>
        <p>Tree-ware lets you rush-to-market</p>
        <p>with a slew of cross-cutting aspects included out of the box</p>
        <p>and consistently implemented features</p>
    </section>
    <section>New features automatically get cross-cutting aspects from tree-ware</section>
    <section>New cross-cutting aspects do NOT require updates in existing features</section>
</section>

<section>
    <h1>Work Involved?</h1>
    <section>
        <p>Developers only define the following:</p>
        <ol>
            <li>a schema for the product/service data</li>
            <li>custom business-logic</li>
        </ol>
    </section>
    <section>Tree-ware takes care of everything else</section>
</section>

<section>
    <h1>How Does it Work?</h1>
    <section>Tree-ware uses a <b>data-first</b> approach</section>
    <section>Developers define the data corresponding to the features</section>
    <section>And tree-ware provides the cross-cutting aspects</section>
    <section>
        <p>It sets up & operates infrastructure</p>
        <p><b><i>for</i></b></p>
        <p>the data defined in the schema</p>
    </section>
    <section>It provides the glue-logic for the necessary infrastructure</section>
    <section>
        <p>It uses existing infrastructure:</p>
        <p>Databases, queues, compute-pipelines, etc.</p>
    </section>
    <section>
        <p>And provides other custom infrastructure:</p>
        <p>UI, load-balancer, API server, cache, RBAC, feature-flags, etc.</p>
    </section>
</section>

<section><img src="/presentations/block-diagram.drawio.svg"></section>

<!--
<section>
    <h1>Is this No-Code?</h1>
    <section>Yes and No</section>
    <section>
        <h2>No</h2>
        Targeted at developers, not non-developers
    </section>
    <section>Designed for building production systems</section>
    <section>
        <h2>Yes</h2>
        Requires no code or a low amount of code
    </section>
    <section>
        <p>Non-developers can build features</p>
        <p><b><i>after</i></b></p>
        <p>developers build products with tree-ware</p>
    </section>
</section>
-->

<section>
    <h1>Common Concerns</h1>
    <section>Tree-ware has solved common concerns people have with such frameworks</section>
    <section>What if I want to do something the framework does not support?</section>
    <section>
        <p>Tree-ware does not limit what can be done</p>
        <p>It is modular and custom code can be inserted wherever needed</p>
    </section>
    <section>How do I prevent the framework from overwriting my manually written code?</section>
    <section>Tree-ware generated code and manually written code do not exist in the same files</section>
    <section>Can it scale?</section>
    <section>Tree-ware was built from the ground up for scale</section>
</section>

<section>
    <h1>What's the Catch?</h1>
    <section>
        <p>It is less than ideal for existing systems</p>
        <p>But it is perfect for brand new systems</p>
    </section>
    <section>
        <p>It is not fully implemented</p>
        <p>But there is enough for a first release</p>
        <p>And it is a great foundation to build on</p>
    </section>
</section>

<section>
    <h1>Recap</h1>
    <section>Tree-ware accelerates feature development by taking care of all cross-cutting aspects</section>
    <section>
        <p>Developers only define the following:</p>
        <ol>
            <li>a schema for the product/service data</li>
            <li>custom business-logic</li>
        </ol>
    </section>
    <section>New cross-cutting aspects can be added WITHOUT modifying existing features</section>
</section>

<section><h1>The End</h1></section>
