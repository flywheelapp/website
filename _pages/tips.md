---
layout: doc
title: "Flywheel Tips"
permalink: /tips
---

- TOC
{:toc}

Create a new document
---------------------
There are several ways to create a new document:
1. Click the plus button in the toolbar.
2. Right click on a folder in the sidebar and choose New Document.
3. Use the File -> New menu to create a new document.
4. Just <kbd>Command</kbd> + <kbd>N</kbd>.

<img src="/assets/new-doc.png" alt="New Document" style="max-width: 650px; width: 100%;">

How to use the Gallery Extension
--------------------------------
We support third party shape libraries to extend shape templates. Currenty the extension for supporting <a href="https://libraries.excalidraw.com/" target="_blank">Excalidraw Libraries</a> is already bundled with the application. Use the following instructions to install the libraries. Once a library is installed, you can drag its components into your document.

<img src="/assets/help-gallery-ext.png" alt="Gallery Extension Usage" style="max-width: 650px; width: 100%;">

Contact
-------
For any issues, questions or suggestions, please do not hesitate to contact us.

{% if site.data.social-media %}
<div id="social-media">
    <ul>
    {% assign sm = site.data.social-media %}
    {% for entry in sm %}
        {% assign key = entry | first %}
        {% if sm[key].id %}
        <li>
            <i class="fa {{ sm[key].fa-icon }}"></i> <a href="{{ sm[key].href }}{{ sm[key].id }}" title="{{ sm[key].title }}">{{ sm[key].id }}</a>
        </li>
        {% endif %}
    {% endfor %}
    </ul>
</div>
{% endif %}
