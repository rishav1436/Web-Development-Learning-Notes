---


---

<h1 id="section-3--introduction-to-css">Section 3 : Introduction to CSS</h1>
<p>CSS is cascading style sheet, allowing us to take control of the design and layout of our websites. We are in version CSS 3. CSS 3 is more mobile compatible.</p>
<p>First, we will introduce some CSS types:</p>
<ul>
<li>Inline CSS:  (All inline CSS code should be in a tag)
<ul>
<li><code>&lt;tag style = "color: red;"&gt;</code> This will change the colour of the tag to red.</li>
<li><code>style = "border: 3px dotted blue"</code> It will make a dotted blue border with size 3px.</li>
<li>Some disadvantage:
<ol>
<li>Too messy if having too many tags</li>
<li>If I want to change many tags at one time, I will have to do many repeated works.</li>
</ol>
</li>
</ul>
</li>
<li>Internal CSS:
<ul>
<li><code>&lt;style&gt;</code>  We can use this tag to start CSS code. We usually put it under the <code>&lt;title&gt;</code> tag.</li>
<li><code>background</code> This will change the background of the tag.</li>
<li>Example:</li>
</ul>
</li>
</ul>
<pre><code>&lt;style&gt;
  h1 {
  color: purple;
  }
</code></pre>
<p>The above code will make <code>h1</code> purple.</p>
<ul>
<li>External CSS: create an external CSS file.
<ul>
<li><code>&lt;link = "stylesheet" href = " CSS filename"&gt;</code>If we want to use external CSS, we need to put this line of code inside our HTML file. It has to be put inside the <code>&lt;head&gt;</code>.</li>
</ul>
</li>
</ul>
<p>Different ways to add CSS to HTML files:</p>
<ul>
<li>Directly target the element: Like the example above, we directly specify <code>h1</code> where we want to add CSS code. This is not recommended.
<ul>
<li><code>background-color: some color</code> Change the background colour. <strong>Note</strong>: we can use hex code to represent colour.</li>
<li><code>text-align</code> How to align your text.</li>
</ul>
</li>
<li><code>&lt;div class = "classname"&gt;</code> This will create a class. It is great when you want to use the same styling in different areas. In CSS file, you should use <code>.classname</code> <strong>Note</strong>: Anything inside the <code>&lt;div&gt;</code> tag will be styling as you specify in the class.</li>
<li><code>&lt;div id = "idname"&gt;</code>Not a good way for styling things. It is usually for interaction with HTML through JavaScript. In CSS file, you should use <code>#idname</code></li>
</ul>
<p>Different ways to assign colour in CSS code:</p>
<ul>
<li>Simply use names of colour, such as <code>purple</code> as above.</li>
<li>Use hex code, such as <code>#ffffff</code> as white</li>
<li><code>rgb(value_for_red, value_for_green, value_for_blue)</code> This allows us to get more specific colour</li>
</ul>
<p>Some specific types of colour:</p>
<ul>
<li><code>linear-gradient(to left, colour one, colour two)</code> This will make a “fading colour”, which will change from colour one to colour two gradually from right to left.</li>
<li><code>text-shadow: h-shadow, v-shadow, blur-radius, colour</code>:
<ul>
<li><code>h-shadow</code>: The position of the horizontal shadow. Negative values are allowed</li>
<li><code>v-shadow</code> The position of the vertical shadow. Negative values are allowed.</li>
<li><code>blur-radius</code>The blur radius. Default value is 0. The larger the value is, the more “fading” the colour is.</li>
</ul>
</li>
<li><code>box-shadow</code> same as <code>text-shadow</code> but the shadow is applied in a box element instead.</li>
</ul>
<p>CSS has a branch of background options. Here we will introduce some basic options:</p>
<ul>
<li><code>background-image</code> Insert an image as background.</li>
<li><code>background-repeat</code> If the background image is too small, the image will repeat itself to fill in the background. For example, you can set <code>background-repeat: no-repeat</code> so the image will not repeat itself but might be very small in the background.</li>
<li><code>background-size</code> You can set the background size. For example, you can set <code>background-size: cover</code> and the image will automatically cover the whole background but the problem is that the resolution of the image will be small if it is a small image.</li>
</ul>
<p>CSS can also set a border to an element:</p>
<ul>
<li><code>border: size_of_border, type_of_border, colour_of_border</code></li>
</ul>
<p>CSS combinations, which is way to design the style of a list. There are two ways to do that:</p>
<ul>
<li><code>ul li {}</code> All list items under unordered list will be changed.</li>
<li><code>ul &gt; li {}</code> Only one level after <code>ul</code> will be changed.</li>
</ul>
<p>CSS grouping, which allows us to add infinite number of elements name, class name or even ID before the <code>{}</code> in a CSS file.</p>
<p>CSS specificity , we can calculate what will be shown on our website by the following photo.<br>
<img src="Specificity.png" alt="Image of Specificity"></p>
<p><strong>Note</strong>: We can also add <code>!important</code> at the end of class inside to make the class most important.</p>

