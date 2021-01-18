+++
title = "Aris Consultancy"
+++
<!--: .wrap .size-70 ..aligncenter bgimage=images/pencil.jpg -->


## **Aris Consultancy Services**

<!--: .text-intro -->Helping Future Leaders find their Dream Instituitions.

---

<!--: .wrap -->

## **Various Streams of Colleges we Consult :-**

<!--: .flexblock gallery -->
- {{< gallery title="Technical" href="#slide=10" src="images/Technical Education.jpg" >}}Technical{{< /gallery >}}
- {{< gallery title="Management" href="https://webslides.tv/demos/landings" src="images/Management Studies.png" >}}Management{{< /gallery >}}
- {{< gallery title="Medical" href="https://webslides.tv/demos/portfolios" src="images/bill-oxford-8u_2imJaVQs-unsplash.jpg" >}}Medical{{< /gallery >}}
- {{< gallery title="Distant Degree" href="https://webslides.tv/demos/apple" src="https://webslides.tv/static/images/demos-apple.png" >}}Distant Degree{{< /gallery >}}

---
<!--: .wrap -->

## **More Examples**
<small>Note. None of these slides are currently not ported to Hugo-Webslides...YET.</small>

<!--: .flexblock gallery -->
- {{< gallery title="Netflix's Culture" href="https://arisonline.co.in/#slide=5" src="images/pencil.jpg" >}}Netflix{{< /gallery >}}
- {{< gallery title="Longform Articles" href="https://webslides.tv/demos/longforms" src="images/bill-oxford-8u_2imJaVQs-unsplash.jpg" >}}Longforms{{< /gallery >}}
- {{< gallery title="Interviews" href="https://webslides.tv/demos/interviews" src="https://webslides.tv/static/images/demos-interviews.png" >}}Interviews{{< /gallery >}}

---
<!-- : .wrap .size-40 -->

### **Configuration**

<!-- : .text-intro -->You can modify WebSlides settings directly from your project config.toml.

~~~toml
[params.webslides]
  banner = false
  slideshow = true
  vertical = false
  autoslide = false
  changeOnClick = false
  disableLoop = false
  minWheelDelta = 40
  disableNavigateOnScroll = false
  scrollWait = 450
  slideOffset = 50
  hideIndex = false
~~~


---
<!-- : .wrap -->

|||v

### **All from one markdown file**

Use three dashes "<code>-</code>" to create a separate slide page.

|||

~~~md

Slide1

---

Slide2

~~~

---
<!-- : .wrap -->


|||

~~~
content
├── home
│   ├── home1.md (weight: 1)
│   └── home2.md (weight: 2)
└── _index.md (initial page)
~~~

|||

### Or not.

You can combine and arrange files with the weight parameter in front matter, and categorize .md files into different folders.

---
<!-- : .aligncenter -->

## Simple Class Assignment

Assign class to a block by using the following notation without quote.

<code><span><!-</span>- : .class -<span>-></span>Content</code>

---
<!-- : .wrap -->

### You can assign class to many elements

<!-- : .flexblock -->
- {{< flexblock "Slides" 6 >}}
<span><!-</span>- : sectionClass .divClass ..subClass -<span>-></span><br>
Content
~~~html
<section class="sectionClass">
  <div class="divClass">
    <div class="subClass">
    Content
    </div>
  </div>
</section>
~~~
{{< /flexblock >}}

- {{< flexblock "Headers and Paragraphs" 6 >}}
<span># <!-</span>- : .hClass -<span>-></span>Header<br>
<span><!-</span>- : .pClass -<span>-></span>Paragraph
~~~html
<h1 class="hClass">Header</h1>
<p class="pClass">Paragraph</p>
~~~
{{< /flexblock >}}

- {{< flexblock "Lists" 6 >}}
<span><!-</span>- : .listClass -<span>-></span><br>
<span>-</span> list1<br>
<span>-</span> list2
~~~
<ul class="listClass">
  <li>list1</li>
  <li>list2</li>
</ul>
~~~
{{< /flexblock >}}
