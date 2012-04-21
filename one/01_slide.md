!SLIDE
<h1 style="font-size: 5.2em">Progressive Enhancement<br/><span style="font-size: 0.9em">on the mobile web</span></h1>
johnbender.github.com/presentation-jqm-rails

!SLIDE bullets mono-bullets
## Me
* @johnbender
* johnbender.us
* github.com/johnbender

!SLIDE center adobe-background
## Jquery Mobile

!SLIDE center
## Vagrant
vagrantup.com

!SLIDE
## Emojicons.com

!SLIDE
<h2 class="blur">Emojicons.com</h2>
<div class="gigantor squished" style="font-size: 12em;">ლ(ಠ益ಠლ)</div>

!SLIDE
# Jquery Mobile
### \|°▿▿▿▿°|/

!SLIDE
## Users
no one uses this crap

!SLIDE bullets grid users
<div style="float: left; margin-left: 100px">
<ul>
  <li> Sears </li>
  <li> Chase </li>
  <li> Ikea </li>
  <li> Life </li>
  <li> Stanford </li>
</ul>
</div>

<div style="float: left">
<ul>
  <li> m.sears.com </li>
  <li> m.chase.com </li>
  <li> m.ikea.com </li>
  <li> m.life.com </li>
  <li> m.stanford.edu </li>
</ul>
</div>

!SLIDE bullets grid users
<div style="float: left; margin-left: 100px">
<ul>
  <li>Sears </li>
  <li>Chase </li>
  <li>Ikea </li>
  <li> Life </li>
  <li style="color: red">Stanford </li>
</ul>
</div>
<div style="float: left">
<ul>
  <li>m.sears.com </li>
  <li>m.chase.com </li>
  <li>m.ikea.com </li>
  <li> m.life.com </li>
  <li style="color: red">m.stanford.edu</li>
</ul>
</div>

!SLIDE
## Browser Support

!SLIDE bullets grid
<div style="float: left;  margin-top: 200px">
<ul>
  <li> Apple iOS 3.2-5.0 </li>
  <li> Android 2.1-4.0 </li>
  <li> Windows Phone 7-7.5 </li>
  <li> Blackberry 6-7, QNX </li>
  <li> Palm WebOS 1.4-3.0 </li>
</ul>
</div>

<div style="float: left; margin-bottom: 100px; margin-top: 200px">
<ul>
  <li> Firebox Mobile </li>
  <li> Opera Mobile 11.0 </li>
  <li> Meego 1.2 </li>
  <li> Chrome, Firefox </li>
  <li> IE 7+, Opera 10+ </li>
</ul>
</div>
jquerymobile.com/gbs/

!SLIDE
## Quick Stats
### (=O*_*)=O Q(*_*Q)

!SLIDE
### github
6000+ watchers • 1000+ forks

!SLIDE
### books
8 books • 7 publishers

!SLIDE
### sentiment
news.ycombinator.com/item?id=3549640

!SLIDE
<h1 style="font-size: 5.2em">Progressive Enhancement</h1>
### ( ˘ ³˘)♥

!SLIDE
## Webkit! amiright?!

