---
title: "Shortcodes Samples"
date: 2020-06-08T08:06:25+06:00
description: Shortcodes sample
menu:
  sidebar:
    name: Shortcodes Sample
    identifier: shortcodes
    weight: 40
hero: boat.jpg
mermaid: true
---

This is a sample post intended to test the followings:

- Create a Hugo Project
- Default hero image.
- Different shortcodes.

# Build a Hugo Toha project

* https://toha-guides.netlify.app/posts/quickstart/#disable-news-letter-functionality

## Step 1: Fork the example repo and rename
At first, fork this sample repo to your account. Then, rename the repo to whatever you want. If you want to use Github Pages to deploy your site, then rename it to <your username>.github.io. The sample repo comes with pre-configured Github Actions to publish the site in Github Pages and Netlify.

## Step 2: Clone the forked repo locally
Once you have forked and renamed the repository, you can now clone the forked repository in your local machine for further changes.

git clone https://github.com/<>your username<>/<>forked repo name<>

## Step 3: Update the module file
You should see go.mod files in the root of the repository. Update the first line of the go.mod file as below:

module github.com/<>your username<>/<>forked repo name<>

## Step 4: Change config.yaml file
Now, open the repository in an editor and change the following configurations in your config.yaml file located at the root of your repository.

### Change the baseURL
At first change the baseURL to your site URL. If you want to use Github Pages to host your site, then set it as below:

baseURL: https://<>your username<>.github.io

### Change the gitRepo

Now, change the gitRepo field under the params section to point to your forked repository. For example,

gitRepo: https://github.com/<>your username<>/<>your forked repo name<>

## Step 5: Run the site locally

Now, run the following commands to run your site locally:

### a. Load Hugo modules

hugo mod tidy

### b. Install node modules

hugo mod npm pack

npm install

### c. Run the site

hugo server -w

## Step 6: Push the changes to Github

If you have come this far, it means your site is running locally without any issue. Let’s push these changes to Github.

**stage all the changes**

git add .

**commit the changes**

git commit -m "Initial site setup"

git remote add origin https://github.com/Marcos14Almeida/mrcmarc.github.io.git

git push -u origin main

**Public folder**

cd public

git add .

git commit -m "Initial site setup"

git remote add origin https://github.com/Marcos14Almeida/mrcmarc.github.io.git

git branch gh-pages

git checkout gh-pages

git push -u origin gh-pages



--------------------------------------------------------------

## Alert

The following alerts are available in this theme.

{{< alert type="success" >}}
This is sample alert with `type="success"`.
{{< /alert >}}

{{< alert type="danger" >}}
This is sample alert with `type="danger"`.
{{< /alert >}}

{{< alert type="warning" >}}
This is sample alert with `type="warning"`.
{{< /alert >}}

{{< alert type="info" >}}
This is sample alert with `type="info"`.
{{< /alert >}}

{{< alert type="dark" >}}
This is sample alert with `type="dark"`.
{{< /alert >}}

{{< alert type="primary" >}}
This is sample alert with `type="primary"`.
{{< /alert >}}

{{< alert type="secondary" >}}
This is sample alert with `type="secondary"`.
{{< /alert >}}

## Image

#### A sample image without any attribute.

{{< img src="/mrcmarc/posts/shortcodes/boat.jpg" title="A boat at the sea" >}}

{{< vs 3 >}}

#### A sample image with `height` and `width` attributes.

{{< img src="/mrcmarc/posts/shortcodes/boat.jpg" height="400" width="600" title="A boat at the sea" >}}

{{< vs 3 >}}

#### A center aligned image with `height` and `width` attributes.

{{< img src="/mrcmarc/posts/shortcodes/boat.jpg" height="400" width="600" align="center" title="A boat at the sea" >}}

{{< vs 3 >}}


{{- raw -}}
<p>This is raw HTML code</p>
<div class="my-div">Another HTML element</div>
{{- endraw -}}

#### A image with `float` attribute.

