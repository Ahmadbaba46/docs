---
layout: home
title: Welcome
---

<section id="future" class="main-bg">
  <div class="panel left">
    <img src="/images/logos/p-logo.svg">
    <summary>
      <h1>Welcome to the future</h1>
      <p>Web Components usher in a new era of web development based on encapsulated and interoperable custom elements that extend HTML itself. Built atop these new standards, Polymer makes it easier and faster to create anything from a button to a complete application across desktop, mobile, and beyond.</p>
      <a href="docs/start/getting-the-code.html">
        <paper-button raised unresolved>
          <core-icon icon="archive"></core-icon> Get {{site.project_title}}
        </paper-button>
      </a>
      <a href="https://github.com/polymer">
        <paper-button class="github" unresolved>
          <core-icon icon="social:post-github"></core-icon> View on GitHub
        </paper-button>
      </a>
    </summary>
  </div>
</section>

<section id="examples">
  <div class="panel">

    <div class="example">

      <h2 class="example-header">Create your own elements</h2>

      <div class="example-wrapper" layout horizontal>
        <div class="example-code" two flex>
      {% highlight html %}
<!-- Import Polymer dependency -->
<link rel="import" href="../polymer/polymer.html">

<!-- Register a new tag called proto-element -->
<script>
  Polymer({
    is: "proto-element",
    // add a callback to the element's prototype
    attached: function() {
      this.innerHTML = "I'm a proto-element!"
    }
  });
</script>

<!-- Use your new element -->
<proto-element></proto-element>
      {% endhighlight %}
        </div>
      
        <div class="example-result" layout vertical flex>
          <span>I'm a proto-element!</span>
        </div>

      </div>
      
      <div class="example-caption">
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aspernatur ad molestias esse alias dicta enim eaque neque voluptatum, doloribus provident nihil laudantium commodi quibusdam debitis ex facilis excepturi magnam itaque?</p>
      </div>

    </div>


    <div class="example">

      <h2 class="example-header">Use someone else's elements</h2>
      
      <div class="example-wrapper" layout horizontal>

        <div class="example-code" two flex>
        {% highlight html %}
<!-- Polyfill Web Components support for older browsers -->
<script src="bower_components/webcomponentsjs/webcomponents-lite.min.js"></script>

<!-- Import element -->
<link rel="import" href="components/google-map/google-map.html">

<!-- Use element -->
<google-map lat="37.790" long="-122.390" flex></google-map>
        {% endhighlight %}
        </div>
        
        <div class="example-result" layout vertical flex>
          <link rel="import" href="components/google-map/google-map.html">
          <google-map lat="37.790" long="-122.390" flex></google-map>
        </div>
        
      </div>

      <div class="example-caption">
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aspernatur ad molestias esse alias dicta enim eaque neque voluptatum, doloribus provident nihil laudantium commodi quibusdam debitis ex facilis excepturi magnam itaque?</p>
      </div>

    </div>


    <div class="example">
      
      <h2 class="example-header">Or combine them!</h2>
      
      <div class="example-wrapper" layout horizontal>
        
        <div class="example-code" two flex>
        {% highlight html %}
<!-- Polyfill Web Components support for older browsers -->
<script src="bower_components/webcomponentsjs/webcomponents-lite.min.js"></script>

<!-- Import element -->
<link rel="import" href="components/google-map/google-map.html">

<!-- Use element -->
<google-map lat="37.790" long="-122.390" flex></google-map>
        {% endhighlight %}
        </div>
        
        <div class="example-result" layout vertical flex>
          <link rel="import" href="components/google-map/google-map.html">
          <google-map lat="37.790" long="-122.390" flex></google-map>
        </div>
        
      </div>

      <div class="example-caption">
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aspernatur ad molestias esse alias dicta enim eaque neque voluptatum, doloribus provident nihil laudantium commodi quibusdam debitis ex facilis excepturi magnam itaque?</p>
      </div>

    </div>

  </div>
</section>

<section id="catalog" class="main-purple">
  <div class="panel">
    <summary style="transform: translateZ(0);">
      <h1>Catalog</h1>
      <a href="https://polymer-designer.appspot.com" target="_blank">
        <img src="/images/designer_fadeout.png" alt="Launch the designer tool" title="Launch the designer tool">
      </a>
      <div>
        <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Officia voluptatem, pariatur excepturi nobis expedita.
        </p>
        <a href="https://polymer-designer.appspot.com" target="_blank">
          <paper-button>
            <core-icon icon="arrow-forward"></core-icon> Try it now
          </paper-button>
        </a>
      </div>
    </summary>
  </div>
</section>

{% comment %}
<section id="everything-element" class="main-purple">
  <div class="panel right">
    <summary>
      <h1>Everything is an element</h1>
      <p>From <code>&lt;a&gt;</code> to <code>&lt;select&gt;</code>, elements are the building blocks of HTML. But modern applications have outgrown these built-in elements, forcing app developers to rely on JavaScript frameworks to provide dynamic, custom behavior.  The resulting apps are frequently complex and monolithic; a component developed for one may not work in another.
      <br><br>
      {{site.project_title}} puts elements back at the center of web development. With {{site.project_title}}, you can craft your own HTML elements and compose them into complete, complex applications that are scalable and maintainable.</p>
      <a href="docs/start/everything.html">
        <paper-button>
          <core-icon icon="arrow-forward"></core-icon> Learn more
        </paper-button>
      </a>
    </summary>
    <img src="/images/logos/p-elements.svg">
  </div>
</section>
{% endcomment %}