!SLIDE
<h2 class="blur">Webkit! amiright?!</h2>
<div class="gigantor squished" style="font-size: 13em;">(ﾉಥ益ಥ）ﾉ</div>

!SLIDE
<h3 style="font-size: 6.0em">gazillions of devices</h3>
usage doubled to 8.5% from '11 to '12

!SLIDE center
<img src="mobile-browser-stats.jpg" class="tweak-img" style="width: 90%; top: 80px; margin-left: 4%;"></img>

!SLIDE
### history
(push|pop|replace)State

!SLIDE
### orientation
180&#176;? 90&#176;? 0&#176;? 270&#176;?

!SLIDE
### tap vs click
don't scroll, you'll be sorry

!SLIDE high-image center
<img src="droidincredible.jpg" style="height: 500px; float: left; margin-left: 155px;"></img>
<img src="blackberry-bold.jpg" style="height: 480px; float: left; margin-top: 10px;"></img>

!SLIDE
### web views
each browser x 2

!SLIDE
## Android

!SLIDE
<h2 class="blur">Android</h2>
<div class="gigantor" style="font-size: 18em; top: -50px">(╥﹏╥)</div>

!SLIDE
### <img src="android-icon.png"></img> is the new <img src="ie-icon.png"></img>
inflammatory statements at railsconf

!SLIDE
### 2.2, 2.3.3
80+% percent of androids

!SLIDE
### rendering
yes, even rendering

!SLIDE
### position fixed
we use &amp;nbsp; to fix bugs

!SLIDE
### transitions
toy examples work great

!SLIDE
# Jqm on Rails
### ʕノ•ᴥ•ʔノ ︵ ┻━┻

!SLIDE
## Sample app
github.com/johnbender/jqm-rails

!SLIDE
### office presence
sign up • sign in • status

!SLIDE center
<div class="rotate-left" style="top: 170px;"><h3>Presence</h3></div>
<iframe class="phone-center" src="http://33.33.33.10:3000/sessions/new"> </iframe>

!SLIDE
## setting up

!SLIDE
<div class="file-name">app/views/layouts/application.html.erb</div>
<pre style="font-size: 2.3em;">
&lt;<span class="function-name">link</span> <span class="variable-name">rel</span>=<span class="string">"stylesheet"</span> <span class="variable-name">href</span>=<span class="string">"$CDN/jquery.mobile.css"</span>/&gt;
&lt;<span class="function-name">script</span> <span class="variable-name">src</span>=<span class="string">"$CDN/jquery-1.6.4.min.js"</span>&gt;&lt;/<span class="function-name">script</span>&gt;
&lt;<span class="function-name">script</span> <span class="variable-name">src</span>=<span class="string">"$CDN/jquery.mobile.js"</span>&gt;&lt;/<span class="function-name">script</span>&gt;
</pre>

!SLIDE
<div class="file-name">app/views/layouts/application.html.erb</div>
<pre style="font-size: 2.3em;">
&lt;<span class="function-name">meta</span> <span class="variable-name">name</span>=<span class="string">"viewport"</span>
      <span class="variable-name">content</span>=<span class="string">"width=device-width, initial-scale=1"</span>&gt;
&lt;%= stylesheet_link_tag <span class="string">"application"</span> %&gt;
&lt;%= javascript_include_tag <span class="string">"application"</span> %&gt;
&lt;<span class="function-name">script</span> <span class="variable-name">src</span>=<span class="string">"$CDN/jquery.mobile.css"</span>&gt;&lt;/<span class="function-name">script</span>&gt;
&lt;<span class="function-name">script</span> <span class="variable-name">src</span>=<span class="string">"$CDN/jquery.mobile.js"</span>&gt;&lt;/<span class="function-name">script</span>&gt;
</pre>

!SLIDE
<div class="file-name">app/views/layouts/application.html.erb</div>
<pre style="font-size: 2.3em;">
<b>&lt;<span class="function-name">meta</span> <span class="variable-name">name</span>=<span class="string">"viewport"</span></b>
      <b><span class="variable-name">content</span>=<span class="string">"width=device-width, initial-scale=1"</span>&gt;</b>
&lt;%= stylesheet_link_tag <span class="string">"application"</span> %&gt;
&lt;%= javascript_include_tag <span class="string">"application"</span> %&gt;
&lt;<span class="function-name">script</span> <span class="variable-name">src</span>=<span class="string">"$CDN/jquery.mobile.css"</span>&gt;&lt;/<span class="function-name">script</span>&gt;
&lt;<span class="function-name">script</span> <span class="variable-name">src</span>=<span class="string">"$CDN/jquery.mobile.js"</span>&gt;&lt;/<span class="function-name">script</span>&gt;
</pre>

!SLIDE
<div class="file-name">app/views/layouts/application.html.erb</div>
<pre style="font-size: 2.3em;">
&lt;<span class="function-name">meta</span> <span class="variable-name">name</span>=<span class="string">"viewport"</span>
     <span class="variable-name">content</span>=<span class="string">"width=device-width, initial-scale=1"</span>&gt;
<b>&lt;%= stylesheet_link_tag <span class="string">"application"</span> %&gt;</b>
<b>&lt;%= javascript_include_tag <span class="string">"application"</span> %&gt;</b>
&lt;<span class="function-name">script</span> <span class="variable-name">src</span>=<span class="string">"$CDN/jquery.mobile.css"</span>&gt;&lt;/<span class="function-name">script</span>&gt;
&lt;<span class="function-name">script</span> <span class="variable-name">src</span>=<span class="string">"$CDN/jquery.mobile.js"</span>&gt;&lt;/<span class="function-name">script</span>&gt;
</pre>

!SLIDE
<div class="file-name">app/views/layouts/application.html.erb</div>
<pre style="font-size: 2.3em;">
&lt;<span class="function-name">meta</span> <span class="variable-name">name</span>=<span class="string">"viewport"</span>
     <span class="variable-name">content</span>=<span class="string">"width=device-width, initial-scale=1"</span>&gt;
&lt;%= stylesheet_link_tag <span class="string">"application"</span> %&gt;
&lt;%= javascript_include_tag <span class="string">"application"</span> %&gt;
<b>&lt;<span class="function-name">script</span> <span class="variable-name">src</span>=<span class="string">"$CDN/jquery.mobile.css"</span>&gt;&lt;/<span class="function-name">script</span>&gt;</b>
<b>&lt;<span class="function-name">script</span> <span class="variable-name">src</span>=<span class="string">"$CDN/jquery.mobile.js"</span>&gt;&lt;/<span class="function-name">script</span>&gt;</b>
</pre>


!SLIDE
## page options
page ∈ layout <span style="font-size: 1.2em">⋁</span> page ∈ view

!SLIDE
### layout
views rendered into jqm page

!SLIDE
<div class="file-name">app/views/layouts/application.html.erb</div>
<pre class="medium">
&lt;<span class="function-name">body</span>&gt;
  &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"page"</span>&gt;
    &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"header"</span>&gt;
      &lt;<span class="function-name">h1</span>&gt;&lt;%= yield :heading %&gt;&lt;/<span class="function-name">h1</span>&gt;
    &lt;/<span class="function-name">div</span>&gt;

    &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"content"</span>&gt;
      &lt;%= yield %&gt;
    &lt;/<span class="function-name">div</span>&gt;
  &lt;/<span class="function-name">div</span>&gt;
&lt;/<span class="function-name">body</span>&gt;
</pre>

!SLIDE
<div class="file-name">app/views/layouts/application.html.erb</div>
<pre class="medium">
&lt;<span class="function-name">body</span>&gt;
  <b>&lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"page"</span>&gt;</b>
    &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"header"</span>&gt;
      &lt;<span class="function-name">h1</span>&gt;&lt;%= yield :heading %&gt;&lt;/<span class="function-name">h1</span>&gt;
    &lt;/<span class="function-name">div</span>&gt;

    &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"content"</span>&gt;
      &lt;%= yield %&gt;
    &lt;/<span class="function-name">div</span>&gt;
  &lt;/<span class="function-name">div</span>&gt;
&lt;/<span class="function-name">body</span>&gt;
</pre>

!SLIDE
<div class="file-name">app/views/layouts/application.html.erb</div>
<pre class="medium">
&lt;<span class="function-name">body</span>&gt;
  &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"page"</span>&gt;
    &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"header"</span>&gt;
      &lt;<span class="function-name">h1</span>&gt;&lt;%= yield :heading %&gt;&lt;/<span class="function-name">h1</span>&gt;
    &lt;/<span class="function-name">div</span>&gt;

    &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"content"</span>&gt;
      <b>&lt;%= yield %&gt;</b>
    &lt;/<span class="function-name">div</span>&gt;
  &lt;/<span class="function-name">div</span>&gt;
&lt;/<span class="function-name">body</span>&gt;
</pre>

!SLIDE
### partial
views render their own pages

!SLIDE
<div class="file-name">app/views/layouts/application.html.erb</div>
<pre class="medium">
&lt;<span class="function-name">body</span>&gt;
  &lt;%= yield %&gt;
&lt;/<span class="function-name">body</span>&gt;
</pre>

!SLIDE
<div class="file-name">app/views/shared/_page.html.erb</div>
<pre class="medium">
&lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"page"</span>&gt;
  &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"header"</span>&gt;
    &lt;<span class="function-name">h1</span>&gt;&lt;%= h1 %&gt;&lt;/<span class="function-name">h1</span>&gt;
  &lt;/<span class="function-name">div</span>&gt;

  &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"content"</span>&gt;
    &lt;%= yield %&gt;
  &lt;/<span class="function-name">div</span>&gt;
&lt;/<span class="function-name">div</span>&gt;
</pre>


!SLIDE
<div class="file-name">app/views/shared/sample.html.erb</div>
<pre class="medium">
&lt;% render <span class="constant">:layout</span> =&gt; <span class="string">'shared/page'</span>,
          <span class="constant">:locals</span> =&gt; { <span class="constant">:h1</span> =&gt; <span class="string">"foo"</span> } <span class="keyword">do</span> %&gt;
  &lt;<span class="function-name">div</span>&gt;The Content&lt;/<span class="function-name">div</span>&gt;
&lt;% <span class="keyword">end</span> %&gt;
</pre>

!SLIDE
## data-* names
jquery-rails data attributes

!SLIDE
<span style="font-family: monospace; font-size: 2.0em">$ grep data- jquery_ujs.js</span>

!SLIDE
<div class="file-name">app/assets/javascripts/application.js</div>
<pre class="medium">
<span class="comment">//= require jquery
//= require jquery_ujs
//= require .
</span>$( document ).on( <span class="string">"mobileinit"</span>, <span class="keyword">function</span>() {
  <span class="js2-external-variable">$</span>.mobile.ns = <span class="string">"foo-"</span>;
});
</pre>

!SLIDE
<div class="file-name">app/assets/javascripts/application.js</div>
<pre class="medium">
<span class="comment">//= require jquery
//= require jquery_ujs
//= require .
</span>$( document ).on( <b><span class="string">"mobileinit"</span></b>, <span class="keyword">function</span>() {
  <span class="js2-external-variable">$</span>.mobile.ns = <span class="string">"foo-"</span>;
});
</pre>

!SLIDE
<div class="file-name">app/assets/javascripts/application.js</div>
<pre class="medium">
<span class="comment"><b>//= require jquery</b>
//= require jquery_ujs
//= require .
</span>$( document ).on( <span class="string">"mobileinit"</span>, <span class="keyword">function</span>() {
  <span class="js2-external-variable">$</span>.mobile.ns = <span class="string">"foo-"</span>;
});
</pre>

!SLIDE
<div class="file-name">app/views/layouts/application.html.erb</div>
<pre style="font-size: 2.3em;">
&lt;<span class="function-name">meta</span> <span class="variable-name">name</span>=<span class="string">"viewport"</span>
      <span class="variable-name">content</span>=<span class="string">"width=device-width, initial-scale=1"</span>&gt;
&lt;%= stylesheet_link_tag <span class="string">"application"</span> %&gt;
<b>&lt;%= javascript_include_tag <span class="string">"application"</span> %&gt;</b>
&lt;<span class="function-name">script</span> <span class="variable-name">src</span>=<span class="string">"$CDN/jquery.mobile.css"</span>&gt;&lt;/<span class="function-name">script</span>&gt;
<b>&lt;<span class="function-name">script</span> <span class="variable-name">src</span>=<span class="string">"$CDN/jquery.mobile.js"</span>&gt;&lt;/<span class="function-name">script</span>&gt;</b>
</pre>

!SLIDE
## form validation
generally, reposting to the same url

!SLIDE
### multipage
existing loaded pages

!SLIDE
<div class="file-name">app/views/foos/index.html.erb*, app/views/bars/index.html.erb*</div>
<pre class="large">
&lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"page"</span> <span class="variable-name">data-url</span>=<span class="string">"/foos"</span>&gt;
  &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"content"</span>&gt;
    All the Foos
  &lt;/<span class="function-name">div</span>&gt;
&lt;/<span class="function-name">div</span>&gt;

&lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"page"</span> <span class="variable-name">data-url</span>=<span class="string">"/bars"</span>&gt;
  &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"content"</span>&gt;
    &lt;<span class="function-name">a</span> <span class="variable-name">href</span>=<span class="string">"/foos"</span>&gt;Go to Foos&lt;/<span class="function-name">a</span>&gt;
    All the Bars
  &lt;/<span class="function-name">div</span>&gt;
&lt;/<span class="function-name">div</span>&gt;</pre>

!SLIDE
<div class="file-name">app/views/foos/index.html.erb*, app/views/bars/index.html.erb*</div>
<pre class="large">
&lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"page"</span> <span class="variable-name">data-url</span>=<span class="string">"/foos"</span>&gt;
  &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"content"</span>&gt;
    All the Foos
  &lt;/<span class="function-name">div</span>&gt;
&lt;/<span class="function-name">div</span>&gt;

&lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"page"</span> <span class="variable-name">data-url</span>=<span class="string">"/bars"</span>&gt;
  &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"content"</span>&gt;
    <b>&lt;<span class="function-name">a</span> <span class="variable-name">href</span>=<span class="string">"/foos"</span>&gt;Go to Foos&lt;/<span class="function-name">a</span>&gt;</b>
    All the Bars
  &lt;/<span class="function-name">div</span>&gt;
&lt;/<span class="function-name">div</span>&gt;</pre>

!SLIDE
<div class="file-name">app/views/foos/index.html.erb*, app/views/bars/index.html.erb*</div>
<pre class="large">
&lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"page"</span> <span class="variable-name">data-url</span>=<span class="string">"/foos"</span>&gt;
  &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"content"</span>&gt;
    All the Foos
  &lt;/<span class="function-name">div</span>&gt;
&lt;/<span class="function-name">div</span>&gt;

&lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"page"</span> <span class="variable-name">data-url</span>=<span class="string">"/bars"</span>&gt;
  &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"content"</span>&gt;
    <b>&lt;<span class="function-name">a</span> <span class="variable-name">href</span>=<span class="string">"/bars"</span>&gt;Go to Foos&lt;/<span class="function-name">a</span>&gt;</b>
    All the Bars
  &lt;/<span class="function-name">div</span>&gt;
&lt;/<span class="function-name">div</span>&gt;</pre>

!SLIDE
### back button
android users are back button fiends

!SLIDE
<div class="file-name">app/helpers/application_helper.rb</div>
<pre style="font-size: 2.3em;">
<span class="keyword">def</span> <span class="function-name">differentiate_path</span>(path, *args)
  attempt = request.parameters[<span class="string">"attempt"</span>].to_i + 1
  args.unshift(path).push(<span class="constant">:attempt</span> =&gt; attempt)
  send(*args)
<span class="keyword">end</span>
</pre>

!SLIDE
<div class="file-name">app/helpers/application_helper.rb</div>
<pre style="font-size: 2.3em;">
<span class="keyword">def</span> <span class="function-name">differentiate_path</span>(path, *args)
  <b>attempt = request.parameters[<span class="string">"attempt"</span>].to_i + 1</b>
  args.unshift(path).push(<span class="constant">:attempt</span> =&gt; attempt)
  send(*args)
<span class="keyword">end</span>
</pre>

!SLIDE
<div class="file-name">app/helpers/application_helper.rb</div>
<pre style="font-size: 2.3em;">
<span class="keyword">def</span> <span class="function-name">differentiate_path</span>(path, *args)
  attempt = request.parameters[<span class="string">"attempt"</span>].to_i + 1
  <b>args.unshift(path).push(<span class="constant">:attempt</span> =&gt; attempt)</b>
  send(*args)
<span class="keyword">end</span>
</pre>

!SLIDE
<div class="file-name">app/helpers/application_helper.rb</div>
<pre style="font-size: 2.3em;">
<span class="keyword">def</span> <span class="function-name">differentiate_path</span>(path, *args)
  attempt = request.parameters[<span class="string">"attempt"</span>].to_i + 1
  args.unshift(path).push(<span class="constant">:attempt</span> =&gt; attempt)
  <b>send(*args)</b>
<span class="keyword">end</span>
</pre>

!SLIDE
<div class="file-name">app/views/users/new.html.erb, app/views/users/edit.html.erb</div>
<pre class="medium">
<span class="comment-delimiter"># </span><span class="comment">new form</span>
<span class="constant">:url</span> =&gt; differentiate_path(<span class="constant">:users_path</span>)

<span class="comment-delimiter"># </span><span class="comment">edit form</span>
<span class="constant">:url</span> =&gt; differentiate_path(<span class="constant">:user_path</span>, <span class="variable-name">@user</span>)
</pre>


!SLIDE
<div class="file-name">app/views/layouts/application.html.erb</div>
<pre class="medium">
&lt;<span class="function-name">body</span>&gt;
  &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"page"</span> <b><span class="variable-name">data-dom-cache</span>=<span class="string">"true"</span></b>&gt;
    &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"header"</span>&gt;
      &lt;<span class="function-name">h1</span>&gt;&lt;%= yield :heading %&gt;&lt;/<span class="function-name">h1</span>&gt;
    &lt;/<span class="function-name">div</span>&gt;

    &lt;<span class="function-name">div</span> <span class="variable-name">data-role</span>=<span class="string">"content"</span>&gt;
      &lt;%= yield %&gt;
    &lt;/<span class="function-name">div</span>&gt;
  &lt;/<span class="function-name">div</span>&gt;
&lt;/<span class="function-name">body</span>&gt;</pre>

!SLIDE
## debugging
weinre • Adobe Shadow

!SLIDE
<div class="file-name">app/views/layouts/application.html.erb</div>
<pre style="font-size: 2.3em">
&lt;<span class="function-name">head</span>&gt;
  ...
  &lt;% <span class="keyword">if</span> <span class="type">Rails</span>.env.development? %&gt;
    &lt;%= javascript_include_tag <span class="string">"debug/pagefailed"</span> %&gt;
  &lt;% <span class="keyword">end</span> %&gt;
  ...
&lt;<span class="function-name">/head</span>&gt;
</pre>

!SLIDE
<div class="file-name">app/assets/javascripts/debug/pagefailed.js</div>
<pre style="font-size: 2.3em">
<span class="keyword">function</span> <span class="function-name">onLoadFailed</span>( <span class="js2-function-param">event</span>, <span class="js2-function-param">data</span> ) {
  <span class="keyword">var</span> <span class="variable-name">text</span> = data.xhr.responseText,
      <span class="variable-name">newHtml</span> = text.split( <span class="string">/&lt;\/?html[^&gt;]*&gt;/gmi</span> )[1];

  $( <span class="string">"html"</span> ).html( newHtml );
}

$( document ).on( <span class="string">"pageloadfailed"</span>, onLoadFailed );</pre>

!SLIDE
<div class="file-name">app/assets/javascripts/debug/pagefailed.js</div>
<pre style="font-size: 2.3em">
<span class="keyword">function</span> <span class="function-name">onLoadFailed</span>( <span class="js2-function-param">event</span>, <span class="js2-function-param">data</span> ) {
  <span class="keyword">var</span> <span class="variable-name">text</span> = data.xhr.responseText,
      <span class="variable-name">newHtml</span> = text.split( <span class="string">/&lt;\/?html[^&gt;]*&gt;/gmi</span> )[1];

  $( <span class="string">"html"</span> ).html( newHtml );
}

$( document ).on( <b><span class="string">"pageloadfailed"</span></b>, onLoadFailed );</pre>

!SLIDE
<div class="file-name">app/assets/javascripts/application.js</div>
<pre>
<span class="comment">//= require jquery
//= require jquery_ujs
<b>//= require .</b>
</span></pre>

!SLIDE
<div class="file-name">app/assets/javascripts/application.js</div>
<pre>
<span class="comment">//= require jquery
//= require jquery_ujs
<b>//= require_directory .</b>
</span></pre>

!SLIDE
## Possibilities

!SLIDE
### responsive
WURFL • media queries

!SLIDE
### asset pipeline
AMD support • meta module

!SLIDE bullets mono-bullets
## Links
* jquerymobile.com/resources
* jquerymobile.com/themeroller
* jqmgallery.com

!SLIDE bullets mono-bullets
## Thanks
* @johnbender
* johnbender.us
* github.com/johnbender

!SLIDE bullets mono-bullets blur
<h2 class="blur">Thanks</h2>
* @johnbender
* johnbender.us
* github.com/johnbender

<div class="gigantor" style="font-size: 9.0em; padding">(づ｡◕‿‿◕｡)づ</div>
