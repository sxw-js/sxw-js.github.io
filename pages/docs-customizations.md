---
layout: default
permalink: /docs/customization.html
---

<!-- Hero unit -->
<div class="page__header">
    <div class="hero__overlay hero__overlay--gradient"></div>
    <div class="hero__mask"></div>
    <div class="page__header__inner">
        <div class="container">
            <div class="page__header__content">
                <div class="page__header__content__inner" id='navConverter'>
                    <h1 class="page__header__title">Customizations</h1>
                    <p class="page__header__text">SXW.js offers extensive customizations. Here is a documentation on
                        the available options.</p>
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
                    <li><a href="./usage.html">Basic usage</a></li>
                    <li><a href="#" class="vMenu--active">Customizations</a></li>
                    <li><a href="./demo.html">Demo</a></li>
                </ul>
            </div>
            <div class="page__main">
                <div class="text-container">
                    <h3 class="page__main__title">Sections</h3>
                    <p>The warning displayed in console contains three sections.</p>
                    <ol>
                        <li>A big STOP sign</li>
                        <li>A caution text in bold</li>
                        <li>A detailed message. It can be used to provide more details to users such as where to
                            report an Self-XSS attack, etc...</li>
                    </ol>
                </div>

                <div class="text-container">
                    <h3 class="page__main__title">Configuration</h3>
                    <p>SXW.js has a config object with the following variables,</p>
                    <ul>
                        <li>
                            <b>stopColor</b>: This is the colour of the stop sign. The default value is
                            <code>red</code>.
                        </li>
                        <li>
                            <b>stopFontWeight</b>: The font weight of the stop sign. The default value is
                            <code>bold</code>.
                        </li>
                        <li>
                            <b>cautionFontWeight</b>: The font weight of the caution notice. The default value is
                            <code>bold</code>.
                        </li>
                        <li>
                            <b>cautionFontSize</b>: The font size of the caution notice. The default value is
                            <code>15px</code>.
                        </li>
                    </ul>
                    <p>These variables can be customized to suit your website needs using the <code>setConfig</code>
                        function.</p>
                    <div>
                        Example js object for configuration
                    </div>
                    <code>
<pre>var config = {
  stopColor: "red",
  stopFontWeight: "bold",
  cautionFontWeight: "bold",
  cautionFontSize: "15px",
};</pre>
						</code>
                </div>

                <div class="text-container">
                    <h3 class="page__main__title">Content</h3>
                    <p>SXW.js has a config object with the following variables for each language,</p>
                    <ul>
                        <li>
                            <b>stopText</b>: `*` based stop sign.
                        </li>
                        <li>
                            <b>cautionText</b>: A caution notice with a short one line content.
                        </li>
                        <li>
                            <b>warningText</b>: A detailed message to the customers with instructions to contact
                            your security team and other details.
                        </li>
                    </ul>
                    <p>
                        These variables can be modified using <code>setContent</code> function.
                    </p>
                    <div>
                        Example js object for content
                    </div>
                    <code><pre>var content = {
  en: {
    stopText: "*********  *********  *********  *********\n***           ***     ***   ***  ***   ***\n***           ***     ***   ***  ***   ***\n*********     ***     ***   ***  *********\n      ***     ***     ***   ***  ***\n      ***     ***     ***   ***  ***\n*********     ***     *********  ***",
    cautionText: "Caution: DO NOT PROCEED.",
    warningText: "This section is intended for developers only. Don't copy paste anything in this area.\nIf someone told you to copy and paste something here, it is a scam and will give them access to your account. In that case, kindly report this to our support team."
  }
};</pre>
</code>
                </div>

                <div class="text-container">
                    <h3 class="page__main__title">Functions</h3>
                    <p>There are four functions in the library that will be available into the sxwjs object.</p>
                    <ol>
                        <li>
                            printStop - Prints just the huge stop sign
                            <br>Example: <code>sxwjs.printstop('en');</code>
                        </li>
                        <li>
                            printCautionNotice - Prints the caution sign
                            <br>Example: <code>sxwjs.printCautionNotice('en');</code>
                        </li>
                        <li>
                            printWarningText - Prints the detailed error message
                            <br>Example: <code>sxwjs.printWarningText('en');</code>
                        </li>
                        <li>
                            printWarning - prints all the three sections
                            <br>Example: <code>sxwjs.printWarning('en');</code>
                        </li>
                        <li>
                            setConfig - Assigns the provided configuration.
                            <br>Example: <code>sxwjs.setConfig(config);</code>
                        </li>
                        <li>
                            getConfig - Retrives the configuration.
                            <br>Example: <code>var config = sxwjs.getConfig();</code>
                        </li>
                        <li>
                            setContent - Can be used to modifiy the content such as warningText, cautionNotice,
                            etc...
                            <br>Example: <code>sxwjs.setContent(content);</code>
                        </li>
                        <li>
                            getContent - Retrives the content that will be displayed on the console.
                            <br>Example: <code>var content = sxwjs.getContent();</code>
                        </li>
                    </ol>
                </div>
                <p>Note: None of these functions are called by default. You can choose to call them as you wish.</p>
            </div>
        </div>
    </div>
</div>