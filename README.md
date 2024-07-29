```yaml
---
title: "How To"
author: "PrashantUnity"
weight: 1
date: 2024-06-10T11:57:15+05:30
dateString: June 2024  
description: "Guide of How To Create Blog Post, Categories And Etc"
#canonicalURL: "https://canonical.url/to/page"
cover:
    image: "cover.jpg" # image path/url
    alt: "Download Logo" # alt text
    #caption: "Optical Character Recognition"  display caption under cover 

tags: [ "NET", "codefrydev", "C sharp", "CFD", "Download File","Downloader","httpclient"]
keywords: [ "NET", "codefrydev", "C sharp", "CFD", "Skia Sharp","Generate Video","Basic","FFMPEG"]
draft: true
---
```


## While Creating Folder Or New Category Follow This Structure
```yaml
├──_index.md 
├──categoryOne
│  ├──_index.md
│  ├──post.md
│  ├──post
│     ├──image.png
│     ├──video.mp4
│  ├──anotherpost.md
│  ├──anotherpost
│     ├──image.png
├──categoryTwo
│  ├──_index.md
│  ├──post.md
│  ├──post
│     ├──image.png
│     ├──video.mp4 
```

## Embedding Image in website

- Created post test.md
- Then Create Folder at same Directory with same Name i.e. test
- Place File which are need in that folder.
- directory will look like this

```yaml
├──parent
│  ├──_index.md
│  ├──test.md
│  ├──test
│     ├──cover.jpg
│     ├──video.mp4  
```

Taking Image use case
- One Inside Top Of Head Or For Cover Image 

```yaml
cover:
    image: "folder.png" # image path/url
    alt: "folder Logo" # alt text
```
- Others part of page

```md
![images](./folder.png)
```

For Video Implementation Use Below Snippet.
```html
  <video width="640" height="360" controls>
    <source src="./test.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
```

### _index.md Is Used to represent/ View List Of Post On that Categories /Folder
template
```yaml
---
title: "Name Of Page"
author: "Codefrydev"
weight: 100
date: 2024-06-10T11:57:15+05:30
dateString: June 2024
description: "Description Of Page" 
keywords: [ "NET", "codefrydev", "C sharp", "CFD", "Skia Sharp","Generate Video","Basic","FFMPEG"]
---
```

#### General Post Head Template

```yaml
---
title: "Replace Me With Actual Title"
author: ["Replace Author Name","Another Author Name"]
weight: 100
dateString: June 2024  
description: "Guide of How TO Create Blog Post, Categories AND Etc"
#canonicalURL: "https://canonical.url/to/page"
cover:
    image: "logo.png" # image path/url
    alt: "Download Logo" # alt text
    caption: "Optical Character Recognition"  #display caption under cover 

tags: [ "Code Fry Dev", "codefrydev", "CFD","NET","C Sharp", "Download File","Downloader","httpclient"]
draft: true #make this false to publicly Available
---
```

#### for relate Linking of another page use below code for reference [SKiaSharp]({{< relref "blog/skiasharp/basic.md" >}})

```md
[Basic Setup]({{< relref "blog/skiasharp/basic.md" >}})
```


## Some Of Comman Commands

### Run the Application In development Mode where draft is also visible

```sh
hugo server -D
```

### For Creating New Sites
```sh
hugo new site blog
```

---

### use of Mermaid
```
{{< mermaid >}}
    classDiagram
        class Person{
            +Name
            +Age
            +IsCoding()
        } 
{{< /mermaid >}}

```

### Mermaid with KaTeX

```
{{< mermaid >}}
 graph TB
      A["$$ Sum Of Ratio = \sum_{i=1}^{n} i = \frac{n(n+1)}{2} -1$$"]
      B["$$ ith Number = \frac{i*N}{Sum Of Ratio}$$"]
      C["$$ ith Number = \frac{i*N}{\frac{n(n+1)}{2} -1}$$"]
{{< /mermaid >}}

```mermaid
graph TB
    A["$$ Sum Of Ratio = \sum_{i=1}^{n} i = \frac{n(n+1)}{2} -1$$"]
    B["$$ ith Number = \frac{i*N}{Sum Of Ratio}$$"]
    C["$$ ith Number = \frac{i*N}{\frac{n(n+1)}{2} -1}$$"]
```

Dummy Code For Setup Replace Youtube id with appropriate youtubeid

```yaml 
## Install / Setup step

### Install .NET SDK
- [Visit Here And Install .NET SDK](https://dotnet.microsoft.com/en-us/download)
- It is Straight forward for all platform.
- For Window user Follow below video for more

{{< youtube EqD1H4T340A >}}

- For Mac User Follow below video for more
{{< youtube EqD1H4T340A >}}

- For Linux User Follow below video for more
{{< youtube EqD1H4T340A >}}

### Install Visual Studio IDE
- [Download From Official Website](https://visualstudio.microsoft.com/)

- Available Only for Windows User
- Alternative is [Rider0](https://www.jetbrains.com/rider/) For Cross platform not free as of Now


- For Installiation Process of Visual Studio IDE on window Follow below video

{{< youtube EqD1H4T340A >}}

### Install Visual Studio Code 
- [Visit Here And Install .NET SDK](https://code.visualstudio.com/)
- It is Straight forward for all platform.
- For Window user Follow below video for more

{{< youtube EqD1H4T340A >}}

- For Mac User Follow below video for more

{{< youtube EqD1H4T340A >}}

- For Linux User Follow below video for more

{{< youtube EqD1H4T340A >}}

### Using Polyglot Notebook in VS Code Step-by-Step Guide

#### 1. Install Polyglot Notebook

- **Open VS Code.**
- Press **Control + Shift + X** to open the Extensions view.
- Search for "Polyglot Notebook" or directly open the URL [Polyglot Notebook Extension](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.dotnet-interactive-vscode).
- Look for the extension logo as shown below and install it.

![Polyglot Notebook Extension Logo](./ply0.png)

#### 2. Create a New File

- Create a new file named `HelloWorld.ipynb` as shown in the image below. Double-click to open the file.
- Note: The `.dib` extension also works, but for this guide, we will use `.ipynb` only.

![Create New File](./ply1.png)

#### 3. Select .NET Interactive Kernel

- On the right side, click the "Show Kernel" button.
- Wait for a few seconds. A list of options will appear.
- Select **.NET Interactive** as your kernel.

![Select Kernel](./ply2.png)
```

### Exp for md injection 

```yaml
{{ readFile "content/include.md" | markdownify }}
```