{{< img src="/mrcmarc/posts/shortcodes/boat.jpg" height="200" width="500" float="right" title="A boat at the sea" >}}

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras egestas lectus sed leo ultricies ultricies. Praesent tellus risus, eleifend vel efficitur ac, venenatis sit amet sem. Ut ut egestas erat. Fusce ut leo turpis. Morbi consectetur sed lacus vitae vehicula. Cras gravida turpis id eleifend volutpat. Suspendisse nec ipsum eu erat finibus dictum. Morbi volutpat nulla purus, vel maximus ex molestie id. Nullam posuere est urna, at fringilla eros venenatis quis.

Fusce vulputate dolor augue, ut porta sapien fringilla nec. Vivamus commodo erat felis, a sodales lectus finibus nec. In a pulvinar orci. Maecenas suscipit eget lorem non pretium. Nulla aliquam a augue nec blandit. Curabitur ac urna iaculis, ornare ligula nec, placerat nulla. Maecenas aliquam nisi vitae tempus vulputate.

## Split

This theme support splitting the page into as many columns as you wish.

#### Two column split

{{< split 6 6>}}

##### Left Column

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras egestas lectus sed leo ultricies ultricies.

---

##### Right Column

Fusce ut leo turpis. Morbi consectetur sed lacus vitae vehicula. Cras gravida turpis id eleifend volutpat.

{{< /split >}}

#### Three column split

{{< split 4 4 4 >}}

##### Left Column

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras egestas lectus sed leo ultricies ultricies.

---

##### Middle Column

Aenean dignissim dictum ex. Donec a nunc vel nibh placerat interdum. 

---

##### Right Column

Fusce ut leo turpis. Morbi consectetur sed lacus vitae vehicula. Cras gravida turpis id eleifend volutpat.

{{< /split >}}

## Vertical Space

Give vertical space between two lines.

This is line one.
{{< vs 4>}}
This is line two. It should have `4rem` vertical space with previous line.

## Video

{{< video src="/videos/sample.mp4" >}}

<!-- markdown-link-check-disable-next-line -->
Video by [Rahul Sharma](https://www.pexels.com/@rahul-sharma-493988) from [Pexels](https://www.pexels.com).

## Mermaid

Here, are few example of mermaid shortcode.

**Graph:**

{{< mermaid align="left" >}}
graph LR;
    A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
{{< /mermaid >}}

**Sequence Diagram:**

{{< mermaid >}}
sequenceDiagram
    participant Alice
    participant Bob
    Alice->>John: Hello John, how are you?
    loop Healthcheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail!
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
{{< /mermaid >}}

**Gantt diagram:**

{{< mermaid >}}
gantt
  dateFormat  YYYY-MM-DD
  title Adding GANTT diagram to mermaid
  excludes weekdays 2014-01-10

section A section
  Completed task            :done,    des1, 2014-01-06,2014-01-08
  Active task               :active,  des2, 2014-01-09, 3d
  Future task               :         des3, after des2, 5d
  Future task2               :         des4, after des3, 5d
{{< /mermaid >}}

**Class Diagram:**

{{< mermaid >}}
classDiagram
  Class01 <|-- AveryLongClass : Cool
  Class03 *-- Class04
  Class05 o-- Class06
  Class07 .. Class08
  Class09 --> C2 : Where am i?
  Class09 --* C3
  Class09 --|> Class07
  Class07 : equals()
  Class07 : Object[] elementData
  Class01 : size()
  Class01 : int chimp
  Class01 : int gorilla
  Class08 <--> C2: Cool label
{{< /mermaid >}}

**Git Graph:**

{{< mermaid background="black" align="right" >}}
gitGraph:
options
{
    "nodeSpacing": 150,
    "nodeRadius": 10
}
end
commit
branch newbranch
checkout newbranch
commit
commit
checkout master
commit
commit
merge newbranch
{{< /mermaid >}}

**ER Diagram:**

{{< mermaid >}}
erDiagram
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ LINE-ITEM : contains
    CUSTOMER }|..|{ DELIVERY-ADDRESS : uses
{{< /mermaid >}}

## Gist

{{< gist hossainemruz 4ad86c9b6378677e14eff12713e75e44 >}}
