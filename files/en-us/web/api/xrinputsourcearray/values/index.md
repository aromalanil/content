---
title: XRInputSourceArray.values()
slug: Web/API/XRInputSourceArray/values
tags:
- API
- AR
- Input Sources
- Inputs
- Iterator
- Method
- Mixed
- Reality
- Reference
- Sources
- VR
- Virtual
- WebXR
- WebXR API
- WebXR API Reference
- XR
- XRInputSourceArrray
- augmented
- values
browser-compat: api.XRInputSourceArray.values
---
<p>{{APIRef("WebXR Device API")}}</p>

<p>The {{domxref("XRInputSourceArray")}}
  method  <code><strong>values()</strong></code> returns a {{Glossary("JavaScript")}}
  <code><a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects/Iterator">iterator</a></code>
  that can walk over the list of {{domxref("XRInputSource")}} objects contained in the
  array, from first to last.</p>

<h2 id="Syntax">Syntax</h2>

<pre class="brush: js"><em>xrInputSourceArray</em>.values();
</pre>

<h3 id="Parameters">Parameters</h3>

<p>None.</p>

<h3 id="Return_value">Return value</h3>

<p>A
  JavaScript <code><a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects/Iterator">iterator</a></code> that
  can be used to walk through the list of {{domxref("XRInputSource")}} objects in the
  array, starting with the first entry (at index 0) and proceeding straight through the
  list.</p>

<h2 id="Examples">Examples</h2>

<p>This example snippet walks through each input and calls the
  function <code>checkInput()</code>  with each returned value.</p>

<pre class="brush: js">for (const source of xrSession.inputSources.values()) {
  checkInput(source);
}
</pre>

<p>Here,
  <code><a href="/en-US/docs/Web/JavaScript/Reference/Statements/for...of">for...of</a></code>
  is used to iterate over the array's contents. Each pass through the loop,
  <code>source</code> is the next {{domxref("XRInputSource")}} in the list. The loop exits
  once every input has been delivered to <code>checkInput()</code>.</p>

<h2 id="Specifications">Specifications</h2>

{{Specifications}}

<h2 id="Browser_compatibility">Browser compatibility</h2>

<p>{{Compat}}</p>

<h2 id="See_also">See also</h2>

<ul>
  <li><a href="/en-US/docs/Web/API/WebXR_Device_API/Inputs">Inputs and input sources</a>
  </li>
  <li>The {{domxref("XRInputSourceArray")}} method {{domxref("XRInputSourceArray.keys",
    "keys()")}}</li>
  <li>The
    <code><a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array">Array</a></code> method <code><a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/values">values(</a>)</code>
  </li>
  <li>{{domxref("XRInputSource")}}</li>
</ul>