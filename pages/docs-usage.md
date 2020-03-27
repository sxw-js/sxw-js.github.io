---
layout: default
permalink: /docs/usage.html
---

<!-- Hero unit -->
<div class="page__header">
    <div class="hero__overlay hero__overlay--gradient"></div>
    <div class="hero__mask"></div>
    <div class="page__header__inner">
        <div class="container">
            <div class="page__header__content">
                <div class="page__header__content__inner" id='navConverter'>
                    <h1 class="page__header__title">Basic usage</h1>
                    <p class="page__header__text">Instruction on how to print simple warnings using SXW.js in
                        various environments.</p>
                </div>
            </div>
        </div>
    </div>
</div>
<!-- Page content -->
<div class="page">
    <div class="container">
        <div class="page__inner">
            <div class="page__menu">
                <ul class="vMenu">
                    <li><a href="./installation.html">Installation</a></li>
                    <li><a href="#" class="vMenu--active">Basic usage</a></li>
                    <li><a href="./customization.html">Customizations</a></li>
                    <li><a href="./demo.html">Demo</a></li>
                </ul>
            </div>
            <div class="page__main">
                <div class="text-container">
                    <h3 class="page__main__title">Using in Javascript</h3>
                    <ul>
                        <li>Include the javascript file in your website coe.</li>
                        <li>
                            All the predefined functions are defined in <code>window.sxwjs</code> object.
                        </li>
                        <li>
                            Call the corresponding funtion fron window.sxwjs object.<br>
                            <code>
                                &lt;script&gt;<br>
                                &nbsp;&nbsp;window.sxwjs.printWarning('en');<br>
                                &lt;/script&gt;
                            </code>
                        </li>
                    </ul>
                </div>
                <div class="text-container">
                    <h3 class="page__main__title">Using in Angular</h3>
                    <ul>
                        <li>Install the package through npm</li>
                        <li>
                            Import the module in your application.<br>
                            <code>import sxwjs from '@sxwjs/sxwjs';</code>
                        </li>
                        <li>
                            Call the corresponding funtion fron sxwjs object.<br>
                            <code>sxwjs.printWarning('en');</code>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</div>