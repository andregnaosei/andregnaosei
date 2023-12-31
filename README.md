png" href="favicon.png">

    <meta charset="utf-8">

    <meta name="description" content="Battle for control of different nations with your Clan and become an economic or military superpower. Proudly made by Faraway">
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, minimum-scale=1, user-scalable=no">
    <meta name="keywords" content="battle royale, multiplayer, io, 3D Battle Royale, browser game, br, survival, game, web game">
    <meta name="mobile-web-app-capable" content="yes">
    <meta name="google-site-verification" content="cigM80uSj2Vg_S3O9poee_cR5HkV7zxGtsV14cRqVqY">

    <meta property="og:image" content="https://miniroyale.io/thumbnail.jpg?v=1.1.213">
    <meta property="og:description" content="Battle for control of different nations with your Clan and become an economic or military superpower. Proudly made by Faraway">
    <meta property="og:type" content="website">
    <meta property="og:title" content="Mini Royale: Nations">
    <meta property="og:url" content="https://miniroyale.io/">
    <meta property="og:site_name" content="miniroyale.io">

    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&amp;display=swap" rel="stylesheet">

    <link rel="canonical" href="https://miniroyale.io">
    <style>
        @font-face {
            font-family: 'Forza-Medium';
            src: url('./fonts/Forza-Medium.ttf') format('truetype');
            font-weight: normal;
            font-style: normal;
        }

        @font-face {
            font-family: 'Forza-BoldItalic';
            src: url('./fonts/Forza-BoldItalic.ttf') format('truetype');
            font-weight: normal;
            font-style: normal;
        }

        @font-face {
            font-family: 'Forza-Bold';
            src: url('./fonts/Forza-Bold.ttf') format('truetype');
            font-weight: normal;
            font-style: normal;
        }

        body {
            background: #000;
            margin: 0;
            padding: 0;
            overflow: hidden;
            font-family: 'Bebas Neue', cursive;
        }

        #links {
            display: none;
        }

        #about {
            display: none;
        }

        #content-wrapper {
            display: none;
            position: absolute;
        }

        #application-splash-wrapper {
            background: #283538 url('./overlay.jpg?v=1.1.213') no-repeat center center;
            background-size: cover !important;
            font-family: 'Roboto', sans-serif;
            position: absolute;
            top: 0;
            left: 0;
            height: 100%;
            width: 100%;
        }

        #application-splash {
            position: absolute;
            top: calc(50% - 150px);
            width: 300px;
            left: calc(50% - 150px);
        }

        #application-splash img {
            width: 100%;
        }

        @media (max-width: 480px) {
            #application-splash {
                width: 170px;
                left: calc(50% - 85px);
            }
        }

        #progress-bar-bg {
            position: absolute;
            left: 5%;
            bottom: 2vw;
            height: 0.9vw;
            width: 90%;
            margin: auto;
            background-color: #252525;
            opacity: 1;
        }

        #progress-bar {
            position: absolute;
            left: 5.1%;
            bottom: 2.15vw;
            height: 0.6vw;
            width: 0;
            margin: auto;
            background-color: #FFCA0E;
        }

        #version-code {
            font-family: 'Forza-Bold', sans-serif;
            text-align: center;
            color: #dadada;
            display: block;
            font-size: 0.85vw;
            position: fixed;
            right: 5.3%;
            bottom: 0.4vw;
        }

        #loading-assets-text {
            font-family: 'Forza-Bold', sans-serif;
            text-align: center;
            color: #fff;
            bottom: 3.7vw;
            font-size: 1.1vw;
            position: absolute;
            left: calc(50% - 3vw);
        }

        #application-canvas {
            width: 100%;
            height: 100%;
            position: absolute;
            outline: none !important;
        }

        @media only screen and (orientation: portrait) {
            #application-splash-wrapper.banner {
                background-size: cover;
            }

            #version-code.banner {
                right: 37%;
                bottom: 5vw;
            }

            button.banner {
                bottom: 10vw;
            }
        }

        @media only screen and (orientation: landscape) {
            #application-splash-wrapper.banner {
                background-size: cover;
            }

            #version-code.banner {
                right: 5%;
                bottom: 2vw;
            }

            button.banner {
                bottom: 5vw;
            }
        }
    @media screen and (min-aspect-ratio: 1920/1080) {    #application-canvas.fill-mode-KEEP_ASPECT {        width: auto;        height: 100%;        margin: 0 auto;    }}</style>

    <script src="https://checkout.faraway.com/faraway-wallets-provider.browser.js?v=1.1.213"></script>
    <script src="https://checkout.faraway.com/faraway-checkout.umd.js?v=1.1.213"></script>
    <script src="https://connect.faraway.com/faraway-connect.umd.js?v=1.1.213"></script>

    <script src="https://sdk.crazygames.com/crazygames-sdk-v2.js"></script>
    <script src="js/playcanvas-stable.min.js?v=1.1.213"></script>
    <script src="js/__settings__.js?v=1.1.213"></script>
    <script src="js/__override__.js?v=1.1.213"></script>
    <script>
        VERSION = "1.1.213";
        BRANCH = "main";
        ENVIRONMENT = "prod";
        DOMAIN = "miniroyale.io";
        ASSET_PREFIX = "";
        SCRIPT_PREFIX = "";
        SCENE_PATH = "1175392.json?v=1.1.213";
        CONTEXT_OPTIONS = {
            'antialias': false,
            'alpha': false,
            'preserveDrawingBuffer': false,
            'preferWebGl2': true
        };
        CONFIG_FILENAME = "config.json?v=1.1.213";
        MAP_PREFIX = "https://maps.miniroyale.io/";
        GS_TAG = "main";
        SENTRY_DSN = "https://b372ac0926094f9bb9ffa5329453a986@o967800.ingest.sentry.io/6752571";
    </script>

    <!-- Google tag (gtag.js) -->
    <script async="" src="https://www.googletagmanager.com/gtag/js?id=G-44EV46Q15W"></script>
    <script>
        window.dataLayer = window.dataLayer || [];
        function gtag(){dataLayer.push(arguments);}
        gtag('js', new Date());

        gtag('config', 'G-44EV46Q15W');
    </script>
<style type="text/css"></style><script async="" src="//static.site24x7rum.eu/beacon/site24x7rum-min.js?appKey=6bbde4312bb4aa27610f2556162573ef"></script><script src="__game-scripts.js?v=1.1.213"></script><style>
    input::-webkit-outer-spin-button,
    input::-webkit-inner-spin-button {
        -webkit-appearance: none;
        margin: 0;
    }

    input[type=number] {
        -moz-appearance: textfield;
    }</style><style>
    input::-webkit-outer-spin-button,
    input::-webkit-inner-spin-button {
        -webkit-appearance: none;
        margin: 0;
    }

    input[type=number] {
        -moz-appearance: textfield;
    }</style><style>
    input::-webkit-outer-spin-button,
    input::-webkit-inner-spin-button {
        -webkit-appearance: none;
        margin: 0;
    }

    input[type=number] {
        -moz-appearance: textfield;
    }</style><style>
    input::-webkit-outer-spin-button,
    input::-webkit-inner-spin-button {
        -webkit-appearance: none;
        margin: 0;
    }

    input[type=number] {
        -moz-appearance: textfield;
    }</style><style>
    input::-webkit-outer-spin-button,
    input::-webkit-inner-spin-button {
        -webkit-appearance: none;
        margin: 0;
    }

    input[type=number] {
        -moz-appearance: textfield;
    }</style><style>
    input::-webkit-outer-spin-button,
    input::-webkit-inner-spin-button {
        -webkit-appearance: none;
        margin: 0;
    }

    input[type=number] {
        -moz-appearance: textfield;<body style="cursor: default;">
    <script type="text/javascript" src="js/__modules__.js"></script>
    <script type="text/javascript" src="js/__start__.js?v=1.1.213"></script><canvas id="application-canvas" tabindex="0" style="user-select: none; width: 1365px; height: 971px;" width="1365" height="971" class="fill-mode-FILL_WINDOW"></canvas><script src="files/assets/140310720/1/ammo.wasm.js"></script>
    <script type="text/javascript" src="js/__loading__.js?v=1.1.213"></script>

    <script type="text/javascript">
        (function(w,d,s,r,k,h,m){
            if(w.performance && w.performance.timing && w.performance.navigation) {
                w[r] = w[r] || function(){(w[r].q = w[r].q || []).push(arguments)};
                h=d.createElement('script');h.async=true;h.setAttribute('src',s+k);
                d.getElementsByTagName('head')[0].appendChild(h);
                (m = window.onerror),(window.onerror = function (b, c, d, f, g) {
                    m && m(b, c, d, f, g),g || (g = new Error(b)),(w[r].q = w[r].q || []).push(["captureException",g]);})
            }
        })(window,document,'//static.site24x7rum.eu/beacon/site24x7rum-min.js?appKey=','s247r','6bbde4312bb4aa27610f2556162573ef');
    </script>


<canvas id="AudiusCanvas" style="width: 377px; height: 570px; right<script type="text/javascript" src="js/__modules__.js"></script>/* The rest of this file contains styles related to the mechanics of
   the editor. You probably shouldn't touch them. */

.CodeMirror {
  position: relative;
  overflow: hidden;
  background: var(--color-background);
}

.CodeMirror-scroll {
  overflow: scroll !important; /* Things will break if this is overridden */
  /* 50px is the magic margin used to hide the element's real scrollbars */
  /* See overflow: hidden in .CodeMirror */
  margin-bottom: -50px;
  margin-right: -50px;
  padding-bottom: 50px;
  height: 100%;
  outline: none; /* Prevent dragging from highlighting the element */
  position: relative;
}

.CodeMirror-sizer {
  position: relative;
  border-right: 50px solid transparent;
}

/* The fake, visible scrollbars. Used to force redraw during scrolling
   before actual scrolling happens, thus preventing shaking and
   flickering artifacts. */
.CodeMirror-vscrollbar,
.CodeMirror-hscrollbar,
.CodeMirror-scrollbar-filler,
.CodeMirror-gutter-filler {
  position: absolute;
  z-index: 6;
  display: none;
  outline: none;
}

.CodeMirror-vscrollbar {
  right: 0;
  top: 0;
  overflow-x: hidden;
  overflow-y: scroll;
}

.CodeMirror-hscrollbar {
  bottom: 0;
  left: 0;
  overflow-y: hidden;
  overflow-x: scroll;
}

.CodeMirror-scrollbar-filler {
  right: 0;
  bottom: 0;
}

.CodeMirror-gutter-filler {
  left: 0;
  bottom: 0;
}

.CodeMirror-gutters {
  position: absolute;
  left: 0;
  top: 0;
  min-height: 100%;
  z-index: 3;
}

.CodeMirror-gutter {
  white-space: normal;
  height: 100%;
  display: inline-block;
  vertical-align: top;
  margin-bottom: -50px;
}

.CodeMirror-gutter-wrapper {
  position: absolute;
  z-index: 4;
  background: none !important;
  border: none !important;
}

.CodeMirror-gutter-background {
  position: absolute;
  top: 0;
  bottom: 0;
  z-index: 4;
}

.CodeMirror-gutter-elt {
  position: absolute;
  cursor: default;
  z-index: 4;
}

.CodeMirror-gutter-wrapper ::selection {
  background-color: transparent;
}

.CodeMirror-gutter-wrapper ::-moz-selection {
  background-color: transparent;
}

.CodeMirror-lines {
  cursor: text;
  min-height: 1px; /* prevents collapsing before first draw */
}

.CodeMirror pre.CodeMirror-line,
.CodeMirror pre.CodeMirror-line-like {
  /* Reset some styles that the rest of the page might have set */
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -moz-border-radius: 0;
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -webkit-border-radius: 0;
  border-radius: 0;
  border-width: 0;
  background: transparent;
  font-family: inherit;
  font-size: inherit;
  margin: 0;
  white-space: pre;
  word-wrap: normal;
  line-height: inherit;
  color: inherit;
  z-index: 2;
  position: relative;
  overflow: visible;
  -webkit-tap-highlight-color: transparent;
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -webkit-font-variant-ligatures: contextual;
  font-variant-ligatures: contextual;
}

.CodeMirror-wrap pre.CodeMirror-line,
.CodeMirror-wrap pre.CodeMirror-line-like {
  word-wrap: break-word;
  white-space: pre-wrap;
  word-break: normal;
}

.CodeMirror-linebackground {
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  z-index: 0;
}

.CodeMirror-linewidget {
  position: relative;
  z-index: 2;
  padding: 0.1px; /* Force widget margins to stay inside of the container */
}

.CodeMirror-rtl pre {
  direction: rtl;
}

.CodeMirror-code {
  outline: none;
}

/* Force content-box sizing for the elements where we expect it */
.CodeMirror-scroll,
.CodeMirror-sizer,
.CodeMirror-gutter,
.CodeMirror-gutters,
.CodeMirror-linenumber {
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -moz-box-sizing: content-box;
  box-sizing: content-box;
}

.CodeMirror-measure {
  position: absolute;
  width: 100%;
  height: 0;
  overflow: hidden;
  visibility: hidden;
}

.CodeMirror-cursor {
  position: absolute;
  pointer-events: none;
}

.CodeMirror-measure pre {
  position: static;
}

div.CodeMirror-cursors {
  visibility: hidden;
  position: relative;
  z-index: 3;
}

div.CodeMirror-dragcursors {
  visibility: visible;
}

.CodeMirror-focused div.CodeMirror-cursors {
  visibility: visible;
}

.CodeMirror-selected {
  --override-cm-selected-background-color: #d9d9d9;

  background: var(--override-cm-selected-background-color);
}

.-theme-with-dark-background .CodeMirror-selected,
:host-context(.-theme-with-dark-background) .CodeMirror-selected {
  --override-cm-selected-background-color: rgb(38 38 38);
}

.CodeMirror-focused .CodeMirror-selected {
  --override-cm-selected-background-color: #d7d4f0;
}

.-theme-with-dark-background .CodeMirror-focused .CodeMirror-selected,
:host-context(.-theme-with-dark-background) .CodeMirror-focused .CodeMirror-selected {
  --override-cm-selected-background-color: rgb(18 15 43);
}

.CodeMirror-crosshair {
  cursor: crosshair;
}

.CodeMirror-line {
  --override-line-selection-background-color: #d7d4f0;
}

.CodeMirror-line::selection,
.CodeMirror-line > span::selection,
.CodeMirror-line > span > span::selection {
  background:var(--override-line-selection-background-color);
}

.CodeMirror-line::-moz-selection,
.CodeMirror-line > span::-moz-selection,
.CodeMirror-line > span > span::-moz-selection {
  background: var(--override-line-selection-background-color);
}

.-theme-with-dark-background .CodeMirror-line,
:host-context(.-theme-with-dark-background) .CodeMirror-line {
  --override-line-selection-background-color: rgb(18 15 43);

}

.cm-searching {
  --override-searching-background-color: rgb(255 255 0 / 40%);

  background-color: var(--override-searching-background-color);
}

/* Used to force a border model for a node */
.cm-force-border {
  padding-right: 0.1px;
}

@media print {
  /* Hide the cursor when printing */
  .CodeMirror div.CodeMirror-cursors {
    visibility: hidden;
  }
}

/* See issue #2901 */
.cm-tab-wrap-hack::after {
  content: "";
}

/* Help users use markselection to safely style text background */
span.CodeMirror-selectedtext {
  background: none;
}

/*# sourceURL=third_party/codemirror/codemirror.css *//*
 * Copyright 2021 The Chromium Authors. All rights reserved.
 * Use of this source code is governed by a BSD-style license that can be
 * found in the LICENSE file.
 */

/* stylelint-disable no-descending-specificity */

/**
 * Many of the CSS variables here were auto generated during the dark mode
 * migration. If you are changing them, please feel free to rename them whilst
 * you're here to make them clearer.
 */

.CodeMirror {
  --override-search-highlight-border-color: rgb(128 128 128);

  line-height: 1.2em !important; /* stylelint-disable-line declaration-no-important */
  background-color: transparent !important; /* stylelint-disable-line declaration-no-important */
  color: var(--color-text-primary);
  height: 300px;
}

.CodeMirror-linewidget {
  overflow: visible !important; /* stylelint-disable-line declaration-no-important */
}

.CodeMirror-gutter-performance {
  width: 60px;
  background-color: var(--color-background);
  margin-left: 3px;
}

.CodeMirror-gutter-memory {
  width: 48px;
  background-color: var(--color-background);
  margin-left: 3px;
}

.CodeMirror-gutter-coverage {
  width: 5px;
  background-color: var(--color-background);
  margin-left: 3px;
}

.CodeMirror .source-frame-eval-expression {
  --override-auto-gen-codemirrorsourceframeevalexpression-backgroundcolor: rgb(255 255 194);
  --override-auto-gen-codemirrorsourceframeevalexpression-border: rgb(163 41 34);

  outline: 0;
  border: 1px solid var(--override-auto-gen-codemirrorsourceframeevalexpression-border);
  border-left-width: 0;
  border-right-width: 0;
  background-color: var(--override-auto-gen-codemirrorsourceframeevalexpression-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .source-frame-eval-expression,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-eval-expression {
  --override-auto-gen-codemirrorsourceframeevalexpression-border: rgb(221 99 92);
  --override-auto-gen-codemirrorsourceframeevalexpression-backgroundcolor: rgb(61 61 0);
}

.CodeMirror .source-frame-eval-expression-start {
  border-left-width: 1px;
  margin-left: -1px;
}

.CodeMirror .source-frame-eval-expression-end {
  border-right-width: 1px;
  margin-right: -1px;
}

.CodeMirror .source-frame-continue-to-location {
  --override-auto-gen-codemirrorsourceframecontinuetolocation-backgroundcolor: rgb(230 236 255);

  outline: 0;
  border: 1px solid transparent;
  border-left-width: 0;
  border-right-width: 0;
  background-color: var(--override-auto-gen-codemirrorsourceframecontinuetolocation-backgroundcolor);
  cursor: pointer;
}

.CodeMirror .source-frame-continue-to-location:hover {
  --override-auto-gen-codemirrorsourceframecontinuetolocationhover-backgroundcolor: rgb(171 191 254);
  --override-auto-gen-codemirrorsourceframecontinuetolocationhover-border: rgb(121 141 254);

  border: 1px solid var(--override-auto-gen-codemirrorsourceframecontinuetolocationhover-border);
  background-color: var(--override-auto-gen-codemirrorsourceframecontinuetolocationhover-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .source-frame-continue-to-location,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-continue-to-location {
  background-color: #14522b;
}

.-theme-with-dark-background .CodeMirror .source-frame-continue-to-location:hover,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-continue-to-location:hover {
  border: 1px solid #33cc6b;
  background-color: #14522b;
}

.CodeMirror .source-frame-continue-to-location-start {
  border-left-width: 1px;
  margin-left: -1px;
}

.CodeMirror .source-frame-continue-to-location-end {
  border-right-width: 1px;
  margin-right: -1px;
}

.CodeMirror .source-frame-async-step-in {
  --override-auto-gen-codemirrorsourceframeasyncstepin-backgroundcolor: hsl(100deg 46% 80% / 100%);

  outline: 0;
  background-color: var(--override-auto-gen-codemirrorsourceframeasyncstepin-backgroundcolor);
  cursor: pointer;
  border: 1px solid transparent;
  border-left-width: 0;
  border-right-width: 0;
}

.-theme-with-dark-background .CodeMirror .source-frame-async-step-in,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-async-step-in {
  --override-auto-gen-codemirrorsourceframeasyncstepin-backgroundcolor: rgb(43 74 28);
}

.source-frame-async-step-in-hovered .source-frame-async-step-in {
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-bordercolor: rgb(100 154 100);
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-backgroundcolor: hsl(96deg 53% 65%);

  background-color: var(--override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-backgroundcolor);
  border-color: var(--override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-bordercolor);
}

.-theme-with-dark-background .source-frame-async-step-in-hovered .source-frame-async-step-in,
:host-context(.-theme-with-dark-background) .source-frame-async-step-in-hovered .source-frame-async-step-in {
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-backgroundcolor: rgb(80 137 42);
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-bordercolor: rgb(101 155 101);
}

.source-frame-async-step-in-hovered .source-frame-async-step-in-start {
  border-left-width: 1px;
  margin-left: -1px;
}

.source-frame-async-step-in-hovered .source-frame-async-step-in-end {
  border-right-width: 1px;
  margin-right: -1px;
}

.CodeMirror-cursor {
  border-left: 1px solid var(--color-background-inverted);
  border-right: none;
  width: 0;
}

.CodeMirror-readonly .CodeMirror-cursor {
  display: none;
}

.CodeMirror-gutters {
  border-right: 1px solid var(--color-details-hairline);
  white-space: nowrap;
  background-color: var(--color-background);
}

.CodeMirror-linenumber {
  --override-auto-gen-codemirrorlinenumber-color: hsl(0deg 0% 46%);

  color: var(--override-auto-gen-codemirrorlinenumber-color);
  padding: 0 3px 0 9px;
  min-width: 28px;
  text-align: right;
  white-space: nowrap;
}

.-theme-with-dark-background .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .CodeMirror-linenumber {
  --override-auto-gen-codemirrorlinenumber-color: rgb(138 138 138);
}

.pretty-printed .CodeMirror-linenumber {
  color: var(--legacy-accent-color);
}

.cm-non-breakable-line .CodeMirror-linenumber {
  --override-auto-gen-cmnonbreakablelinecodemirrorlinenumber-color: rgb(128 128 128 / 40%);

  color: var(--override-auto-gen-cmnonbreakablelinecodemirrorlinenumber-color);
}

.-theme-with-dark-background .cm-non-breakable-line .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-non-breakable-line .CodeMirror-linenumber {
  --override-auto-gen-cmnonbreakablelinecodemirrorlinenumber-color: rgb(127 127 127 / 40%);
}

.cm-highlight {
  animation: fadeout 2s 0s;
}

.-theme-with-dark-background .cm-highlight,
:host-context(.-theme-with-dark-background) .cm-highlight {
  animation: fadeout-dark 2s 0s;
}

@keyframes fadeout {
  from {
    background-color: rgb(255 255 120); /* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: var(--color-background); }
}

@keyframes fadeout {
  from {
    background-color: rgb(255 255 120); /* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: var(--color-background); }
}

@keyframes fadeout-dark {
  from {
    background-color: hsl(133deg 100% 30% / 50%);/* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: transparent; }
}

@keyframes fadeout-dark {
  from {
    background-color: hsl(133deg 100% 30% / 50%);/* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: transparent; }
}

.cm-readonly-highlight {
  --override-auto-gen-cmreadonlyhighlight-backgroundcolor: rgb(255 255 120);

  background-color: var(--override-auto-gen-cmreadonlyhighlight-backgroundcolor);
}

.-theme-with-dark-background .cm-readonly-highlight,
:host-context(.-theme-with-dark-background) .cm-readonly-highlight {
  background-color: hsl(133deg 100% 30% / 50%);
}

.cm-highlight.cm-execution-line {
  animation: fadeout-execution-line 1s 0s;
}

.-theme-with-dark-background .cm-highlight.cm-execution-line,
:host-context(.-theme-with-dark-background) .cm-highlight.cm-execution-line {
  animation: fadeout-execution-line-dark 1s 0s;
}

@keyframes fadeout-execution-line {
  from {
    background-color: rgb(121 141 254);/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: rgb(171 191 254);/* stylelint-disable-line plugin/use_theme_colors */
  }
}

@keyframes fadeout-execution-line {
  from {
    background-color: rgb(121 141 254);/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: rgb(171 191 254);/* stylelint-disable-line plugin/use_theme_colors */
  }
}

@keyframes fadeout-execution-line-dark {
  from {
    background-color: #208043;/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: #14522b;/* stylelint-disable-line plugin/use_theme_colors */
  }
}

@keyframes fadeout-execution-line-dark {
  from {
    background-color: #208043;/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: #14522b;/* stylelint-disable-line plugin/use_theme_colors */
  }
}

.CodeMirror-linenumber:hover,
.cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-preserve {
  border-width: 1px 4px 1px 1px;
  padding-right: 3px;
  padding-left: 8px;
  height: 11px;
  line-height: 12px;
  border-style: solid;
  position: relative;
  /* The line number jumps slightly on hover when the minify banner is showing
     if this fractional value is not there. */
  top: -0.15px;
}

.CodeMirror-linenumber:hover {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23ebeced" stroke="%23ebeced"/></svg>') 1 3 1 1;
  padding-left: 8px;
}

.-theme-with-dark-background .CodeMirror-linenumber:hover,
:host-context(.-theme-with-dark-background) .CodeMirror-linenumber:hover {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%233c4043" stroke="%233c4043"/></svg>') 1 3 1 1;
}

.cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color: #fff;

  color: var(--override-auto-gen-cmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%234285f4" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%235186EC" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.cm-breakpoint-disabled .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.breakpoints-deactivated .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointdisabledcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color: #1a73e8;

  color: var(--override-auto-gen-cmbreakpointdisabledcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23d9e7fd" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-disabled .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-with-dark-background .breakpoints-deactivated .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-disabled .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .breakpoints-deactivated .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  color: #1a73e8;
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%232a384e" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23f29900" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23e9a33a" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.cm-breakpoint-disabled.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.breakpoints-deactivated .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointdisabledcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-color: #e37400;

  color: var(--override-auto-gen-cmbreakpointdisabledcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23fcebcc" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-disabled.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-with-dark-background .breakpoints-deactivated .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-disabled.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .breakpoints-deactivated .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  color: #e37400;
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%234d3c1d" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23f439a0" stroke="%23d01884"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23E54D9B" stroke="%23d01884"/></svg>') 1 3 1 1;
}

.cm-breakpoint-disabled.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.breakpoints-deactivated .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointdisabledcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-color: #d01884;

  color: var(--override-auto-gen-cmbreakpointdisabledcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23fdd7ec" stroke="%23f439a0"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-disabled.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-with-dark-background .breakpoints-deactivated .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-disabled.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .breakpoints-deactivated .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  color: #d01884;
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%234e283d" stroke="%23f439a0"/></svg>') 1 3 1 1;
}

.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber::before,
.-theme-preserve {
  content: "?";
  position: absolute;
  top: 0;
  left: 1px;
}

.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber::before,
.-theme-preserve {
  content: "‥";
  position: absolute;
  top: -3px;
  left: 1px;
}

.cm-inline-breakpoint {
  cursor: pointer;
  position: relative;
  top: 1px;
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%234285F4" stroke="%231A73E8"/></svg>');
  height: 10px;
}

.-theme-with-dark-background .cm-inline-breakpoint,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%235186EC" stroke="%231A73E8"/></svg>');
}

.cm-inline-breakpoint.cm-inline-disabled,
.breakpoints-deactivated .cm-inline-breakpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%234285F4" fill-opacity="0.2" stroke="%231A73E8"/></svg>');
}

.cm-inline-breakpoint.cm-inline-breakpoint-conditional {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.75489 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.75489 11.2583 6.29382 11.5 5.80138 11.5H0.5V0.5Z" fill="%23F29900" stroke="%23E37400"/><path d="M3.51074 7.75635H4.68408V9H3.51074V7.75635ZM4.68408 7.23779H3.51074V6.56104C3.51074 6.271 3.55615 6.02344 3.64697 5.81836C3.73779 5.61328 3.90039 5.39648 4.13477 5.16797L4.53027 4.77686C4.71484 4.59814 4.83936 4.4502 4.90381 4.33301C4.97119 4.21582 5.00488 4.09424 5.00488 3.96826C5.00488 3.77197 4.9375 3.62402 4.80273 3.52441C4.66797 3.4248 4.46582 3.375 4.19629 3.375C3.9502 3.375 3.69238 3.42773 3.42285 3.5332C3.15625 3.63574 2.88232 3.78955 2.60107 3.99463V2.81689C2.88818 2.65283 3.17822 2.52979 3.47119 2.44775C3.76709 2.36279 4.06299 2.32031 4.35889 2.32031C4.95068 2.32031 5.41504 2.45801 5.75195 2.7334C6.08887 3.00879 6.25732 3.38818 6.25732 3.87158C6.25732 4.09424 6.20752 4.30225 6.10791 4.49561C6.0083 4.68604 5.8208 4.91602 5.54541 5.18555L5.15869 5.56348C4.95947 5.75684 4.83203 5.91504 4.77637 6.03809C4.7207 6.16113 4.69287 6.31201 4.69287 6.49072C4.69287 6.51709 4.69141 6.54785 4.68848 6.58301C4.68848 6.61816 4.68701 6.65625 4.68408 6.69727V7.23779Z" fill="white"/></svg>');
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-inline-breakpoint-conditional,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-inline-breakpoint-conditional {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.75489 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.75489 11.2583 6.29382 11.5 5.80138 11.5H0.5V0.5Z" fill="%23e9a33a" stroke="%23E37400"/><path d="M3.51074 7.75635H4.68408V9H3.51074V7.75635ZM4.68408 7.23779H3.51074V6.56104C3.51074 6.271 3.55615 6.02344 3.64697 5.81836C3.73779 5.61328 3.90039 5.39648 4.13477 5.16797L4.53027 4.77686C4.71484 4.59814 4.83936 4.4502 4.90381 4.33301C4.97119 4.21582 5.00488 4.09424 5.00488 3.96826C5.00488 3.77197 4.9375 3.62402 4.80273 3.52441C4.66797 3.4248 4.46582 3.375 4.19629 3.375C3.9502 3.375 3.69238 3.42773 3.42285 3.5332C3.15625 3.63574 2.88232 3.78955 2.60107 3.99463V2.81689C2.88818 2.65283 3.17822 2.52979 3.47119 2.44775C3.76709 2.36279 4.06299 2.32031 4.35889 2.32031C4.95068 2.32031 5.41504 2.45801 5.75195 2.7334C6.08887 3.00879 6.25732 3.38818 6.25732 3.87158C6.25732 4.09424 6.20752 4.30225 6.10791 4.49561C6.0083 4.68604 5.8208 4.91602 5.54541 5.18555L5.15869 5.56348C4.95947 5.75684 4.83203 5.91504 4.77637 6.03809C4.7207 6.16113 4.69287 6.31201 4.69287 6.49072C4.69287 6.51709 4.69141 6.54785 4.68848 6.58301C4.68848 6.61816 4.68701 6.65625 4.68408 6.69727V7.23779Z" fill="white"/></svg>');
}

.cm-inline-breakpoint.cm-inline-breakpoint-conditional.cm-inline-disabled,
.breakpoints-deactivated .cm-inline-breakpoint.cm-inline-breakpoint-conditional {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.75489 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.75489 11.2583 6.29382 11.5 5.80138 11.5H0.5V0.5Z" fill="%23F9AB00" fill-opacity="0.2" stroke="%23E37400"/><path d="M3.51074 7.75635H4.68408V9H3.51074V7.75635ZM4.68408 7.23779H3.51074V6.56104C3.51074 6.271 3.55615 6.02344 3.64697 5.81836C3.73779 5.61328 3.90039 5.39648 4.13477 5.16797L4.53027 4.77686C4.71484 4.59814 4.83936 4.4502 4.90381 4.33301C4.97119 4.21582 5.00488 4.09424 5.00488 3.96826C5.00488 3.77197 4.9375 3.62402 4.80273 3.52441C4.66797 3.4248 4.46582 3.375 4.19629 3.375C3.9502 3.375 3.69238 3.42773 3.42285 3.5332C3.15625 3.63574 2.88232 3.78955 2.60107 3.99463V2.81689C2.88818 2.65283 3.17822 2.52979 3.47119 2.44775C3.76709 2.36279 4.06299 2.32031 4.35889 2.32031C4.95068 2.32031 5.41504 2.45801 5.75195 2.7334C6.08887 3.00879 6.25732 3.38818 6.25732 3.87158C6.25732 4.09424 6.20752 4.30225 6.10791 4.49561C6.0083 4.68604 5.8208 4.91602 5.54541 5.18555L5.15869 5.56348C4.95947 5.75684 4.83203 5.91504 4.77637 6.03809C4.7207 6.16113 4.69287 6.31201 4.69287 6.49072C4.69287 6.51709 4.69141 6.54785 4.68848 6.58301C4.68848 6.61816 4.68701 6.65625 4.68408 6.69727V7.23779Z" fill="%23E37400"/></svg>');
}

.cm-inline-breakpoint.cm-inline-logpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%23F439A0" stroke="%23D01884"/><circle cx="3" cy="6" r="1" fill="white"/><circle cx="7" cy="6" r="1" fill="white"/></svg>');
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-inline-logpoint,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-inline-logpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%23E54D9B" stroke="%23D01884"/><circle cx="3" cy="6" r="1" fill="white"/><circle cx="7" cy="6" r="1" fill="white"/></svg>');
}

.cm-inline-breakpoint.cm-inline-logpoint.cm-inline-disabled,
.breakpoints-deactivated .cm-inline-breakpoint.cm-inline-logpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%23F439A0" fill-opacity="0.2" stroke="%23D01884"/><circle cx="3" cy="6" r="1" fill="%23D01884"/><circle cx="7" cy="6" r="1" fill="%23D01884"/></svg>');
}

.cm-execution-line-tail + .CodeMirror-widget {
  --override-auto-gen-cmexecutionlinetailcodemirrorwidget-backgroundcolor: #abbffe;

  background-color: var(--override-auto-gen-cmexecutionlinetailcodemirrorwidget-backgroundcolor);
}

.-theme-with-dark-background .cm-execution-line-tail + .CodeMirror-widget,
:host-context(.-theme-with-dark-background) .cm-execution-line-tail + .CodeMirror-widget {
  --override-auto-gen-cmexecutionlinetailcodemirrorwidget-backgroundcolor: rgb(1 21 84);
}

.source-frame-eval-expression + .CodeMirror-widget {
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-backgroundcolor: rgb(255 255 194);
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-border: rgb(163 41 34);

  border: 1px solid var(--override-auto-gen-sourceframeevalexpressioncodemirrorwidget-border);
  border-left-width: 0;
  border-right-width: 0;
  background-color: var(--override-auto-gen-sourceframeevalexpressioncodemirrorwidget-backgroundcolor);
}

.-theme-with-dark-background .source-frame-eval-expression + .CodeMirror-widget,
:host-context(.-theme-with-dark-background) .source-frame-eval-expression + .CodeMirror-widget {
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-border: rgb(221 99 92);
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-backgroundcolor: rgb(61 61 0);
}

.cm-inline-breakpoint.cm-execution-line-tail {
  --override-auto-gen-cminlinebreakpointcmexecutionlinetail-backgroundcolor: #698cfe;

  background-color: var(--override-auto-gen-cminlinebreakpointcmexecutionlinetail-backgroundcolor);
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-execution-line-tail,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-execution-line-tail {
  --override-auto-gen-cminlinebreakpointcmexecutionlinetail-backgroundcolor: rgb(1 36 150);
}

.cm-execution-line-tail .cm-inline-breakpoint {
  background-color: var(--color-background);
}

.cm-inline-breakpoint.cm-inline-conditional {
  --override-auto-gen-cminlinebreakpointcminlineconditional-backgroundcolor: #ef9d0d;

  background-color: var(--override-auto-gen-cminlinebreakpointcminlineconditional-backgroundcolor);
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-inline-conditional,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-inline-conditional {
  --override-auto-gen-cminlinebreakpointcminlineconditional-backgroundcolor: rgb(242 160 16);
}

.cm-continue-to-location {
  cursor: pointer;
  opacity: 80%;
  position: relative;
  top: 2px;
}

.cm-continue-to-location:hover {
  opacity: 100%;
}

div.CodeMirror:focus-within span.CodeMirror-matchingbracket {
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-borderbottom: rgb(0 0 0 / 50%);
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-backgroundcolor: rgb(0 0 0 / 7%);

  background-color: var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-backgroundcolor);
  border-bottom: 1px solid var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-borderbottom);
}

div.CodeMirror:focus-within span.CodeMirror-nonmatchingbracket {
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-borderbottom: rgb(255 0 0 / 50%);
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-backgroundcolor: rgb(255 0 0 / 7%);

  background-color: var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-backgroundcolor);
  border-bottom: 1px solid var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-borderbottom);
}

.-theme-with-dark-background div.CodeMirror:focus-within span.CodeMirror-matchingbracket,
:host-context(.-theme-with-dark-background) div.CodeMirror:focus-within span.CodeMirror-matchingbracket {
  border-bottom: 1px solid rgb(217 217 217);
  background-color: initial;
}

.-theme-with-dark-background div.CodeMirror:focus-within span.CodeMirror-nonmatchingbracket,
:host-context(.-theme-with-dark-background) div.CodeMirror:focus-within span.CodeMirror-nonmatchingbracket {
  border-bottom: 1px solid rgb(255 26 26);
  background-color: initial;
}

.cm-whitespace::before {
  --override-auto-gen-cmwhitespacebefore-color: rgb(175 175 175);

  position: absolute;
  pointer-events: none;
  color: var(--override-auto-gen-cmwhitespacebefore-color);
}

.-theme-with-dark-background .cm-whitespace::before,
:host-context(.-theme-with-dark-background) .cm-whitespace::before {
  --override-auto-gen-cmwhitespacebefore-color: rgb(80 80 80);
}

.cm-tab {
  display: inline-block;
  text-decoration: inherit;
  position: relative;
}

.cm-tab::before {
  --override-auto-gen-cmtabbefore-borderbottom: rgb(175 175 175);

  display: none;
  content: ".";
  color: transparent;
  border-bottom: 1px solid var(--override-auto-gen-cmtabbefore-borderbottom);
  position: absolute;
  width: 90%;
  bottom: 50%;
  left: 5%;
}

.-theme-with-dark-background .cm-tab::before,
:host-context(.-theme-with-dark-background) .cm-tab::before {
  --override-auto-gen-cmtabbefore-borderbottom: rgb(80 80 80);
}

.show-whitespaces .CodeMirror .cm-tab::before {
  display: block !important; /* stylelint-disable-line declaration-no-important */
}

.cm-execution-line {
  --override-auto-gen-cmexecutionline-backgroundcolor: rgb(0 59 255 / 10%);

  background-color: var(--override-auto-gen-cmexecutionline-backgroundcolor);
}

.cm-execution-line-outline {
  --override-auto-gen-cmexecutionlineoutline-outline: rgb(64 115 244);

  outline: 1px solid var(--override-auto-gen-cmexecutionlineoutline-outline);
}

.cm-execution-line-tail {
  --override-auto-gen-cmexecutionlinetail-backgroundcolor: rgb(171 191 254);

  background-color: var(--override-auto-gen-cmexecutionlinetail-backgroundcolor);
}

.-theme-with-dark-background .cm-execution-line,
:host-context(.-theme-with-dark-background) .cm-execution-line {
  background-color: #14522b;
}

.-theme-with-dark-background .cm-execution-line-outline,
:host-context(.-theme-with-dark-background) .cm-execution-line-outline {
  outline: 1px solid #33cc6b;
}

.-theme-with-dark-background .cm-execution-line-tail,
:host-context(.-theme-with-dark-background) .cm-execution-line-tail {
  background-color: #347132;
}

.cm-token-highlight {
  position: relative;
}

.cm-token-highlight::before {
  position: absolute;
  border: 1px solid var(--override-search-highlight-border-color);
  border-radius: 3px;
  top: 0;
  bottom: -1px;
  left: 0;
  right: 0;
  content: "";
}

.cm-line-with-selection .cm-column-with-selection::before {
  border: none;
}

.cm-search-highlight {
  position: relative;
}

.cm-search-highlight::before {
  position: absolute;
  border-top-style: solid;
  border-bottom-style: solid;
  border-top-color: var(--override-search-highlight-border-color);
  border-bottom-color: var(--override-search-highlight-border-color);
  border-top-width: 1px;
  border-bottom-width: 1px;
  top: -1px;
  bottom: 0;
  left: 0;
  right: 0;
  content: "";
}

.cm-search-highlight-full::before {
  border: 1px solid var(--override-search-highlight-border-color);
  border-radius: 3px;
}

.cm-search-highlight-start::before {
  border-left-width: 1px;
  border-top-left-radius: 2px;
  border-bottom-left-radius: 2px;
  border-left-style: solid;
  border-left-color: var(--override-search-highlight-border-color);
}

.cm-search-highlight-end::before {
  border-right-width: 1px;
  border-top-right-radius: 2px;
  border-bottom-right-radius: 2px;
  border-right-style: solid;
  border-right-color: var(--override-search-highlight-border-color);
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight-full::before {
  border-radius: 1px;
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight-start::before {
  border-top-left-radius: 1px;
  border-bottom-left-radius: 1px;
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight-end::before {
  border-top-right-radius: 1px;
  border-bottom-right-radius: 1px;
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight::before {
  --override-auto-gen-cmlinewithselectioncmcolumnwithselectioncmsearchhighlightbefore-backgroundcolor: rgb(241 234 0);

  margin: -1px -1px -1px -1px;
  background-color: var(--override-auto-gen-cmlinewithselectioncmcolumnwithselectioncmsearchhighlightbefore-backgroundcolor);
  z-index: -1;
}

.-theme-with-dark-background .cm-line-with-selection .cm-column-with-selection.cm-search-highlight::before,
:host-context(.-theme-with-dark-background) .cm-line-with-selection .cm-column-with-selection.cm-search-highlight::before {
  background-color: hsl(133deg 100% 30%);
}

.-theme-with-dark-background .cm-line-with-selection .cm-search-highlight,
:host-context(.-theme-with-dark-background) .cm-line-with-selection .cm-search-highlight {
  color: #eee;
}

.CodeMirror .text-editor-line-marker-text {
  text-align: right;
  padding-right: 3px;
  height: 12px;
}

.CodeMirror .text-editor-line-marker-text span.line-marker-units {
  color: var(--color-text-secondary);
  font-size: 75%;
  margin-left: 3px;
}

.CodeMirror .text-editor-coverage-unused-marker {
  text-align: right;
  padding-right: 2px;
  background-color: var(--color-accent-red);
}

.CodeMirror .text-editor-coverage-unused-marker::after {
  content: "\200B";
}

.CodeMirror .text-editor-coverage-used-marker {
  --override-auto-gen-codemirrortexteditorcoverageusedmarker-backgroundcolor: #63acbe;

  text-align: right;
  padding-right: 2px;
  background-color: var(--override-auto-gen-codemirrortexteditorcoverageusedmarker-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .text-editor-coverage-used-marker,
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-coverage-used-marker {
  --override-auto-gen-codemirrortexteditorcoverageusedmarker-backgroundcolor: rgb(65 138 156);
}

.CodeMirror .text-editor-coverage-used-marker::after {
  content: "\200B";
}

.CodeMirror .text-editor-line-decoration {
  position: absolute;
}

.CodeMirror .text-editor-line-decoration-wave {
  position: absolute;
  top: -2px;
  right: -4px;
  left: 4px;
  cursor: pointer;
  height: 4px;
  background-image: var(--image-file-errorWave);
  background-repeat: repeat-x;
  background-size: contain;
}

.CodeMirror .text-editor-value-decoration {
  --override-auto-gen-codemirrortexteditorvaluedecoration-backgroundcolor: #ffe3c7;

  position: absolute;
  bottom: 0;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  max-width: 1000px;
  opacity: 80%;
  background-color: var(--override-auto-gen-codemirrortexteditorvaluedecoration-backgroundcolor);
  margin-left: 10px;
  padding-left: 5px;
  color: var(--color-text-primary);
  user-select: text;
}

.-theme-with-dark-background .CodeMirror .text-editor-value-decoration,
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-value-decoration {
  --override-auto-gen-codemirrortexteditorvaluedecoration-backgroundcolor: rgb(56 28 0);
}

.CodeMirror .cm-execution-line .text-editor-value-decoration {
  background-color: transparent;
  opacity: 50%;
}

.CodeMirror .text-editor-line-decoration-icon {
  cursor: pointer;
}

.CodeMirror .text-editor-line-decoration-icon > * {
  vertical-align: text-bottom;
  margin-left: 2px;
}

.CodeMirror .text-editor-line-decoration-icon-issue {
  cursor: pointer;
}

.CodeMirror .text-editor-line-with-warning:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewithwarningnotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(241 230 0 / 10%);

  background-color: var(--override-auto-gen-codemirrortexteditorlinewithwarningnotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .text-editor-line-with-warning:not(.cm-execution-line):not(.cm-readonly-highlight),
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-line-with-warning:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewithwarningnotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(255 244 14 / 10%);
}

.CodeMirror .text-editor-line-with-error:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewitherrornotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(255 0 0 / 5%);

  background-color: var(--override-auto-gen-codemirrortexteditorlinewitherrornotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .text-editor-line-with-error:not(.cm-execution-line):not(.cm-readonly-highlight),
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-line-with-error:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewitherrornotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(255 0 0 / 5%);
}

.CodeMirror .CodeMirror-vscrollbar,
.CodeMirror .CodeMirror-hscrollbar {
  transform: translateZ(0);
}

.cm-trailing-whitespace {
  --override-auto-gen-cmtrailingwhitespace-backgroundcolor: rgb(255 0 0 / 5%);

  background-color: var(--override-auto-gen-cmtrailingwhitespace-backgroundcolor);
}

.-theme-with-dark-background .cm-trailing-whitespace,
:host-context(.-theme-with-dark-background) .cm-trailing-whitespace {
  --override-auto-gen-cmtrailingwhitespace-backgroundcolor: rgb(255 0 0 / 5%);
}

.CodeMirror-activeline .cm-trailing-whitespace {
  background-color: transparent;
}

.CodeMirror .CodeMirror-selected {
  background-color: var(--legacy-item-selection-inactive-bg-color);
}

.CodeMirror-focused .CodeMirror-selected {
  background-color: var(--legacy-item-selection-bg-color);
}

.-theme-with-dark-background .CodeMirror .CodeMirror-selected,
:host-context(.-theme-with-dark-background) .CodeMirror .CodeMirror-selected {
  background-color: #454545;
}

.-theme-with-dark-background span.CodeMirror-selectedtext,
:host-context(.-theme-with-dark-background) span.CodeMirror-selectedtext {
  background-color: #454545;
}

.CodeMirror .auto-complete-text {
  color: var(--color-text-secondary);
}

.CodeMirror .placeholder-text {
  height: 0;
  color: var(--color-text-secondary);
}

.CodeMirror textarea {
  resize: none;
  overflow: hidden;
}

.CodeMirror-lines {
  padding: 4px 0; /* Vertical padding around content */
}

.CodeMirror pre {
  padding: 0 4px; /* Horizontal padding of content */
}

.CodeMirror-scrollbar-filler,
.CodeMirror-gutter-filler {
  /* The little square between H and V scrollbars */
  background-color: var(--color-background);
}

.CodeMirror div.CodeMirror-secondarycursor {
  --override-auto-gen-codemirrordivcodemirrorsecondarycursor-borderleft: #c0c0c0;

  border-left: 1px solid var(--override-auto-gen-codemirrordivcodemirrorsecondarycursor-borderleft);
}

.-theme-with-dark-background .CodeMirror div.CodeMirror-secondarycursor,
:host-context(.-theme-with-dark-background) .CodeMirror div.CodeMirror-secondarycursor {
  --override-auto-gen-codemirrordivcodemirrorsecondarycursor-borderleft: rgb(63 63 63);
}

.CodeMirror-composing {
  border-bottom: 2px solid;
}

.CodeMirror-foldmarker {
  cursor: pointer;
  font-size: 0;
  line-height: 0;
  height: 0;
}

.CodeMirror-foldmarker::before {
  content: '\2026';
  font-size: 13px;
  color: var(--color-text-secondary);
}

.CodeMirror-foldgutter {
  width: 1.5em;
}

.CodeMirror-gutters:hover .CodeMirror-foldgutter {
  background-color: transparent;
}

.CodeMirror-foldgutter-open,
.CodeMirror-foldgutter-folded {
  cursor: pointer;
  position: relative;
}

.CodeMirror-foldgutter-open {
  transition: opacity 0.2s;
  opacity: 0%;
}

.CodeMirror-gutter-hovered .CodeMirror-foldgutter-open {
  opacity: 100%;
}

.CodeMirror-foldgutter-open::before,
.CodeMirror-foldgutter-folded::before {
  background-color: var(--color-text-secondary);
  user-select: none;
  -webkit-mask-image: var(--image-file-treeoutlineTriangles);
  -webkit-mask-size: 32px 24px;
  content: "";
  display: block;
  width: 8px;
  color: transparent;
  text-shadow: none;
  height: 12px;
  position: absolute;
  right: 4px;
}

.CodeMirror-foldgutter-open::before {
  -webkit-mask-position: -16px 0;
}

.CodeMirror-foldgutter-folded::before {
  -webkit-mask-position: 0 0;
}

.CodeMirror .CodeMirror-line::selection,
.CodeMirror .CodeMirror-line > span::selection,
.CodeMirror .CodeMirror-line > span > span::selection {
  background: var(--legacy-item-selection-bg-color);
}

@media (forced-colors: active) {
  .cm-token-highlight::before {
    forced-color-adjust: none;
    border-color: Highlight;
  }
}

/* stylelint-enable no-descending-specificity */

/*# sourceURL=ui/legacy/components/text_editor/cmdevtools.css */x<script type="text/javascript" src="js/__modules__.js"></script>: 20px; bottom: 1.76951e-08px; position: absolute; color: rgb(255, 165, 0);"></canvas><iframe src="https://audius.co/embed/playlist/DOPRl?flavor=card" id="Audius" style="width: 357px; height: 550px; right: 15.9898px; bottom: 273.635px; border: none; position: absolute; display: none; transform: scale(0.799491, 0.799491); transform-origin: right bottom;"></iframe><a id="link"></a></body>
    }</style><style type="text/css"></style></head><script type="text/javascript" src="js/__start__.js?v=1.1.213"></script>/* The rest of this file contains styles related to the mechanics of
   the editor. You probably shouldn't touch them. */

.CodeMirror {
  position: relative;
  overflow: hidden;
  background: var(--color-background);
}

.CodeMirror-scroll {
  overflow: scroll !important; /* Things will break if this is overridden */
  /* 50px is the magic margin used to hide the element's real scrollbars */
  /* See overflow: hidden in .CodeMirror */
  margin-bottom: -50px;
  margin-right: -50px;
  padding-bottom: 50px;
  height: 100%;
  outline: none; /* Prevent dragging from highlighting the element */
  position: relative;
}

.CodeMirror-sizer {
  position: relative;
  border-right: 50px solid transparent;
}

/* The fake, visible scrollbars. Used to force redraw during scrolling
   before actual scrolling happens, thus preventing shaking and
   flickering artifacts. */
.CodeMirror-vscrollbar,
.CodeMirror-hscrollbar,
.CodeMirror-scrollbar-filler,
.CodeMirror-gutter-filler {
  position: absolute;
  z-index: 6;
  display: none;
  outline: none;
}

.CodeMirror-vscrollbar {
  right: 0;
  top: 0;
  overflow-x: hidden;
  overflow-y: scroll;
}

.CodeMirror-hscrollbar {
  bottom: 0;
  left: 0;
  overflow-y: hidden;
  overflow-x: scroll;
}

.CodeMirror-scrollbar-filler {
  right: 0;
  bottom: 0;
}

.CodeMirror-gutter-filler {
  left: 0;
  bottom: 0;
}

.CodeMirror-gutters {
  position: absolute;
  left: 0;
  top: 0;
  min-height: 100%;
  z-index: 3;
}

.CodeMirror-gutter {
  white-space: normal;
  height: 100%;
  display: inline-block;
  vertical-align: top;
  margin-bottom: -50px;
}

.CodeMirror-gutter-wrapper {
  position: absolute;
  z-index: 4;
  background: none !important;
  border: none !important;
}

.CodeMirror-gutter-background {
  position: absolute;
  top: 0;
  bottom: 0;
  z-index: 4;
}

.CodeMirror-gutter-elt {
  position: absolute;
  cursor: default;
  z-index: 4;
}

.CodeMirror-gutter-wrapper ::selection {
  background-color: transparent;
}

.CodeMirror-gutter-wrapper ::-moz-selection {
  background-color: transparent;
}

.CodeMirror-lines {
  cursor: text;
  min-height: 1px; /* prevents collapsing before first draw */
}

.CodeMirror pre.CodeMirror-line,
.CodeMirror pre.CodeMirror-line-like {
  /* Reset some styles that the rest of the page might have set */
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -moz-border-radius: 0;
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -webkit-border-radius: 0;
  border-radius: 0;
  border-width: 0;
  background: transparent;
  font-family: inherit;
  font-size: inherit;
  margin: 0;
  white-space: pre;
  word-wrap: normal;
  line-height: inherit;
  color: inherit;
  z-index: 2;
  position: relative;
  overflow: visible;
  -webkit-tap-highlight-color: transparent;
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -webkit-font-variant-ligatures: contextual;
  font-variant-ligatures: contextual;
}

.CodeMirror-wrap pre.CodeMirror-line,
.CodeMirror-wrap pre.CodeMirror-line-like {
  word-wrap: break-word;
  white-space: pre-wrap;
  word-break: normal;
}

.CodeMirror-linebackground {
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  z-index: 0;
}

.CodeMirror-linewidget {
  position: relative;
  z-index: 2;
  padding: 0.1px; /* Force widget margins to stay inside of the container */
}

.CodeMirror-rtl pre {
  direction: rtl;
}

.CodeMirror-code {
  outline: none;
}

/* Force content-box sizing for the elements where we expect it */
.CodeMirror-scroll,
.CodeMirror-sizer,
.CodeMirror-gutter,
.CodeMirror-gutters,
.CodeMirror-linenumber {
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -moz-box-sizing: content-box;
  box-sizing: content-box;
}

.CodeMirror-measure {
  position: absolute;
  width: 100%;
  height: 0;
  overflow: hidden;
  visibility: hidden;
}

.CodeMirror-cursor {
  position: absolute;
  pointer-events: none;
}

.CodeMirror-measure pre {
  position: static;
}

div.CodeMirror-cursors {
  visibility: hidden;
  position: relative;
  z-index: 3;
}

div.CodeMirror-dragcursors {
  visibility: visible;
}

.CodeMirror-focused div.CodeMirror-cursors {
  visibility: visible;
}

.CodeMirror-selected {
  --override-cm-selected-background-color: #d9d9d9;

  background: var(--override-cm-selected-background-color);
}

.-theme-with-dark-background .CodeMirror-selected,
:host-context(.-theme-with-dark-background) .CodeMirror-selected {
  --override-cm-selected-background-color: rgb(38 38 38);
}

.CodeMirror-focused .CodeMirror-selected {
  --override-cm-selected-background-color: #d7d4f0;
}

.-theme-with-dark-background .CodeMirror-focused .CodeMirror-selected,
:host-context(.-theme-with-dark-background) .CodeMirror-focused .CodeMirror-selected {
  --override-cm-selected-background-color: rgb(18 15 43);
}

.CodeMirror-crosshair {
  cursor: crosshair;
}

.CodeMirror-line {
  --override-line-selection-background-color: #d7d4f0;
}

.CodeMirror-line::selection,
.CodeMirror-line > span::selection,
.CodeMirror-line > span > span::selection {
  background:var(--override-line-selection-background-color);
}

.CodeMirror-line::-moz-selection,
.CodeMirror-line > span::-moz-selection,
.CodeMirror-line > span > span::-moz-selection {
  background: var(--override-line-selection-background-color);
}

.-theme-with-dark-background .CodeMirror-line,
:host-context(.-theme-with-dark-background) .CodeMirror-line {
  --override-line-selection-background-color: rgb(18 15 43);

}

.cm-searching {
  --override-searching-background-color: rgb(255 255 0 / 40%);

  background-color: var(--override-searching-background-color);
}

/* Used to force a border model for a node */
.cm-force-border {
  padding-right: 0.1px;
}

@media print {
  /* Hide the cursor when printing */
  .CodeMirror div.CodeMirror-cursors {
    visibility: hidden;
  }
}

/* See issue #2901 */
.cm-tab-wrap-hack::after {
  content: "";
}

/* Help users use markselection to safely style text background */
span.CodeMirror-selectedtext {
  background: none;
}

/*# sourceURL=third_party/codemirror/codemirror.css *//*
 * Copyright 2021 The Chromium Authors. All rights reserved.
 * Use of this source code is governed by a BSD-style license that can be
 * found in the LICENSE file.
 */

/* stylelint-disable no-descending-specificity */

/**
 * Many of the CSS variables here were auto generated during the dark mode
 * migration. If you are changing them, please feel free to rename them whilst
 * you're here to make them clearer.
 */

.CodeMirror {
  --override-search-highlight-border-color: rgb(128 128 128);

  line-height: 1.2em !important; /* stylelint-disable-line declaration-no-important */
  background-color: transparent !important; /* stylelint-disable-line declaration-no-important */
  color: var(--color-text-primary);
  height: 300px;
}

.CodeMirror-linewidget {
  overflow: visible !important; /* stylelint-disable-line declaration-no-important */
}

.CodeMirror-gutter-performance {
  width: 60px;
  background-color: var(--color-background);
  margin-left: 3px;
}

.CodeMirror-gutter-memory {
  width: 48px;
  background-color: var(--color-background);
  margin-left: 3px;
}

.CodeMirror-gutter-coverage {
  width: 5px;
  background-color: var(--color-background);
  margin-left: 3px;
}

.CodeMirror .source-frame-eval-expression {
  --override-auto-gen-codemirrorsourceframeevalexpression-backgroundcolor: rgb(255 255 194);
  --override-auto-gen-codemirrorsourceframeevalexpression-border: rgb(163 41 34);

  outline: 0;
  border: 1px solid var(--override-auto-gen-codemirrorsourceframeevalexpression-border);
  border-left-width: 0;
  border-right-width: 0;
  background-color: var(--override-auto-gen-codemirrorsourceframeevalexpression-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .source-frame-eval-expression,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-eval-expression {
  --override-auto-gen-codemirrorsourceframeevalexpression-border: rgb(221 99 92);
  --override-auto-gen-codemirrorsourceframeevalexpression-backgroundcolor: rgb(61 61 0);
}

.CodeMirror .source-frame-eval-expression-start {
  border-left-width: 1px;
  margin-left: -1px;
}

.CodeMirror .source-frame-eval-expression-end {
  border-right-width: 1px;
  margin-right: -1px;
}

.CodeMirror .source-frame-continue-to-location {
  --override-auto-gen-codemirrorsourceframecontinuetolocation-backgroundcolor: rgb(230 236 255);

  outline: 0;
  border: 1px solid transparent;
  border-left-width: 0;
  border-right-width: 0;
  background-color: var(--override-auto-gen-codemirrorsourceframecontinuetolocation-backgroundcolor);
  cursor: pointer;
}

.CodeMirror .source-frame-continue-to-location:hover {
  --override-auto-gen-codemirrorsourceframecontinuetolocationhover-backgroundcolor: rgb(171 191 254);
  --override-auto-gen-codemirrorsourceframecontinuetolocationhover-border: rgb(121 141 254);

  border: 1px solid var(--override-auto-gen-codemirrorsourceframecontinuetolocationhover-border);
  background-color: var(--override-auto-gen-codemirrorsourceframecontinuetolocationhover-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .source-frame-continue-to-location,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-continue-to-location {
  background-color: #14522b;
}

.-theme-with-dark-background .CodeMirror .source-frame-continue-to-location:hover,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-continue-to-location:hover {
  border: 1px solid #33cc6b;
  background-color: #14522b;
}

.CodeMirror .source-frame-continue-to-location-start {
  border-left-width: 1px;
  margin-left: -1px;
}

.CodeMirror .source-frame-continue-to-location-end {
  border-right-width: 1px;
  margin-right: -1px;
}

.CodeMirror .source-frame-async-step-in {
  --override-auto-gen-codemirrorsourceframeasyncstepin-backgroundcolor: hsl(100deg 46% 80% / 100%);

  outline: 0;
  background-color: var(--override-auto-gen-codemirrorsourceframeasyncstepin-backgroundcolor);
  cursor: pointer;
  border: 1px solid transparent;
  border-left-width: 0;
  border-right-width: 0;
}

.-theme-with-dark-background .CodeMirror .source-frame-async-step-in,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-async-step-in {
  --override-auto-gen-codemirrorsourceframeasyncstepin-backgroundcolor: rgb(43 74 28);
}

.source-frame-async-step-in-hovered .source-frame-async-step-in {
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-bordercolor: rgb(100 154 100);
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-backgroundcolor: hsl(96deg 53% 65%);

  background-color: var(--override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-backgroundcolor);
  border-color: var(--override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-bordercolor);
}

.-theme-with-dark-background .source-frame-async-step-in-hovered .source-frame-async-step-in,
:host-context(.-theme-with-dark-background) .source-frame-async-step-in-hovered .source-frame-async-step-in {
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-backgroundcolor: rgb(80 137 42);
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-bordercolor: rgb(101 155 101);
}

.source-frame-async-step-in-hovered .source-frame-async-step-in-start {
  border-left-width: 1px;
  margin-left: -1px;
}

.source-frame-async-step-in-hovered .source-frame-async-step-in-end {
  border-right-width: 1px;
  margin-right: -1px;
}

.CodeMirror-cursor {
  border-left: 1px solid var(--color-background-inverted);
  border-right: none;
  width: 0;
}

.CodeMirror-readonly .CodeMirror-cursor {
  display: none;
}

.CodeMirror-gutters {
  border-right: 1px solid var(--color-details-hairline);
  white-space: nowrap;
  background-color: var(--color-background);
}

.CodeMirror-linenumber {
  --override-auto-gen-codemirrorlinenumber-color: hsl(0deg 0% 46%);

  color: var(--override-auto-gen-codemirrorlinenumber-color);
  padding: 0 3px 0 9px;
  min-width: 28px;
  text-align: right;
  white-space: nowrap;
}

.-theme-with-dark-background .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .CodeMirror-linenumber {
  --override-auto-gen-codemirrorlinenumber-color: rgb(138 138 138);
}

.pretty-printed .CodeMirror-linenumber {
  color: var(--legacy-accent-color);
}

.cm-non-breakable-line .CodeMirror-linenumber {
  --override-auto-gen-cmnonbreakablelinecodemirrorlinenumber-color: rgb(128 128 128 / 40%);

  color: var(--override-auto-gen-cmnonbreakablelinecodemirrorlinenumber-color);
}

.-theme-with-dark-background .cm-non-breakable-line .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-non-breakable-line .CodeMirror-linenumber {
  --override-auto-gen-cmnonbreakablelinecodemirrorlinenumber-color: rgb(127 127 127 / 40%);
}

.cm-highlight {
  animation: fadeout 2s 0s;
}

.-theme-with-dark-background .cm-highlight,
:host-context(.-theme-with-dark-background) .cm-highlight {
  animation: fadeout-dark 2s 0s;
}

@keyframes fadeout {
  from {
    background-color: rgb(255 255 120); /* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: var(--color-background); }
}

@keyframes fadeout {
  from {
    background-color: rgb(255 255 120); /* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: var(--color-background); }
}

@keyframes fadeout-dark {
  from {
    background-color: hsl(133deg 100% 30% / 50%);/* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: transparent; }
}

@keyframes fadeout-dark {
  from {
    background-color: hsl(133deg 100% 30% / 50%);/* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: transparent; }
}

.cm-readonly-highlight {
  --override-auto-gen-cmreadonlyhighlight-backgroundcolor: rgb(255 255 120);

  background-color: var(--override-auto-gen-cmreadonlyhighlight-backgroundcolor);
}

.-theme-with-dark-background .cm-readonly-highlight,
:host-context(.-theme-with-dark-background) .cm-readonly-highlight {
  background-color: hsl(133deg 100% 30% / 50%);
}

.cm-highlight.cm-execution-line {
  animation: fadeout-execution-line 1s 0s;
}

.-theme-with-dark-background .cm-highlight.cm-execution-line,
:host-context(.-theme-with-dark-background) .cm-highlight.cm-execution-line {
  animation: fadeout-execution-line-dark 1s 0s;
}

@keyframes fadeout-execution-line {
  from {
    background-color: rgb(121 141 254);/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: rgb(171 191 254);/* stylelint-disable-line plugin/use_theme_colors */
  }
}

@keyframes fadeout-execution-line {
  from {
    background-color: rgb(121 141 254);/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: rgb(171 191 254);/* stylelint-disable-line plugin/use_theme_colors */
  }
}

@keyframes fadeout-execution-line-dark {
  from {
    background-color: #208043;/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: #14522b;/* stylelint-disable-line plugin/use_theme_colors */
  }
}

@keyframes fadeout-execution-line-dark {
  from {
    background-color: #208043;/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: #14522b;/* stylelint-disable-line plugin/use_theme_colors */
  }
}

.CodeMirror-linenumber:hover,
.cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-preserve {
  border-width: 1px 4px 1px 1px;
  padding-right: 3px;
  padding-left: 8px;
  height: 11px;
  line-height: 12px;
  border-style: solid;
  position: relative;
  /* The line number jumps slightly on hover when the minify banner is showing
     if this fractional value is not there. */
  top: -0.15px;
}

.CodeMirror-linenumber:hover {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23ebeced" stroke="%23ebeced"/></svg>') 1 3 1 1;
  padding-left: 8px;
}

.-theme-with-dark-background .CodeMirror-linenumber:hover,
:host-context(.-theme-with-dark-background) .CodeMirror-linenumber:hover {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%233c4043" stroke="%233c4043"/></svg>') 1 3 1 1;
}

.cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color: #fff;

  color: var(--override-auto-gen-cmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%234285f4" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%235186EC" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.cm-breakpoint-disabled .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.breakpoints-deactivated .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointdisabledcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color: #1a73e8;

  color: var(--override-auto-gen-cmbreakpointdisabledcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23d9e7fd" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-disabled .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-with-dark-background .breakpoints-deactivated .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-disabled .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .breakpoints-deactivated .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  color: #1a73e8;
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%232a384e" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23f29900" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23e9a33a" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.cm-breakpoint-disabled.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.breakpoints-deactivated .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointdisabledcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-color: #e37400;

  color: var(--override-auto-gen-cmbreakpointdisabledcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23fcebcc" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-disabled.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-with-dark-background .breakpoints-deactivated .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-disabled.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .breakpoints-deactivated .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  color: #e37400;
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%234d3c1d" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23f439a0" stroke="%23d01884"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23E54D9B" stroke="%23d01884"/></svg>') 1 3 1 1;
}

.cm-breakpoint-disabled.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.breakpoints-deactivated .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointdisabledcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-color: #d01884;

  color: var(--override-auto-gen-cmbreakpointdisabledcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23fdd7ec" stroke="%23f439a0"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-disabled.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-with-dark-background .breakpoints-deactivated .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-disabled.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .breakpoints-deactivated .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  color: #d01884;
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%234e283d" stroke="%23f439a0"/></svg>') 1 3 1 1;
}

.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber::before,
.-theme-preserve {
  content: "?";
  position: absolute;
  top: 0;
  left: 1px;
}

.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber::before,
.-theme-preserve {
  content: "‥";
  position: absolute;
  top: -3px;
  left: 1px;
}

.cm-inline-breakpoint {
  cursor: pointer;
  position: relative;
  top: 1px;
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%234285F4" stroke="%231A73E8"/></svg>');
  height: 10px;
}

.-theme-with-dark-background .cm-inline-breakpoint,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%235186EC" stroke="%231A73E8"/></svg>');
}

.cm-inline-breakpoint.cm-inline-disabled,
.breakpoints-deactivated .cm-inline-breakpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%234285F4" fill-opacity="0.2" stroke="%231A73E8"/></svg>');
}

.cm-inline-breakpoint.cm-inline-breakpoint-conditional {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.75489 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.75489 11.2583 6.29382 11.5 5.80138 11.5H0.5V0.5Z" fill="%23F29900" stroke="%23E37400"/><path d="M3.51074 7.75635H4.68408V9H3.51074V7.75635ZM4.68408 7.23779H3.51074V6.56104C3.51074 6.271 3.55615 6.02344 3.64697 5.81836C3.73779 5.61328 3.90039 5.39648 4.13477 5.16797L4.53027 4.77686C4.71484 4.59814 4.83936 4.4502 4.90381 4.33301C4.97119 4.21582 5.00488 4.09424 5.00488 3.96826C5.00488 3.77197 4.9375 3.62402 4.80273 3.52441C4.66797 3.4248 4.46582 3.375 4.19629 3.375C3.9502 3.375 3.69238 3.42773 3.42285 3.5332C3.15625 3.63574 2.88232 3.78955 2.60107 3.99463V2.81689C2.88818 2.65283 3.17822 2.52979 3.47119 2.44775C3.76709 2.36279 4.06299 2.32031 4.35889 2.32031C4.95068 2.32031 5.41504 2.45801 5.75195 2.7334C6.08887 3.00879 6.25732 3.38818 6.25732 3.87158C6.25732 4.09424 6.20752 4.30225 6.10791 4.49561C6.0083 4.68604 5.8208 4.91602 5.54541 5.18555L5.15869 5.56348C4.95947 5.75684 4.83203 5.91504 4.77637 6.03809C4.7207 6.16113 4.69287 6.31201 4.69287 6.49072C4.69287 6.51709 4.69141 6.54785 4.68848 6.58301C4.68848 6.61816 4.68701 6.65625 4.68408 6.69727V7.23779Z" fill="white"/></svg>');
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-inline-breakpoint-conditional,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-inline-breakpoint-conditional {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.75489 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.75489 11.2583 6.29382 11.5 5.80138 11.5H0.5V0.5Z" fill="%23e9a33a" stroke="%23E37400"/><path d="M3.51074 7.75635H4.68408V9H3.51074V7.75635ZM4.68408 7.23779H3.51074V6.56104C3.51074 6.271 3.55615 6.02344 3.64697 5.81836C3.73779 5.61328 3.90039 5.39648 4.13477 5.16797L4.53027 4.77686C4.71484 4.59814 4.83936 4.4502 4.90381 4.33301C4.97119 4.21582 5.00488 4.09424 5.00488 3.96826C5.00488 3.77197 4.9375 3.62402 4.80273 3.52441C4.66797 3.4248 4.46582 3.375 4.19629 3.375C3.9502 3.375 3.69238 3.42773 3.42285 3.5332C3.15625 3.63574 2.88232 3.78955 2.60107 3.99463V2.81689C2.88818 2.65283 3.17822 2.52979 3.47119 2.44775C3.76709 2.36279 4.06299 2.32031 4.35889 2.32031C4.95068 2.32031 5.41504 2.45801 5.75195 2.7334C6.08887 3.00879 6.25732 3.38818 6.25732 3.87158C6.25732 4.09424 6.20752 4.30225 6.10791 4.49561C6.0083 4.68604 5.8208 4.91602 5.54541 5.18555L5.15869 5.56348C4.95947 5.75684 4.83203 5.91504 4.77637 6.03809C4.7207 6.16113 4.69287 6.31201 4.69287 6.49072C4.69287 6.51709 4.69141 6.54785 4.68848 6.58301C4.68848 6.61816 4.68701 6.65625 4.68408 6.69727V7.23779Z" fill="white"/></svg>');
}

.cm-inline-breakpoint.cm-inline-breakpoint-conditional.cm-inline-disabled,
.breakpoints-deactivated .cm-inline-breakpoint.cm-inline-breakpoint-conditional {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.75489 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.75489 11.2583 6.29382 11.5 5.80138 11.5H0.5V0.5Z" fill="%23F9AB00" fill-opacity="0.2" stroke="%23E37400"/><path d="M3.51074 7.75635H4.68408V9H3.51074V7.75635ZM4.68408 7.23779H3.51074V6.56104C3.51074 6.271 3.55615 6.02344 3.64697 5.81836C3.73779 5.61328 3.90039 5.39648 4.13477 5.16797L4.53027 4.77686C4.71484 4.59814 4.83936 4.4502 4.90381 4.33301C4.97119 4.21582 5.00488 4.09424 5.00488 3.96826C5.00488 3.77197 4.9375 3.62402 4.80273 3.52441C4.66797 3.4248 4.46582 3.375 4.19629 3.375C3.9502 3.375 3.69238 3.42773 3.42285 3.5332C3.15625 3.63574 2.88232 3.78955 2.60107 3.99463V2.81689C2.88818 2.65283 3.17822 2.52979 3.47119 2.44775C3.76709 2.36279 4.06299 2.32031 4.35889 2.32031C4.95068 2.32031 5.41504 2.45801 5.75195 2.7334C6.08887 3.00879 6.25732 3.38818 6.25732 3.87158C6.25732 4.09424 6.20752 4.30225 6.10791 4.49561C6.0083 4.68604 5.8208 4.91602 5.54541 5.18555L5.15869 5.56348C4.95947 5.75684 4.83203 5.91504 4.77637 6.03809C4.7207 6.16113 4.69287 6.31201 4.69287 6.49072C4.69287 6.51709 4.69141 6.54785 4.68848 6.58301C4.68848 6.61816 4.68701 6.65625 4.68408 6.69727V7.23779Z" fill="%23E37400"/></svg>');
}

.cm-inline-breakpoint.cm-inline-logpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%23F439A0" stroke="%23D01884"/><circle cx="3" cy="6" r="1" fill="white"/><circle cx="7" cy="6" r="1" fill="white"/></svg>');
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-inline-logpoint,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-inline-logpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%23E54D9B" stroke="%23D01884"/><circle cx="3" cy="6" r="1" fill="white"/><circle cx="7" cy="6" r="1" fill="white"/></svg>');
}

.cm-inline-breakpoint.cm-inline-logpoint.cm-inline-disabled,
.breakpoints-deactivated .cm-inline-breakpoint.cm-inline-logpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%23F439A0" fill-opacity="0.2" stroke="%23D01884"/><circle cx="3" cy="6" r="1" fill="%23D01884"/><circle cx="7" cy="6" r="1" fill="%23D01884"/></svg>');
}

.cm-execution-line-tail + .CodeMirror-widget {
  --override-auto-gen-cmexecutionlinetailcodemirrorwidget-backgroundcolor: #abbffe;

  background-color: var(--override-auto-gen-cmexecutionlinetailcodemirrorwidget-backgroundcolor);
}

.-theme-with-dark-background .cm-execution-line-tail + .CodeMirror-widget,
:host-context(.-theme-with-dark-background) .cm-execution-line-tail + .CodeMirror-widget {
  --override-auto-gen-cmexecutionlinetailcodemirrorwidget-backgroundcolor: rgb(1 21 84);
}

.source-frame-eval-expression + .CodeMirror-widget {
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-backgroundcolor: rgb(255 255 194);
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-border: rgb(163 41 34);

  border: 1px solid var(--override-auto-gen-sourceframeevalexpressioncodemirrorwidget-border);
  border-left-width: 0;
  border-right-width: 0;
  background-color: var(--override-auto-gen-sourceframeevalexpressioncodemirrorwidget-backgroundcolor);
}

.-theme-with-dark-background .source-frame-eval-expression + .CodeMirror-widget,
:host-context(.-theme-with-dark-background) .source-frame-eval-expression + .CodeMirror-widget {
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-border: rgb(221 99 92);
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-backgroundcolor: rgb(61 61 0);
}

.cm-inline-breakpoint.cm-execution-line-tail {
  --override-auto-gen-cminlinebreakpointcmexecutionlinetail-backgroundcolor: #698cfe;

  background-color: var(--override-auto-gen-cminlinebreakpointcmexecutionlinetail-backgroundcolor);
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-execution-line-tail,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-execution-line-tail {
  --override-auto-gen-cminlinebreakpointcmexecutionlinetail-backgroundcolor: rgb(1 36 150);
}

.cm-execution-line-tail .cm-inline-breakpoint {
  background-color: var(--color-background);
}

.cm-inline-breakpoint.cm-inline-conditional {
  --override-auto-gen-cminlinebreakpointcminlineconditional-backgroundcolor: #ef9d0d;

  background-color: var(--override-auto-gen-cminlinebreakpointcminlineconditional-backgroundcolor);
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-inline-conditional,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-inline-conditional {
  --override-auto-gen-cminlinebreakpointcminlineconditional-backgroundcolor: rgb(242 160 16);
}

.cm-continue-to-location {
  cursor: pointer;
  opacity: 80%;
  position: relative;
  top: 2px;
}

.cm-continue-to-location:hover {
  opacity: 100%;
}

div.CodeMirror:focus-within span.CodeMirror-matchingbracket {
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-borderbottom: rgb(0 0 0 / 50%);
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-backgroundcolor: rgb(0 0 0 / 7%);

  background-color: var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-backgroundcolor);
  border-bottom: 1px solid var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-borderbottom);
}

div.CodeMirror:focus-within span.CodeMirror-nonmatchingbracket {
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-borderbottom: rgb(255 0 0 / 50%);
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-backgroundcolor: rgb(255 0 0 / 7%);

  background-color: var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-backgroundcolor);
  border-bottom: 1px solid var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-borderbottom);
}

.-theme-with-dark-background div.CodeMirror:focus-within span.CodeMirror-matchingbracket,
:host-context(.-theme-with-dark-background) div.CodeMirror:focus-within span.CodeMirror-matchingbracket {
  border-bottom: 1px solid rgb(217 217 217);
  background-color: initial;
}

.-theme-with-dark-background div.CodeMirror:focus-within span.CodeMirror-nonmatchingbracket,
:host-context(.-theme-with-dark-background) div.CodeMirror:focus-within span.CodeMirror-nonmatchingbracket {
  border-bottom: 1px solid rgb(255 26 26);
  background-color: initial;
}

.cm-whitespace::before {
  --override-auto-gen-cmwhitespacebefore-color: rgb(175 175 175);

  position: absolute;
  pointer-events: none;
  color: var(--override-auto-gen-cmwhitespacebefore-color);
}

.-theme-with-dark-background .cm-whitespace::before,
:host-context(.-theme-with-dark-background) .cm-whitespace::before {
  --override-auto-gen-cmwhitespacebefore-color: rgb(80 80 80);
}

.cm-tab {
  display: inline-block;
  text-decoration: inherit;
  position: relative;
}

.cm-tab::before {
  --override-auto-gen-cmtabbefore-borderbottom: rgb(175 175 175);

  display: none;
  content: ".";
  color: transparent;
  border-bottom: 1px solid var(--override-auto-gen-cmtabbefore-borderbottom);
  position: absolute;
  width: 90%;
  bottom: 50%;
  left: 5%;
}

.-theme-with-dark-background .cm-tab::before,
:host-context(.-theme-with-dark-background) .cm-tab::before {
  --override-auto-gen-cmtabbefore-borderbottom: rgb(80 80 80);
}

.show-whitespaces .CodeMirror .cm-tab::before {
  display: block !important; /* stylelint-disable-line declaration-no-important */
}

.cm-execution-line {
  --override-auto-gen-cmexecutionline-backgroundcolor: rgb(0 59 255 / 10%);

  background-color: var(--override-auto-gen-cmexecutionline-backgroundcolor);
}

.cm-execution-line-outline {
  --override-auto-gen-cmexecutionlineoutline-outline: rgb(64 115 244);

  outline: 1px solid var(--override-auto-gen-cmexecutionlineoutline-outline);
}

.cm-execution-line-tail {
  --override-auto-gen-cmexecutionlinetail-backgroundcolor: rgb(171 191 254);

  background-color: var(--override-auto-gen-cmexecutionlinetail-backgroundcolor);
}

.-theme-with-dark-background .cm-execution-line,
:host-context(.-theme-with-dark-background) .cm-execution-line {
  background-color: #14522b;
}

.-theme-with-dark-background .cm-execution-line-outline,
:host-context(.-theme-with-dark-background) .cm-execution-line-outline {
  outline: 1px solid #33cc6b;
}

.-theme-with-dark-background .cm-execution-line-tail,
:host-context(.-theme-with-dark-background) .cm-execution-line-tail {
  background-color: #347132;
}

.cm-token-highlight {
  position: relative;
}

.cm-token-highlight::before {
  position: absolute;
  border: 1px solid var(--override-search-highlight-border-color);
  border-radius: 3px;
  top: 0;
  bottom: -1px;
  left: 0;
  right: 0;
  content: "";
}

.cm-line-with-selection .cm-column-with-selection::before {
  border: none;
}

.cm-search-highlight {
  position: relative;
}

.cm-search-highlight::before {
  position: absolute;
  border-top-style: solid;
  border-bottom-style: solid;
  border-top-color: var(--override-search-highlight-border-color);
  border-bottom-color: var(--override-search-highlight-border-color);
  border-top-width: 1px;
  border-bottom-width: 1px;
  top: -1px;
  bottom: 0;
  left: 0;
  right: 0;
  content: "";
}

.cm-search-highlight-full::before {
  border: 1px solid var(--override-search-highlight-border-color);
  border-radius: 3px;
}

.cm-search-highlight-start::before {
  border-left-width: 1px;
  border-top-left-radius: 2px;
  border-bottom-left-radius: 2px;
  border-left-style: solid;
  border-left-color: var(--override-search-highlight-border-color);
}

.cm-search-highlight-end::before {
  border-right-width: 1px;
  border-top-right-radius: 2px;
  border-bottom-right-radius: 2px;
  border-right-style: solid;
  border-right-color: var(--override-search-highlight-border-color);
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight-full::before {
  border-radius: 1px;
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight-start::before {
  border-top-left-radius: 1px;
  border-bottom-left-radius: 1px;
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight-end::before {
  border-top-right-radius: 1px;
  border-bottom-right-radius: 1px;
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight::before {
  --override-auto-gen-cmlinewithselectioncmcolumnwithselectioncmsearchhighlightbefore-backgroundcolor: rgb(241 234 0);

  margin: -1px -1px -1px -1px;
  background-color: var(--override-auto-gen-cmlinewithselectioncmcolumnwithselectioncmsearchhighlightbefore-backgroundcolor);
  z-index: -1;
}

.-theme-with-dark-background .cm-line-with-selection .cm-column-with-selection.cm-search-highlight::before,
:host-context(.-theme-with-dark-background) .cm-line-with-selection .cm-column-with-selection.cm-search-highlight::before {
  background-color: hsl(133deg 100% 30%);
}

.-theme-with-dark-background .cm-line-with-selection .cm-search-highlight,
:host-context(.-theme-with-dark-background) .cm-line-with-selection .cm-search-highlight {
  color: #eee;
}

.CodeMirror .text-editor-line-marker-text {
  text-align: right;
  padding-right: 3px;
  height: 12px;
}

.CodeMirror .text-editor-line-marker-text span.line-marker-units {
  color: var(--color-text-secondary);
  font-size: 75%;
  margin-left: 3px;
}

.CodeMirror .text-editor-coverage-unused-marker {
  text-align: right;
  padding-right: 2px;
  background-color: var(--color-accent-red);
}

.CodeMirror .text-editor-coverage-unused-marker::after {
  content: "\200B";
}

.CodeMirror .text-editor-coverage-used-marker {
  --override-auto-gen-codemirrortexteditorcoverageusedmarker-backgroundcolor: #63acbe;

  text-align: right;
  padding-right: 2px;
  background-color: var(--override-auto-gen-codemirrortexteditorcoverageusedmarker-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .text-editor-coverage-used-marker,
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-coverage-used-marker {
  --override-auto-gen-codemirrortexteditorcoverageusedmarker-backgroundcolor: rgb(65 138 156);
}

.CodeMirror .text-editor-coverage-used-marker::after {
  content: "\200B";
}

.CodeMirror .text-editor-line-decoration {
  position: absolute;
}

.CodeMirror .text-editor-line-decoration-wave {
  position: absolute;
  top: -2px;
  right: -4px;
  left: 4px;
  cursor: pointer;
  height: 4px;
  background-image: var(--image-file-errorWave);
  background-repeat: repeat-x;
  background-size: contain;
}

.CodeMirror .text-editor-value-decoration {
  --override-auto-gen-codemirrortexteditorvaluedecoration-backgroundcolor: #ffe3c7;

  position: absolute;
  bottom: 0;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  max-width: 1000px;
  opacity: 80%;
  background-color: var(--override-auto-gen-codemirrortexteditorvaluedecoration-backgroundcolor);
  margin-left: 10px;
  padding-left: 5px;
  color: var(--color-text-primary);
  user-select: text;
}

.-theme-with-dark-background .CodeMirror .text-editor-value-decoration,
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-value-decoration {
  --override-auto-gen-codemirrortexteditorvaluedecoration-backgroundcolor: rgb(56 28 0);
}

.CodeMirror .cm-execution-line .text-editor-value-decoration {
  background-color: transparent;
  opacity: 50%;
}

.CodeMirror .text-editor-line-decoration-icon {
  cursor: pointer;
}

.CodeMirror .text-editor-line-decoration-icon > * {
  vertical-align: text-bottom;
  margin-left: 2px;
}

.CodeMirror .text-editor-line-decoration-icon-issue {
  cursor: pointer;
}

.CodeMirror .text-editor-line-with-warning:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewithwarningnotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(241 230 0 / 10%);

  background-color: var(--override-auto-gen-codemirrortexteditorlinewithwarningnotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .text-editor-line-with-warning:not(.cm-execution-line):not(.cm-readonly-highlight),
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-line-with-warning:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewithwarningnotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(255 244 14 / 10%);
}

.CodeMirror .text-editor-line-with-error:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewitherrornotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(255 0 0 / 5%);

  background-color: var(--override-auto-gen-codemirrortexteditorlinewitherrornotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .text-editor-line-with-error:not(.cm-execution-line):not(.cm-readonly-highlight),
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-line-with-error:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewitherrornotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(255 0 0 / 5%);
}

.CodeMirror .CodeMirror-vscrollbar,
.CodeMirror .CodeMirror-hscrollbar {
  transform: translateZ(0);
}

.cm-trailing-whitespace {
  --override-auto-gen-cmtrailingwhitespace-backgroundcolor: rgb(255 0 0 / 5%);

  background-color: var(--override-auto-gen-cmtrailingwhitespace-backgroundcolor);
}

.-theme-with-dark-background .cm-trailing-whitespace,
:host-context(.-theme-with-dark-background) .cm-trailing-whitespace {
  --override-auto-gen-cmtrailingwhitespace-backgroundcolor: rgb(255 0 0 / 5%);
}

.CodeMirror-activeline .cm-trailing-whitespace {
  background-color: transparent;
}

.CodeMirror .CodeMirror-selected {
  background-color: var(--legacy-item-selection-inactive-bg-color);
}

.CodeMirror-focused .CodeMirror-selected {
  background-color: var(--legacy-item-selection-bg-color);
}

.-theme-with-dark-background .CodeMirror .CodeMirror-selected,
:host-context(.-theme-with-dark-background) .CodeMirror .CodeMirror-selected {
  background-color: #454545;
}

.-theme-with-dark-background span.CodeMirror-selectedtext,
:host-context(.-theme-with-dark-background) span.CodeMirror-selectedtext {
  background-color: #454545;
}

.CodeMirror .auto-complete-text {
  color: var(--color-text-secondary);
}

.CodeMirror .placeholder-text {
  height: 0;
  color: var(--color-text-secondary);
}

.CodeMirror textarea {
  resize: none;
  overflow: hidden;
}

.CodeMirror-lines {
  padding: 4px 0; /* Vertical padding around content */
}

.CodeMirror pre {
  padding: 0 4px; /* Horizontal padding of content */
}

.CodeMirror-scrollbar-filler,
.CodeMirror-gutter-filler {
  /* The little square between H and V scrollbars */
  background-color: var(--color-background);
}

.CodeMirror div.CodeMirror-secondarycursor {
  --override-auto-gen-codemirrordivcodemirrorsecondarycursor-borderleft: #c0c0c0;

  border-left: 1px solid var(--override-auto-gen-codemirrordivcodemirrorsecondarycursor-borderleft);
}

.-theme-with-dark-background .CodeMirror div.CodeMirror-secondarycursor,
:host-context(.-theme-with-dark-background) .CodeMirror div.CodeMirror-secondarycursor {
  --override-auto-gen-codemirrordivcodemirrorsecondarycursor-borderleft: rgb(63 63 63);
}

.CodeMirror-composing {
  border-bottom: 2px solid;
}

.CodeMirror-foldmarker {
  cursor: pointer;
  font-size: 0;
  line-height: 0;
  height: 0;
}

.CodeMirror-foldmarker::before {
  content: '\2026';
  font-size: 13px;
  color: var(--color-text-secondary);
}

.CodeMirror-foldgutter {
  width: 1.5em;
}

.CodeMirror-gutters:hover .CodeMirror-foldgutter {
  background-color: transparent;
}

.CodeMirror-foldgutter-open,
.CodeMirror-foldgutter-folded {
  cursor: pointer;
  position: relative;
}

.CodeMirror-foldgutter-open {
  transition: opacity 0.2s;
  opacity: 0%;
}

.CodeMirror-gutter-hovered .CodeMirror-foldgutter-open {
  opacity: 100%;
}

.CodeMirror-foldgutter-open::before,
.CodeMirror-foldgutter-folded::before {
  background-color: var(--color-text-secondary);
  user-select: none;
  -webkit-mask-image: var(--image-file-treeoutlineTriangles);
  -webkit-mask-size: 32px 24px;
  content: "";
  display: block;
  width: 8px;
  color: transparent;
  text-shadow: none;
  height: 12px;
  position: absolute;
  right: 4px;
}

.CodeMirror-foldgutter-open::before {
  -webkit-mask-position: -16px 0;
}

.CodeMirror-foldgutter-folded::before {
  -webkit-mask-position: 0 0;
}

.CodeMirror .CodeMirror-line::selection,
.CodeMirror .CodeMirror-line > span::selection,
.CodeMirror .CodeMirror-line > span > span::selection {
  background: var(--legacy-item-selection-bg-color);
}

@media (forced-colors: active) {
  .cm-token-highlight::before {
    forced-color-adjust: none;
    border-color: Highlight;
  }
}

/* stylelint-enable no-descending-specificity */

/*# sourceURL=ui/legacy/components/text_editor/cmdevtools.css */x<script type="text/javascript" src="js/__start__.js?v=1.1.213"></script><canvas id="application-canvas" tabindex="0" style="user-select: none; width: 1365px; height: 971px;" width="1365" height="971" class="fill-mode-FILL_WINDOW">/* The rest of this file contains styles related to the mechanics of
   the editor. You probably shouldn't touch them. */

.CodeMirror {
  position: relative;
  overflow: hidden;
  background: var(--color-background);
}

.CodeMirror-scroll {
  overflow: scroll !important; /* Things will break if this is overridden */
  /* 50px is the magic margin used to hide the element's real scrollbars */
  /* See overflow: hidden in .CodeMirror */
  margin-bottom: -50px;
  margin-right: -50px;
  padding-bottom: 50px;
  height: 100%;
  outline: none; /* Prevent dragging from highlighting the element */
  position: relative;
}

.CodeMirror-sizer {
  position: relative;
  border-right: 50px solid transparent;
}

/* The fake, visible scrollbars. Used to force redraw during scrolling
   before actual scrolling happens, thus preventing shaking and
   flickering artifacts. */
.CodeMirror-vscrollbar,
.CodeMirror-hscrollbar,
.CodeMirror-scrollbar-filler,
.CodeMirror-gutter-filler {
  position: absolute;
  z-index: 6;
  display: none;
  outline: none;
}

.CodeMirror-vscrollbar {
  right: 0;
  top: 0;
  overflow-x: hidden;
  overflow-y: scroll;
}

.CodeMirror-hscrollbar {
  bottom: 0;
  left: 0;
  overflow-y: hidden;
  overflow-x: scroll;
}

.CodeMirror-scrollbar-filler {
  right: 0;
  bottom: 0;
}

.CodeMirror-gutter-filler {
  left: 0;
  bottom: 0;
}

.CodeMirror-gutters {
  position: absolute;
  left: 0;
  top: 0;
  min-height: 100%;
  z-index: 3;
}

.CodeMirror-gutter {
  white-space: normal;
  height: 100%;
  display: inline-block;
  vertical-align: top;
  margin-bottom: -50px;
}

.CodeMirror-gutter-wrapper {
  position: absolute;
  z-index: 4;
  background: none !important;
  border: none !important;
}

.CodeMirror-gutter-background {
  position: absolute;
  top: 0;
  bottom: 0;
  z-index: 4;
}

.CodeMirror-gutter-elt {
  position: absolute;
  cursor: default;
  z-index: 4;
}

.CodeMirror-gutter-wrapper ::selection {
  background-color: transparent;
}

.CodeMirror-gutter-wrapper ::-moz-selection {
  background-color: transparent;
}

.CodeMirror-lines {
  cursor: text;
  min-height: 1px; /* prevents collapsing before first draw */
}

.CodeMirror pre.CodeMirror-line,
.CodeMirror pre.CodeMirror-line-like {
  /* Reset some styles that the rest of the page might have set */
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -moz-border-radius: 0;
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -webkit-border-radius: 0;
  border-radius: 0;
  border-width: 0;
  background: transparent;
  font-family: inherit;
  font-size: inherit;
  margin: 0;
  white-space: pre;
  word-wrap: normal;
  line-height: inherit;
  color: inherit;
  z-index: 2;
  position: relative;
  overflow: visible;
  -webkit-tap-highlight-color: transparent;
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -webkit-font-variant-ligatures: contextual;
  font-variant-ligatures: contextual;
}

.CodeMirror-wrap pre.CodeMirror-line,
.CodeMirror-wrap pre.CodeMirror-line-like {
  word-wrap: break-word;
  white-space: pre-wrap;
  word-break: normal;
}

.CodeMirror-linebackground {
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  z-index: 0;
}

.CodeMirror-linewidget {
  position: relative;
  z-index: 2;
  padding: 0.1px; /* Force widget margins to stay inside of the container */
}

.CodeMirror-rtl pre {
  direction: rtl;
}

.CodeMirror-code {
  outline: none;
}

/* Force content-box sizing for the elements where we expect it */
.CodeMirror-scroll,
.CodeMirror-sizer,
.CodeMirror-gutter,
.CodeMirror-gutters,
.CodeMirror-linenumber {
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -moz-box-sizing: content-box;
  box-sizing: content-box;
}

.CodeMirror-measure {
  position: absolute;
  width: 100%;
  height: 0;
  overflow: hidden;
  visibility: hidden;
}

.CodeMirror-cursor {
  position: absolute;
  pointer-events: none;
}

.CodeMirror-measure pre {
  position: static;
}

div.CodeMirror-cursors {
  visibility: hidden;
  position: relative;
  z-index: 3;
}

div.CodeMirror-dragcursors {
  visibility: visible;
}

.CodeMirror-focused div.CodeMirror-cursors {
  visibility: visible;
}

.CodeMirror-selected {
  --override-cm-selected-background-color: #d9d9d9;

  background: var(--override-cm-selected-background-color);
}

.-theme-with-dark-background .CodeMirror-selected,
:host-context(.-theme-with-dark-background) .CodeMirror-selected {
  --override-cm-selected-background-color: rgb(38 38 38);
}

.CodeMirror-focused .CodeMirror-selected {
  --override-cm-selected-background-color: #d7d4f0;
}

.-theme-with-dark-background .CodeMirror-focused .CodeMirror-selected,
:host-context(.-theme-with-dark-background) .CodeMirror-focused .CodeMirror-selected {
  --override-cm-selected-background-color: rgb(18 15 43);
}

.CodeMirror-crosshair {
  cursor: crosshair;
}

.CodeMirror-line {
  --override-line-selection-background-color: #d7d4f0;
}

.CodeMirror-line::selection,
.CodeMirror-line > span::selection,
.CodeMirror-line > span > span::selection {
  background:var(--override-line-selection-background-color);
}

.CodeMirror-line::-moz-selection,
.CodeMirror-line > span::-moz-selection,
.CodeMirror-line > span > span::-moz-selection {
  background: var(--override-line-selection-background-color);
}

.-theme-with-dark-background .CodeMirror-line,
:host-context(.-theme-with-dark-background) .CodeMirror-line {
  --override-line-selection-background-color: rgb(18 15 43);

}

.cm-searching {
  --override-searching-background-color: rgb(255 255 0 / 40%);

  background-color: var(--override-searching-background-color);
}

/* Used to force a border model for a node */
.cm-force-border {
  padding-right: 0.1px;
}

@media print {
  /* Hide the cursor when printing */
  .CodeMirror div.CodeMirror-cursors {
    visibility: hidden;
  }
}

/* See issue #2901 */
.cm-tab-wrap-hack::after {
  content: "";
}

/* Help users use markselection to safely style text background */
span.CodeMirror-selectedtext {
  background: none;
}

/*# sourceURL=third_party/codemirror/codemirror.css *//*
 * Copyright 2021 The Chromium Authors. All rights reserved.
 * Use of this source code is governed by a BSD-style license that can be
 * found in the LICENSE file.
 */

/* stylelint-disable no-descending-specificity */

/**
 * Many of the CSS variables here were auto generated during the dark mode
 * migration. If you are changing them, please feel free to rename them whilst
 * you're here to make them clearer.
 */

.CodeMirror {
  --override-search-highlight-border-color: rgb(128 128 128);

  line-height: 1.2em !important; /* stylelint-disable-line declaration-no-important */
  background-color: transparent !important; /* stylelint-disable-line declaration-no-important */
  color: var(--color-text-primary);
  height: 300px;
}

.CodeMirror-linewidget {
  overflow: visible !important; /* stylelint-disable-line declaration-no-important */
}

.CodeMirror-gutter-performance {
  width: 60px;
  background-color: var(--color-background);
  margin-left: 3px;
}

.CodeMirror-gutter-memory {
  width: 48px;
  background-color: var(--color-background);
  margin-left: 3px;
}

.CodeMirror-gutter-coverage {
  width: 5px;
  background-color: var(--color-background);
  margin-left: 3px;
}

.CodeMirror .source-frame-eval-expression {
  --override-auto-gen-codemirrorsourceframeevalexpression-backgroundcolor: rgb(255 255 194);
  --override-auto-gen-codemirrorsourceframeevalexpression-border: rgb(163 41 34);

  outline: 0;
  border: 1px solid var(--override-auto-gen-codemirrorsourceframeevalexpression-border);
  border-left-width: 0;
  border-right-width: 0;
  background-color: var(--override-auto-gen-codemirrorsourceframeevalexpression-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .source-frame-eval-expression,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-eval-expression {
  --override-auto-gen-codemirrorsourceframeevalexpression-border: rgb(221 99 92);
  --override-auto-gen-codemirrorsourceframeevalexpression-backgroundcolor: rgb(61 61 0);
}

.CodeMirror .source-frame-eval-expression-start {
  border-left-width: 1px;
  margin-left: -1px;
}

.CodeMirror .source-frame-eval-expression-end {
  border-right-width: 1px;
  margin-right: -1px;
}

.CodeMirror .source-frame-continue-to-location {
  --override-auto-gen-codemirrorsourceframecontinuetolocation-backgroundcolor: rgb(230 236 255);

  outline: 0;
  border: 1px solid transparent;
  border-left-width: 0;
  border-right-width: 0;
  background-color: var(--override-auto-gen-codemirrorsourceframecontinuetolocation-backgroundcolor);
  cursor: pointer;
}

.CodeMirror .source-frame-continue-to-location:hover {
  --override-auto-gen-codemirrorsourceframecontinuetolocationhover-backgroundcolor: rgb(171 191 254);
  --override-auto-gen-codemirrorsourceframecontinuetolocationhover-border: rgb(121 141 254);

  border: 1px solid var(--override-auto-gen-codemirrorsourceframecontinuetolocationhover-border);
  background-color: var(--override-auto-gen-codemirrorsourceframecontinuetolocationhover-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .source-frame-continue-to-location,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-continue-to-location {
  background-color: #14522b;
}

.-theme-with-dark-background .CodeMirror .source-frame-continue-to-location:hover,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-continue-to-location:hover {
  border: 1px solid #33cc6b;
  background-color: #14522b;
}

.CodeMirror .source-frame-continue-to-location-start {
  border-left-width: 1px;
  margin-left: -1px;
}

.CodeMirror .source-frame-continue-to-location-end {
  border-right-width: 1px;
  margin-right: -1px;
}

.CodeMirror .source-frame-async-step-in {
  --override-auto-gen-codemirrorsourceframeasyncstepin-backgroundcolor: hsl(100deg 46% 80% / 100%);

  outline: 0;
  background-color: var(--override-auto-gen-codemirrorsourceframeasyncstepin-backgroundcolor);
  cursor: pointer;
  border: 1px solid transparent;
  border-left-width: 0;
  border-right-width: 0;
}

.-theme-with-dark-background .CodeMirror .source-frame-async-step-in,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-async-step-in {
  --override-auto-gen-codemirrorsourceframeasyncstepin-backgroundcolor: rgb(43 74 28);
}

.source-frame-async-step-in-hovered .source-frame-async-step-in {
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-bordercolor: rgb(100 154 100);
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-backgroundcolor: hsl(96deg 53% 65%);

  background-color: var(--override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-backgroundcolor);
  border-color: var(--override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-bordercolor);
}

.-theme-with-dark-background .source-frame-async-step-in-hovered .source-frame-async-step-in,
:host-context(.-theme-with-dark-background) .source-frame-async-step-in-hovered .source-frame-async-step-in {
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-backgroundcolor: rgb(80 137 42);
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-bordercolor: rgb(101 155 101);
}

.source-frame-async-step-in-hovered .source-frame-async-step-in-start {
  border-left-width: 1px;
  margin-left: -1px;
}

.source-frame-async-step-in-hovered .source-frame-async-step-in-end {
  border-right-width: 1px;
  margin-right: -1px;
}

.CodeMirror-cursor {
  border-left: 1px solid var(--color-background-inverted);
  border-right: none;
  width: 0;
}

.CodeMirror-readonly .CodeMirror-cursor {
  display: none;
}

.CodeMirror-gutters {
  border-right: 1px solid var(--color-details-hairline);
  white-space: nowrap;
  background-color: var(--color-background);
}

.CodeMirror-linenumber {
  --override-auto-gen-codemirrorlinenumber-color: hsl(0deg 0% 46%);

  color: var(--override-auto-gen-codemirrorlinenumber-color);
  padding: 0 3px 0 9px;
  min-width: 28px;
  text-align: right;
  white-space: nowrap;
}

.-theme-with-dark-background .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .CodeMirror-linenumber {
  --override-auto-gen-codemirrorlinenumber-color: rgb(138 138 138);
}

.pretty-printed .CodeMirror-linenumber {
  color: var(--legacy-accent-color);
}

.cm-non-breakable-line .CodeMirror-linenumber {
  --override-auto-gen-cmnonbreakablelinecodemirrorlinenumber-color: rgb(128 128 128 / 40%);

  color: var(--override-auto-gen-cmnonbreakablelinecodemirrorlinenumber-color);
}

.-theme-with-dark-background .cm-non-breakable-line .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-non-breakable-line .CodeMirror-linenumber {
  --override-auto-gen-cmnonbreakablelinecodemirrorlinenumber-color: rgb(127 127 127 / 40%);
}

.cm-highlight {
  animation: fadeout 2s 0s;
}

.-theme-with-dark-background .cm-highlight,
:host-context(.-theme-with-dark-background) .cm-highlight {
  animation: fadeout-dark 2s 0s;
}

@keyframes fadeout {
  from {
    background-color: rgb(255 255 120); /* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: var(--color-background); }
}

@keyframes fadeout {
  from {
    background-color: rgb(255 255 120); /* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: var(--color-background); }
}

@keyframes fadeout-dark {
  from {
    background-color: hsl(133deg 100% 30% / 50%);/* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: transparent; }
}

@keyframes fadeout-dark {
  from {
    background-color: hsl(133deg 100% 30% / 50%);/* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: transparent; }
}

.cm-readonly-highlight {
  --override-auto-gen-cmreadonlyhighlight-backgroundcolor: rgb(255 255 120);

  background-color: var(--override-auto-gen-cmreadonlyhighlight-backgroundcolor);
}

.-theme-with-dark-background .cm-readonly-highlight,
:host-context(.-theme-with-dark-background) .cm-readonly-highlight {
  background-color: hsl(133deg 100% 30% / 50%);
}

.cm-highlight.cm-execution-line {
  animation: fadeout-execution-line 1s 0s;
}

.-theme-with-dark-background .cm-highlight.cm-execution-line,
:host-context(.-theme-with-dark-background) .cm-highlight.cm-execution-line {
  animation: fadeout-execution-line-dark 1s 0s;
}

@keyframes fadeout-execution-line {
  from {
    background-color: rgb(121 141 254);/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: rgb(171 191 254);/* stylelint-disable-line plugin/use_theme_colors */
  }
}

@keyframes fadeout-execution-line {
  from {
    background-color: rgb(121 141 254);/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: rgb(171 191 254);/* stylelint-disable-line plugin/use_theme_colors */
  }
}

@keyframes fadeout-execution-line-dark {
  from {
    background-color: #208043;/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: #14522b;/* stylelint-disable-line plugin/use_theme_colors */
  }
}

@keyframes fadeout-execution-line-dark {
  from {
    background-color: #208043;/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: #14522b;/* stylelint-disable-line plugin/use_theme_colors */
  }
}

.CodeMirror-linenumber:hover,
.cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-preserve {
  border-width: 1px 4px 1px 1px;
  padding-right: 3px;
  padding-left: 8px;
  height: 11px;
  line-height: 12px;
  border-style: solid;
  position: relative;
  /* The line number jumps slightly on hover when the minify banner is showing
     if this fractional value is not there. */
  top: -0.15px;
}

.CodeMirror-linenumber:hover {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23ebeced" stroke="%23ebeced"/></svg>') 1 3 1 1;
  padding-left: 8px;
}

.-theme-with-dark-background .CodeMirror-linenumber:hover,
:host-context(.-theme-with-dark-background) .CodeMirror-linenumber:hover {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%233c4043" stroke="%233c4043"/></svg>') 1 3 1 1;
}

.cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color: #fff;

  color: var(--override-auto-gen-cmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%234285f4" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%235186EC" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.cm-breakpoint-disabled .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.breakpoints-deactivated .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointdisabledcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color: #1a73e8;

  color: var(--override-auto-gen-cmbreakpointdisabledcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23d9e7fd" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-disabled .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-with-dark-background .breakpoints-deactivated .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-disabled .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .breakpoints-deactivated .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  color: #1a73e8;
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%232a384e" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23f29900" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23e9a33a" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.cm-breakpoint-disabled.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.breakpoints-deactivated .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointdisabledcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-color: #e37400;

  color: var(--override-auto-gen-cmbreakpointdisabledcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23fcebcc" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-disabled.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-with-dark-background .breakpoints-deactivated .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-disabled.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .breakpoints-deactivated .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  color: #e37400;
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%234d3c1d" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23f439a0" stroke="%23d01884"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23E54D9B" stroke="%23d01884"/></svg>') 1 3 1 1;
}

.cm-breakpoint-disabled.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.breakpoints-deactivated .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointdisabledcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-color: #d01884;

  color: var(--override-auto-gen-cmbreakpointdisabledcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23fdd7ec" stroke="%23f439a0"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-disabled.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-with-dark-background .breakpoints-deactivated .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-disabled.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .breakpoints-deactivated .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  color: #d01884;
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%234e283d" stroke="%23f439a0"/></svg>') 1 3 1 1;
}

.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber::before,
.-theme-preserve {
  content: "?";
  position: absolute;
  top: 0;
  left: 1px;
}

.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber::before,
.-theme-preserve {
  content: "‥";
  position: absolute;
  top: -3px;
  left: 1px;
}

.cm-inline-breakpoint {
  cursor: pointer;
  position: relative;
  top: 1px;
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%234285F4" stroke="%231A73E8"/></svg>');
  height: 10px;
}

.-theme-with-dark-background .cm-inline-breakpoint,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%235186EC" stroke="%231A73E8"/></svg>');
}

.cm-inline-breakpoint.cm-inline-disabled,
.breakpoints-deactivated .cm-inline-breakpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%234285F4" fill-opacity="0.2" stroke="%231A73E8"/></svg>');
}

.cm-inline-breakpoint.cm-inline-breakpoint-conditional {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.75489 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.75489 11.2583 6.29382 11.5 5.80138 11.5H0.5V0.5Z" fill="%23F29900" stroke="%23E37400"/><path d="M3.51074 7.75635H4.68408V9H3.51074V7.75635ZM4.68408 7.23779H3.51074V6.56104C3.51074 6.271 3.55615 6.02344 3.64697 5.81836C3.73779 5.61328 3.90039 5.39648 4.13477 5.16797L4.53027 4.77686C4.71484 4.59814 4.83936 4.4502 4.90381 4.33301C4.97119 4.21582 5.00488 4.09424 5.00488 3.96826C5.00488 3.77197 4.9375 3.62402 4.80273 3.52441C4.66797 3.4248 4.46582 3.375 4.19629 3.375C3.9502 3.375 3.69238 3.42773 3.42285 3.5332C3.15625 3.63574 2.88232 3.78955 2.60107 3.99463V2.81689C2.88818 2.65283 3.17822 2.52979 3.47119 2.44775C3.76709 2.36279 4.06299 2.32031 4.35889 2.32031C4.95068 2.32031 5.41504 2.45801 5.75195 2.7334C6.08887 3.00879 6.25732 3.38818 6.25732 3.87158C6.25732 4.09424 6.20752 4.30225 6.10791 4.49561C6.0083 4.68604 5.8208 4.91602 5.54541 5.18555L5.15869 5.56348C4.95947 5.75684 4.83203 5.91504 4.77637 6.03809C4.7207 6.16113 4.69287 6.31201 4.69287 6.49072C4.69287 6.51709 4.69141 6.54785 4.68848 6.58301C4.68848 6.61816 4.68701 6.65625 4.68408 6.69727V7.23779Z" fill="white"/></svg>');
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-inline-breakpoint-conditional,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-inline-breakpoint-conditional {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.75489 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.75489 11.2583 6.29382 11.5 5.80138 11.5H0.5V0.5Z" fill="%23e9a33a" stroke="%23E37400"/><path d="M3.51074 7.75635H4.68408V9H3.51074V7.75635ZM4.68408 7.23779H3.51074V6.56104C3.51074 6.271 3.55615 6.02344 3.64697 5.81836C3.73779 5.61328 3.90039 5.39648 4.13477 5.16797L4.53027 4.77686C4.71484 4.59814 4.83936 4.4502 4.90381 4.33301C4.97119 4.21582 5.00488 4.09424 5.00488 3.96826C5.00488 3.77197 4.9375 3.62402 4.80273 3.52441C4.66797 3.4248 4.46582 3.375 4.19629 3.375C3.9502 3.375 3.69238 3.42773 3.42285 3.5332C3.15625 3.63574 2.88232 3.78955 2.60107 3.99463V2.81689C2.88818 2.65283 3.17822 2.52979 3.47119 2.44775C3.76709 2.36279 4.06299 2.32031 4.35889 2.32031C4.95068 2.32031 5.41504 2.45801 5.75195 2.7334C6.08887 3.00879 6.25732 3.38818 6.25732 3.87158C6.25732 4.09424 6.20752 4.30225 6.10791 4.49561C6.0083 4.68604 5.8208 4.91602 5.54541 5.18555L5.15869 5.56348C4.95947 5.75684 4.83203 5.91504 4.77637 6.03809C4.7207 6.16113 4.69287 6.31201 4.69287 6.49072C4.69287 6.51709 4.69141 6.54785 4.68848 6.58301C4.68848 6.61816 4.68701 6.65625 4.68408 6.69727V7.23779Z" fill="white"/></svg>');
}

.cm-inline-breakpoint.cm-inline-breakpoint-conditional.cm-inline-disabled,
.breakpoints-deactivated .cm-inline-breakpoint.cm-inline-breakpoint-conditional {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.75489 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.75489 11.2583 6.29382 11.5 5.80138 11.5H0.5V0.5Z" fill="%23F9AB00" fill-opacity="0.2" stroke="%23E37400"/><path d="M3.51074 7.75635H4.68408V9H3.51074V7.75635ZM4.68408 7.23779H3.51074V6.56104C3.51074 6.271 3.55615 6.02344 3.64697 5.81836C3.73779 5.61328 3.90039 5.39648 4.13477 5.16797L4.53027 4.77686C4.71484 4.59814 4.83936 4.4502 4.90381 4.33301C4.97119 4.21582 5.00488 4.09424 5.00488 3.96826C5.00488 3.77197 4.9375 3.62402 4.80273 3.52441C4.66797 3.4248 4.46582 3.375 4.19629 3.375C3.9502 3.375 3.69238 3.42773 3.42285 3.5332C3.15625 3.63574 2.88232 3.78955 2.60107 3.99463V2.81689C2.88818 2.65283 3.17822 2.52979 3.47119 2.44775C3.76709 2.36279 4.06299 2.32031 4.35889 2.32031C4.95068 2.32031 5.41504 2.45801 5.75195 2.7334C6.08887 3.00879 6.25732 3.38818 6.25732 3.87158C6.25732 4.09424 6.20752 4.30225 6.10791 4.49561C6.0083 4.68604 5.8208 4.91602 5.54541 5.18555L5.15869 5.56348C4.95947 5.75684 4.83203 5.91504 4.77637 6.03809C4.7207 6.16113 4.69287 6.31201 4.69287 6.49072C4.69287 6.51709 4.69141 6.54785 4.68848 6.58301C4.68848 6.61816 4.68701 6.65625 4.68408 6.69727V7.23779Z" fill="%23E37400"/></svg>');
}

.cm-inline-breakpoint.cm-inline-logpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%23F439A0" stroke="%23D01884"/><circle cx="3" cy="6" r="1" fill="white"/><circle cx="7" cy="6" r="1" fill="white"/></svg>');
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-inline-logpoint,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-inline-logpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%23E54D9B" stroke="%23D01884"/><circle cx="3" cy="6" r="1" fill="white"/><circle cx="7" cy="6" r="1" fill="white"/></svg>');
}

.cm-inline-breakpoint.cm-inline-logpoint.cm-inline-disabled,
.breakpoints-deactivated .cm-inline-breakpoint.cm-inline-logpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%23F439A0" fill-opacity="0.2" stroke="%23D01884"/><circle cx="3" cy="6" r="1" fill="%23D01884"/><circle cx="7" cy="6" r="1" fill="%23D01884"/></svg>');
}

.cm-execution-line-tail + .CodeMirror-widget {
  --override-auto-gen-cmexecutionlinetailcodemirrorwidget-backgroundcolor: #abbffe;

  background-color: var(--override-auto-gen-cmexecutionlinetailcodemirrorwidget-backgroundcolor);
}

.-theme-with-dark-background .cm-execution-line-tail + .CodeMirror-widget,
:host-context(.-theme-with-dark-background) .cm-execution-line-tail + .CodeMirror-widget {
  --override-auto-gen-cmexecutionlinetailcodemirrorwidget-backgroundcolor: rgb(1 21 84);
}

.source-frame-eval-expression + .CodeMirror-widget {
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-backgroundcolor: rgb(255 255 194);
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-border: rgb(163 41 34);

  border: 1px solid var(--override-auto-gen-sourceframeevalexpressioncodemirrorwidget-border);
  border-left-width: 0;
  border-right-width: 0;
  background-color: var(--override-auto-gen-sourceframeevalexpressioncodemirrorwidget-backgroundcolor);
}

.-theme-with-dark-background .source-frame-eval-expression + .CodeMirror-widget,
:host-context(.-theme-with-dark-background) .source-frame-eval-expression + .CodeMirror-widget {
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-border: rgb(221 99 92);
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-backgroundcolor: rgb(61 61 0);
}

.cm-inline-breakpoint.cm-execution-line-tail {
  --override-auto-gen-cminlinebreakpointcmexecutionlinetail-backgroundcolor: #698cfe;

  background-color: var(--override-auto-gen-cminlinebreakpointcmexecutionlinetail-backgroundcolor);
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-execution-line-tail,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-execution-line-tail {
  --override-auto-gen-cminlinebreakpointcmexecutionlinetail-backgroundcolor: rgb(1 36 150);
}

.cm-execution-line-tail .cm-inline-breakpoint {
  background-color: var(--color-background);
}

.cm-inline-breakpoint.cm-inline-conditional {
  --override-auto-gen-cminlinebreakpointcminlineconditional-backgroundcolor: #ef9d0d;

  background-color: var(--override-auto-gen-cminlinebreakpointcminlineconditional-backgroundcolor);
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-inline-conditional,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-inline-conditional {
  --override-auto-gen-cminlinebreakpointcminlineconditional-backgroundcolor: rgb(242 160 16);
}

.cm-continue-to-location {
  cursor: pointer;
  opacity: 80%;
  position: relative;
  top: 2px;
}

.cm-continue-to-location:hover {
  opacity: 100%;
}

div.CodeMirror:focus-within span.CodeMirror-matchingbracket {
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-borderbottom: rgb(0 0 0 / 50%);
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-backgroundcolor: rgb(0 0 0 / 7%);

  background-color: var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-backgroundcolor);
  border-bottom: 1px solid var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-borderbottom);
}

div.CodeMirror:focus-within span.CodeMirror-nonmatchingbracket {
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-borderbottom: rgb(255 0 0 / 50%);
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-backgroundcolor: rgb(255 0 0 / 7%);

  background-color: var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-backgroundcolor);
  border-bottom: 1px solid var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-borderbottom);
}

.-theme-with-dark-background div.CodeMirror:focus-within span.CodeMirror-matchingbracket,
:host-context(.-theme-with-dark-background) div.CodeMirror:focus-within span.CodeMirror-matchingbracket {
  border-bottom: 1px solid rgb(217 217 217);
  background-color: initial;
}

.-theme-with-dark-background div.CodeMirror:focus-within span.CodeMirror-nonmatchingbracket,
:host-context(.-theme-with-dark-background) div.CodeMirror:focus-within span.CodeMirror-nonmatchingbracket {
  border-bottom: 1px solid rgb(255 26 26);
  background-color: initial;
}

.cm-whitespace::before {
  --override-auto-gen-cmwhitespacebefore-color: rgb(175 175 175);

  position: absolute;
  pointer-events: none;
  color: var(--override-auto-gen-cmwhitespacebefore-color);
}

.-theme-with-dark-background .cm-whitespace::before,
:host-context(.-theme-with-dark-background) .cm-whitespace::before {
  --override-auto-gen-cmwhitespacebefore-color: rgb(80 80 80);
}

.cm-tab {
  display: inline-block;
  text-decoration: inherit;
  position: relative;
}

.cm-tab::before {
  --override-auto-gen-cmtabbefore-borderbottom: rgb(175 175 175);

  display: none;
  content: ".";
  color: transparent;
  border-bottom: 1px solid var(--override-auto-gen-cmtabbefore-borderbottom);
  position: absolute;
  width: 90%;
  bottom: 50%;
  left: 5%;
}

.-theme-with-dark-background .cm-tab::before,
:host-context(.-theme-with-dark-background) .cm-tab::before {
  --override-auto-gen-cmtabbefore-borderbottom: rgb(80 80 80);
}

.show-whitespaces .CodeMirror .cm-tab::before {
  display: block !important; /* stylelint-disable-line declaration-no-important */
}

.cm-execution-line {
  --override-auto-gen-cmexecutionline-backgroundcolor: rgb(0 59 255 / 10%);

  background-color: var(--override-auto-gen-cmexecutionline-backgroundcolor);
}

.cm-execution-line-outline {
  --override-auto-gen-cmexecutionlineoutline-outline: rgb(64 115 244);

  outline: 1px solid var(--override-auto-gen-cmexecutionlineoutline-outline);
}

.cm-execution-line-tail {
  --override-auto-gen-cmexecutionlinetail-backgroundcolor: rgb(171 191 254);

  background-color: var(--override-auto-gen-cmexecutionlinetail-backgroundcolor);
}

.-theme-with-dark-background .cm-execution-line,
:host-context(.-theme-with-dark-background) .cm-execution-line {
  background-color: #14522b;
}

.-theme-with-dark-background .cm-execution-line-outline,
:host-context(.-theme-with-dark-background) .cm-execution-line-outline {
  outline: 1px solid #33cc6b;
}

.-theme-with-dark-background .cm-execution-line-tail,
:host-context(.-theme-with-dark-background) .cm-execution-line-tail {
  background-color: #347132;
}

.cm-token-highlight {
  position: relative;
}

.cm-token-highlight::before {
  position: absolute;
  border: 1px solid var(--override-search-highlight-border-color);
  border-radius: 3px;
  top: 0;
  bottom: -1px;
  left: 0;
  right: 0;
  content: "";
}

.cm-line-with-selection .cm-column-with-selection::before {
  border: none;
}

.cm-search-highlight {
  position: relative;
}

.cm-search-highlight::before {
  position: absolute;
  border-top-style: solid;
  border-bottom-style: solid;
  border-top-color: var(--override-search-highlight-border-color);
  border-bottom-color: var(--override-search-highlight-border-color);
  border-top-width: 1px;
  border-bottom-width: 1px;
  top: -1px;
  bottom: 0;
  left: 0;
  right: 0;
  content: "";
}

.cm-search-highlight-full::before {
  border: 1px solid var(--override-search-highlight-border-color);
  border-radius: 3px;
}

.cm-search-highlight-start::before {
  border-left-width: 1px;
  border-top-left-radius: 2px;
  border-bottom-left-radius: 2px;
  border-left-style: solid;
  border-left-color: var(--override-search-highlight-border-color);
}

.cm-search-highlight-end::before {
  border-right-width: 1px;
  border-top-right-radius: 2px;
  border-bottom-right-radius: 2px;
  border-right-style: solid;
  border-right-color: var(--override-search-highlight-border-color);
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight-full::before {
  border-radius: 1px;
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight-start::before {
  border-top-left-radius: 1px;
  border-bottom-left-radius: 1px;
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight-end::before {
  border-top-right-radius: 1px;
  border-bottom-right-radius: 1px;
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight::before {
  --override-auto-gen-cmlinewithselectioncmcolumnwithselectioncmsearchhighlightbefore-backgroundcolor: rgb(241 234 0);

  margin: -1px -1px -1px -1px;
  background-color: var(--override-auto-gen-cmlinewithselectioncmcolumnwithselectioncmsearchhighlightbefore-backgroundcolor);
  z-index: -1;
}

.-theme-with-dark-background .cm-line-with-selection .cm-column-with-selection.cm-search-highlight::before,
:host-context(.-theme-with-dark-background) .cm-line-with-selection .cm-column-with-selection.cm-search-highlight::before {
  background-color: hsl(133deg 100% 30%);
}

.-theme-with-dark-background .cm-line-with-selection .cm-search-highlight,
:host-context(.-theme-with-dark-background) .cm-line-with-selection .cm-search-highlight {
  color: #eee;
}

.CodeMirror .text-editor-line-marker-text {
  text-align: right;
  padding-right: 3px;
  height: 12px;
}

.CodeMirror .text-editor-line-marker-text span.line-marker-units {
  color: var(--color-text-secondary);
  font-size: 75%;
  margin-left: 3px;
}

.CodeMirror .text-editor-coverage-unused-marker {
  text-align: right;
  padding-right: 2px;
  background-color: var(--color-accent-red);
}

.CodeMirror .text-editor-coverage-unused-marker::after {
  content: "\200B";
}

.CodeMirror .text-editor-coverage-used-marker {
  --override-auto-gen-codemirrortexteditorcoverageusedmarker-backgroundcolor: #63acbe;

  text-align: right;
  padding-right: 2px;
  background-color: var(--override-auto-gen-codemirrortexteditorcoverageusedmarker-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .text-editor-coverage-used-marker,
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-coverage-used-marker {
  --override-auto-gen-codemirrortexteditorcoverageusedmarker-backgroundcolor: rgb(65 138 156);
}

.CodeMirror .text-editor-coverage-used-marker::after {
  content: "\200B";
}

.CodeMirror .text-editor-line-decoration {
  position: absolute;
}

.CodeMirror .text-editor-line-decoration-wave {
  position: absolute;
  top: -2px;
  right: -4px;
  left: 4px;
  cursor: pointer;
  height: 4px;
  background-image: var(--image-file-errorWave);
  background-repeat: repeat-x;
  background-size: contain;
}

.CodeMirror .text-editor-value-decoration {
  --override-auto-gen-codemirrortexteditorvaluedecoration-backgroundcolor: #ffe3c7;

  position: absolute;
  bottom: 0;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  max-width: 1000px;
  opacity: 80%;
  background-color: var(--override-auto-gen-codemirrortexteditorvaluedecoration-backgroundcolor);
  margin-left: 10px;
  padding-left: 5px;
  color: var(--color-text-primary);
  user-select: text;
}

.-theme-with-dark-background .CodeMirror .text-editor-value-decoration,
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-value-decoration {
  --override-auto-gen-codemirrortexteditorvaluedecoration-backgroundcolor: rgb(56 28 0);
}

.CodeMirror .cm-execution-line .text-editor-value-decoration {
  background-color: transparent;
  opacity: 50%;
}

.CodeMirror .text-editor-line-decoration-icon {
  cursor: pointer;
}

.CodeMirror .text-editor-line-decoration-icon > * {
  vertical-align: text-bottom;
  margin-left: 2px;
}

.CodeMirror .text-editor-line-decoration-icon-issue {
  cursor: pointer;
}

.CodeMirror .text-editor-line-with-warning:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewithwarningnotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(241 230 0 / 10%);

  background-color: var(--override-auto-gen-codemirrortexteditorlinewithwarningnotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .text-editor-line-with-warning:not(.cm-execution-line):not(.cm-readonly-highlight),
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-line-with-warning:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewithwarningnotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(255 244 14 / 10%);
}

.CodeMirror .text-editor-line-with-error:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewitherrornotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(255 0 0 / 5%);

  background-color: var(--override-auto-gen-codemirrortexteditorlinewitherrornotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .text-editor-line-with-error:not(.cm-execution-line):not(.cm-readonly-highlight),
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-line-with-error:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewitherrornotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(255 0 0 / 5%);
}

.CodeMirror .CodeMirror-vscrollbar,
.CodeMirror .CodeMirror-hscrollbar {
  transform: translateZ(0);
}

.cm-trailing-whitespace {
  --override-auto-gen-cmtrailingwhitespace-backgroundcolor: rgb(255 0 0 / 5%);

  background-color: var(--override-auto-gen-cmtrailingwhitespace-backgroundcolor);
}

.-theme-with-dark-background .cm-trailing-whitespace,
:host-context(.-theme-with-dark-background) .cm-trailing-whitespace {
  --override-auto-gen-cmtrailingwhitespace-backgroundcolor: rgb(255 0 0 / 5%);
}

.CodeMirror-activeline .cm-trailing-whitespace {
  background-color: transparent;
}

.CodeMirror .CodeMirror-selected {
  background-color: var(--legacy-item-selection-inactive-bg-color);
}

.CodeMirror-focused .CodeMirror-selected {
  background-color: var(--legacy-item-selection-bg-color);
}

.-theme-with-dark-background .CodeMirror .CodeMirror-selected,
:host-context(.-theme-with-dark-background) .CodeMirror .CodeMirror-selected {
  background-color: #454545;
}

.-theme-with-dark-background span.CodeMirror-selectedtext,
:host-context(.-theme-with-dark-background) span.CodeMirror-selectedtext {
  background-color: #454545;
}

.CodeMirror .auto-complete-text {
  color: var(--color-text-secondary);
}

.CodeMirror .placeholder-text {
  height: 0;
  color: var(--color-text-secondary);
}

.CodeMirror textarea {
  resize: none;
  overflow: hidden;
}

.CodeMirror-lines {
  padding: 4px 0; /* Vertical padding around content */
}

.CodeMirror pre {
  padding: 0 4px; /* Horizontal padding of content */
}

.CodeMirror-scrollbar-filler,
.CodeMirror-gutter-filler {
  /* The little square between H and V scrollbars */
  background-color: var(--color-background);
}

.CodeMirror div.CodeMirror-secondarycursor {
  --override-auto-gen-codemirrordivcodemirrorsecondarycursor-borderleft: #c0c0c0;

  border-left: 1px solid var(--override-auto-gen-codemirrordivcodemirrorsecondarycursor-borderleft);
}

.-theme-with-dark-background .CodeMirror div.CodeMirror-secondarycursor,
:host-context(.-theme-with-dark-background) .CodeMirror div.CodeMirror-secondarycursor {
  --override-auto-gen-codemirrordivcodemirrorsecondarycursor-borderleft: rgb(63 63 63);
}

.CodeMirror-composing {
  border-bottom: 2px solid;
}

.CodeMirror-foldmarker {
  cursor: pointer;
  font-size: 0;
  line-height: 0;
  height: 0;
}

.CodeMirror-foldmarker::before {
  content: '\2026';
  font-size: 13px;
  color: var(--color-text-secondary);
}

.CodeMirror-foldgutter {
  width: 1.5em;
}

.CodeMirror-gutters:hover .CodeMirror-foldgutter {
  background-color: transparent;
}

.CodeMirror-foldgutter-open,
.CodeMirror-foldgutter-folded {
  cursor: pointer;
  position: relative;
}

.CodeMirror-foldgutter-open {
  transition: opacity 0.2s;
  opacity: 0%;
}

.CodeMirror-gutter-hovered .CodeMirror-foldgutter-open {
  opacity: 100%;
}

.CodeMirror-foldgutter-open::before,
.CodeMirror-foldgutter-folded::before {
  background-color: var(--color-text-secondary);
  user-select: none;
  -webkit-mask-image: var(--image-file-treeoutlineTriangles);
  -webkit-mask-size: 32px 24px;
  content: "";
  display: block;
  width: 8px;
  color: transparent;
  text-shadow: none;
  height: 12px;
  position: absolute;
  right: 4px;
}

.CodeMirror-foldgutter-open::before {
  -webkit-mask-position: -16px 0;
}

.CodeMirror-foldgutter-folded::before {
  -webkit-mask-position: 0 0;
}

.CodeMirror .CodeMirror-line::selection,
.CodeMirror .CodeMirror-line > span::selection,
.CodeMirror .CodeMirror-line > span > span::selection {
  background: var(--legacy-item-selection-bg-color);
}

@media (forced-colors: active) {
  .cm-token-highlight::before {
    forced-color-adjust: none;
    border-color: Highlight;
  }
}

/* stylelint-enable no-descending-specificity */

/*# sourceURL=ui/legacy/components/text_editor/cmdevtools.css */x<canvas id="application-canvas" tabindex="0" style="user-select: none; width: 1365px; height: 971px;" width="1365" height="971" class="fill-mode-FILL_WINDOW"></canvas><script src="files/assets/140310720/1/ammo.wasm.js"></script>/* The rest of this file contains styles related to the mechanics of
   the editor. You probably shouldn't touch them. */

.CodeMirror {
  position: relative;
  overflow: hidden;
  background: var(--color-background);
}

.CodeMirror-scroll {
  overflow: scroll !important; /* Things will break if this is overridden */
  /* 50px is the magic margin used to hide the element's real scrollbars */
  /* See overflow: hidden in .CodeMirror */
  margin-bottom: -50px;
  margin-right: -50px;
  padding-bottom: 50px;
  height: 100%;
  outline: none; /* Prevent dragging from highlighting the element */
  position: relative;
}

.CodeMirror-sizer {
  position: relative;
  border-right: 50px solid transparent;
}

/* The fake, visible scrollbars. Used to force redraw during scrolling
   before actual scrolling happens, thus preventing shaking and
   flickering artifacts. */
.CodeMirror-vscrollbar,
.CodeMirror-hscrollbar,
.CodeMirror-scrollbar-filler,
.CodeMirror-gutter-filler {
  position: absolute;
  z-index: 6;
  display: none;
  outline: none;
}

.CodeMirror-vscrollbar {
  right: 0;
  top: 0;
  overflow-x: hidden;
  overflow-y: scroll;
}

.CodeMirror-hscrollbar {
  bottom: 0;
  left: 0;
  overflow-y: hidden;
  overflow-x: scroll;
}

.CodeMirror-scrollbar-filler {
  right: 0;
  bottom: 0;
}

.CodeMirror-gutter-filler {
  left: 0;
  bottom: 0;
}

.CodeMirror-gutters {
  position: absolute;
  left: 0;
  top: 0;
  min-height: 100%;
  z-index: 3;
}

.CodeMirror-gutter {
  white-space: normal;
  height: 100%;
  display: inline-block;
  vertical-align: top;
  margin-bottom: -50px;
}

.CodeMirror-gutter-wrapper {
  position: absolute;
  z-index: 4;
  background: none !important;
  border: none !important;
}

.CodeMirror-gutter-background {
  position: absolute;
  top: 0;
  bottom: 0;
  z-index: 4;
}

.CodeMirror-gutter-elt {
  position: absolute;
  cursor: default;
  z-index: 4;
}

.CodeMirror-gutter-wrapper ::selection {
  background-color: transparent;
}

.CodeMirror-gutter-wrapper ::-moz-selection {
  background-color: transparent;
}

.CodeMirror-lines {
  cursor: text;
  min-height: 1px; /* prevents collapsing before first draw */
}

.CodeMirror pre.CodeMirror-line,
.CodeMirror pre.CodeMirror-line-like {
  /* Reset some styles that the rest of the page might have set */
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -moz-border-radius: 0;
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -webkit-border-radius: 0;
  border-radius: 0;
  border-width: 0;
  background: transparent;
  font-family: inherit;
  font-size: inherit;
  margin: 0;
  white-space: pre;
  word-wrap: normal;
  line-height: inherit;
  color: inherit;
  z-index: 2;
  position: relative;
  overflow: visible;
  -webkit-tap-highlight-color: transparent;
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -webkit-font-variant-ligatures: contextual;
  font-variant-ligatures: contextual;
}

.CodeMirror-wrap pre.CodeMirror-line,
.CodeMirror-wrap pre.CodeMirror-line-like {
  word-wrap: break-word;
  white-space: pre-wrap;
  word-break: normal;
}

.CodeMirror-linebackground {
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  z-index: 0;
}

.CodeMirror-linewidget {
  position: relative;
  z-index: 2;
  padding: 0.1px; /* Force widget margins to stay inside of the container */
}

.CodeMirror-rtl pre {
  direction: rtl;
}

.CodeMirror-code {
  outline: none;
}

/* Force content-box sizing for the elements where we expect it */
.CodeMirror-scroll,
.CodeMirror-sizer,
.CodeMirror-gutter,
.CodeMirror-gutters,
.CodeMirror-linenumber {
  /* stylelint-disable-next-line property-no-vendor-prefix */
  -moz-box-sizing: content-box;
  box-sizing: content-box;
}

.CodeMirror-measure {
  position: absolute;
  width: 100%;
  height: 0;
  overflow: hidden;
  visibility: hidden;
}

.CodeMirror-cursor {
  position: absolute;
  pointer-events: none;
}

.CodeMirror-measure pre {
  position: static;
}

div.CodeMirror-cursors {
  visibility: hidden;
  position: relative;
  z-index: 3;
}

div.CodeMirror-dragcursors {
  visibility: visible;
}

.CodeMirror-focused div.CodeMirror-cursors {
  visibility: visible;
}

.CodeMirror-selected {
  --override-cm-selected-background-color: #d9d9d9;

  background: var(--override-cm-selected-background-color);
}

.-theme-with-dark-background .CodeMirror-selected,
:host-context(.-theme-with-dark-background) .CodeMirror-selected {
  --override-cm-selected-background-color: rgb(38 38 38);
}

.CodeMirror-focused .CodeMirror-selected {
  --override-cm-selected-background-color: #d7d4f0;
}

.-theme-with-dark-background .CodeMirror-focused .CodeMirror-selected,
:host-context(.-theme-with-dark-background) .CodeMirror-focused .CodeMirror-selected {
  --override-cm-selected-background-color: rgb(18 15 43);
}

.CodeMirror-crosshair {
  cursor: crosshair;
}

.CodeMirror-line {
  --override-line-selection-background-color: #d7d4f0;
}

.CodeMirror-line::selection,
.CodeMirror-line > span::selection,
.CodeMirror-line > span > span::selection {
  background:var(--override-line-selection-background-color);
}

.CodeMirror-line::-moz-selection,
.CodeMirror-line > span::-moz-selection,
.CodeMirror-line > span > span::-moz-selection {
  background: var(--override-line-selection-background-color);
}

.-theme-with-dark-background .CodeMirror-line,
:host-context(.-theme-with-dark-background) .CodeMirror-line {
  --override-line-selection-background-color: rgb(18 15 43);

}

.cm-searching {
  --override-searching-background-color: rgb(255 255 0 / 40%);

  background-color: var(--override-searching-background-color);
}

/* Used to force a border model for a node */
.cm-force-border {
  padding-right: 0.1px;
}

@media print {
  /* Hide the cursor when printing */
  .CodeMirror div.CodeMirror-cursors {
    visibility: hidden;
  }
}

/* See issue #2901 */
.cm-tab-wrap-hack::after {
  content: "";
}

/* Help users use markselection to safely style text background */
span.CodeMirror-selectedtext {
  background: none;
}

/*# sourceURL=third_party/codemirror/codemirror.css *//*
 * Copyright 2021 The Chromium Authors. All rights reserved.
 * Use of this source code is governed by a BSD-style license that can be
 * found in the LICENSE file.
 */

/* stylelint-disable no-descending-specificity */

/**
 * Many of the CSS variables here were auto generated during the dark mode
 * migration. If you are changing them, please feel free to rename them whilst
 * you're here to make them clearer.
 */

.CodeMirror {
  --override-search-highlight-border-color: rgb(128 128 128);

  line-height: 1.2em !important; /* stylelint-disable-line declaration-no-important */
  background-color: transparent !important; /* stylelint-disable-line declaration-no-important */
  color: var(--color-text-primary);
  height: 300px;
}

.CodeMirror-linewidget {
  overflow: visible !important; /* stylelint-disable-line declaration-no-important */
}

.CodeMirror-gutter-performance {
  width: 60px;
  background-color: var(--color-background);
  margin-left: 3px;
}

.CodeMirror-gutter-memory {
  width: 48px;
  background-color: var(--color-background);
  margin-left: 3px;
}

.CodeMirror-gutter-coverage {
  width: 5px;
  background-color: var(--color-background);
  margin-left: 3px;
}

.CodeMirror .source-frame-eval-expression {
  --override-auto-gen-codemirrorsourceframeevalexpression-backgroundcolor: rgb(255 255 194);
  --override-auto-gen-codemirrorsourceframeevalexpression-border: rgb(163 41 34);

  outline: 0;
  border: 1px solid var(--override-auto-gen-codemirrorsourceframeevalexpression-border);
  border-left-width: 0;
  border-right-width: 0;
  background-color: var(--override-auto-gen-codemirrorsourceframeevalexpression-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .source-frame-eval-expression,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-eval-expression {
  --override-auto-gen-codemirrorsourceframeevalexpression-border: rgb(221 99 92);
  --override-auto-gen-codemirrorsourceframeevalexpression-backgroundcolor: rgb(61 61 0);
}

.CodeMirror .source-frame-eval-expression-start {
  border-left-width: 1px;
  margin-left: -1px;
}

.CodeMirror .source-frame-eval-expression-end {
  border-right-width: 1px;
  margin-right: -1px;
}

.CodeMirror .source-frame-continue-to-location {
  --override-auto-gen-codemirrorsourceframecontinuetolocation-backgroundcolor: rgb(230 236 255);

  outline: 0;
  border: 1px solid transparent;
  border-left-width: 0;
  border-right-width: 0;
  background-color: var(--override-auto-gen-codemirrorsourceframecontinuetolocation-backgroundcolor);
  cursor: pointer;
}

.CodeMirror .source-frame-continue-to-location:hover {
  --override-auto-gen-codemirrorsourceframecontinuetolocationhover-backgroundcolor: rgb(171 191 254);
  --override-auto-gen-codemirrorsourceframecontinuetolocationhover-border: rgb(121 141 254);

  border: 1px solid var(--override-auto-gen-codemirrorsourceframecontinuetolocationhover-border);
  background-color: var(--override-auto-gen-codemirrorsourceframecontinuetolocationhover-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .source-frame-continue-to-location,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-continue-to-location {
  background-color: #14522b;
}

.-theme-with-dark-background .CodeMirror .source-frame-continue-to-location:hover,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-continue-to-location:hover {
  border: 1px solid #33cc6b;
  background-color: #14522b;
}

.CodeMirror .source-frame-continue-to-location-start {
  border-left-width: 1px;
  margin-left: -1px;
}

.CodeMirror .source-frame-continue-to-location-end {
  border-right-width: 1px;
  margin-right: -1px;
}

.CodeMirror .source-frame-async-step-in {
  --override-auto-gen-codemirrorsourceframeasyncstepin-backgroundcolor: hsl(100deg 46% 80% / 100%);

  outline: 0;
  background-color: var(--override-auto-gen-codemirrorsourceframeasyncstepin-backgroundcolor);
  cursor: pointer;
  border: 1px solid transparent;
  border-left-width: 0;
  border-right-width: 0;
}

.-theme-with-dark-background .CodeMirror .source-frame-async-step-in,
:host-context(.-theme-with-dark-background) .CodeMirror .source-frame-async-step-in {
  --override-auto-gen-codemirrorsourceframeasyncstepin-backgroundcolor: rgb(43 74 28);
}

.source-frame-async-step-in-hovered .source-frame-async-step-in {
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-bordercolor: rgb(100 154 100);
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-backgroundcolor: hsl(96deg 53% 65%);

  background-color: var(--override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-backgroundcolor);
  border-color: var(--override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-bordercolor);
}

.-theme-with-dark-background .source-frame-async-step-in-hovered .source-frame-async-step-in,
:host-context(.-theme-with-dark-background) .source-frame-async-step-in-hovered .source-frame-async-step-in {
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-backgroundcolor: rgb(80 137 42);
  --override-auto-gen-sourceframeasyncstepinhoveredsourceframeasyncstepin-bordercolor: rgb(101 155 101);
}

.source-frame-async-step-in-hovered .source-frame-async-step-in-start {
  border-left-width: 1px;
  margin-left: -1px;
}

.source-frame-async-step-in-hovered .source-frame-async-step-in-end {
  border-right-width: 1px;
  margin-right: -1px;
}

.CodeMirror-cursor {
  border-left: 1px solid var(--color-background-inverted);
  border-right: none;
  width: 0;
}

.CodeMirror-readonly .CodeMirror-cursor {
  display: none;
}

.CodeMirror-gutters {
  border-right: 1px solid var(--color-details-hairline);
  white-space: nowrap;
  background-color: var(--color-background);
}

.CodeMirror-linenumber {
  --override-auto-gen-codemirrorlinenumber-color: hsl(0deg 0% 46%);

  color: var(--override-auto-gen-codemirrorlinenumber-color);
  padding: 0 3px 0 9px;
  min-width: 28px;
  text-align: right;
  white-space: nowrap;
}

.-theme-with-dark-background .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .CodeMirror-linenumber {
  --override-auto-gen-codemirrorlinenumber-color: rgb(138 138 138);
}

.pretty-printed .CodeMirror-linenumber {
  color: var(--legacy-accent-color);
}

.cm-non-breakable-line .CodeMirror-linenumber {
  --override-auto-gen-cmnonbreakablelinecodemirrorlinenumber-color: rgb(128 128 128 / 40%);

  color: var(--override-auto-gen-cmnonbreakablelinecodemirrorlinenumber-color);
}

.-theme-with-dark-background .cm-non-breakable-line .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-non-breakable-line .CodeMirror-linenumber {
  --override-auto-gen-cmnonbreakablelinecodemirrorlinenumber-color: rgb(127 127 127 / 40%);
}

.cm-highlight {
  animation: fadeout 2s 0s;
}

.-theme-with-dark-background .cm-highlight,
:host-context(.-theme-with-dark-background) .cm-highlight {
  animation: fadeout-dark 2s 0s;
}

@keyframes fadeout {
  from {
    background-color: rgb(255 255 120); /* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: var(--color-background); }
}

@keyframes fadeout {
  from {
    background-color: rgb(255 255 120); /* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: var(--color-background); }
}

@keyframes fadeout-dark {
  from {
    background-color: hsl(133deg 100% 30% / 50%);/* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: transparent; }
}

@keyframes fadeout-dark {
  from {
    background-color: hsl(133deg 100% 30% / 50%);/* stylelint-disable-line plugin/use_theme_colors */
  }
  to { background-color: transparent; }
}

.cm-readonly-highlight {
  --override-auto-gen-cmreadonlyhighlight-backgroundcolor: rgb(255 255 120);

  background-color: var(--override-auto-gen-cmreadonlyhighlight-backgroundcolor);
}

.-theme-with-dark-background .cm-readonly-highlight,
:host-context(.-theme-with-dark-background) .cm-readonly-highlight {
  background-color: hsl(133deg 100% 30% / 50%);
}

.cm-highlight.cm-execution-line {
  animation: fadeout-execution-line 1s 0s;
}

.-theme-with-dark-background .cm-highlight.cm-execution-line,
:host-context(.-theme-with-dark-background) .cm-highlight.cm-execution-line {
  animation: fadeout-execution-line-dark 1s 0s;
}

@keyframes fadeout-execution-line {
  from {
    background-color: rgb(121 141 254);/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: rgb(171 191 254);/* stylelint-disable-line plugin/use_theme_colors */
  }
}

@keyframes fadeout-execution-line {
  from {
    background-color: rgb(121 141 254);/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: rgb(171 191 254);/* stylelint-disable-line plugin/use_theme_colors */
  }
}

@keyframes fadeout-execution-line-dark {
  from {
    background-color: #208043;/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: #14522b;/* stylelint-disable-line plugin/use_theme_colors */
  }
}

@keyframes fadeout-execution-line-dark {
  from {
    background-color: #208043;/* stylelint-disable-line plugin/use_theme_colors */
  }

  to {
    background-color: #14522b;/* stylelint-disable-line plugin/use_theme_colors */
  }
}

.CodeMirror-linenumber:hover,
.cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-preserve {
  border-width: 1px 4px 1px 1px;
  padding-right: 3px;
  padding-left: 8px;
  height: 11px;
  line-height: 12px;
  border-style: solid;
  position: relative;
  /* The line number jumps slightly on hover when the minify banner is showing
     if this fractional value is not there. */
  top: -0.15px;
}

.CodeMirror-linenumber:hover {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23ebeced" stroke="%23ebeced"/></svg>') 1 3 1 1;
  padding-left: 8px;
}

.-theme-with-dark-background .CodeMirror-linenumber:hover,
:host-context(.-theme-with-dark-background) .CodeMirror-linenumber:hover {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%233c4043" stroke="%233c4043"/></svg>') 1 3 1 1;
}

.cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color: #fff;

  color: var(--override-auto-gen-cmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%234285f4" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%235186EC" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.cm-breakpoint-disabled .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.breakpoints-deactivated .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointdisabledcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color: #1a73e8;

  color: var(--override-auto-gen-cmbreakpointdisabledcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23d9e7fd" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-disabled .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-with-dark-background .breakpoints-deactivated .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-disabled .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .breakpoints-deactivated .cm-breakpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  color: #1a73e8;
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%232a384e" stroke="%231a73e8"/></svg>') 1 3 1 1;
}

.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23f29900" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23e9a33a" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.cm-breakpoint-disabled.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.breakpoints-deactivated .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointdisabledcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-color: #e37400;

  color: var(--override-auto-gen-cmbreakpointdisabledcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointconditionalcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23fcebcc" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-disabled.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-with-dark-background .breakpoints-deactivated .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-disabled.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .breakpoints-deactivated .cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  color: #e37400;
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%234d3c1d" stroke="%23e37400"/></svg>') 1 3 1 1;
}

.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23f439a0" stroke="%23d01884"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23E54D9B" stroke="%23d01884"/></svg>') 1 3 1 1;
}

.cm-breakpoint-disabled.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.breakpoints-deactivated .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  --override-auto-gen-cmbreakpointdisabledcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-color: #d01884;

  color: var(--override-auto-gen-cmbreakpointdisabledcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-breakpointsdeactivatedcmbreakpointlogpointcodemirrorgutterwrappercodemirrorlinenumber-color);
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%23fdd7ec" stroke="%23f439a0"/></svg>') 1 3 1 1;
}

.-theme-with-dark-background .cm-breakpoint-disabled.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
.-theme-with-dark-background .breakpoints-deactivated .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .cm-breakpoint-disabled.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber,
:host-context(.-theme-with-dark-background) .breakpoints-deactivated .cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber {
  color: #d01884;
  -webkit-border-image: url('data:image/svg+xml,<svg height="11" width="26" xmlns="http://www.w3.org/2000/svg"><path d="M22.8.5l2.7 5-2.7 5H.5V.5z" fill="%234e283d" stroke="%23f439a0"/></svg>') 1 3 1 1;
}

.cm-breakpoint-conditional .CodeMirror-gutter-wrapper .CodeMirror-linenumber::before,
.-theme-preserve {
  content: "?";
  position: absolute;
  top: 0;
  left: 1px;
}

.cm-breakpoint-logpoint .CodeMirror-gutter-wrapper .CodeMirror-linenumber::before,
.-theme-preserve {
  content: "‥";
  position: absolute;
  top: -3px;
  left: 1px;
}

.cm-inline-breakpoint {
  cursor: pointer;
  position: relative;
  top: 1px;
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%234285F4" stroke="%231A73E8"/></svg>');
  height: 10px;
}

.-theme-with-dark-background .cm-inline-breakpoint,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%235186EC" stroke="%231A73E8"/></svg>');
}

.cm-inline-breakpoint.cm-inline-disabled,
.breakpoints-deactivated .cm-inline-breakpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%234285F4" fill-opacity="0.2" stroke="%231A73E8"/></svg>');
}

.cm-inline-breakpoint.cm-inline-breakpoint-conditional {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.75489 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.75489 11.2583 6.29382 11.5 5.80138 11.5H0.5V0.5Z" fill="%23F29900" stroke="%23E37400"/><path d="M3.51074 7.75635H4.68408V9H3.51074V7.75635ZM4.68408 7.23779H3.51074V6.56104C3.51074 6.271 3.55615 6.02344 3.64697 5.81836C3.73779 5.61328 3.90039 5.39648 4.13477 5.16797L4.53027 4.77686C4.71484 4.59814 4.83936 4.4502 4.90381 4.33301C4.97119 4.21582 5.00488 4.09424 5.00488 3.96826C5.00488 3.77197 4.9375 3.62402 4.80273 3.52441C4.66797 3.4248 4.46582 3.375 4.19629 3.375C3.9502 3.375 3.69238 3.42773 3.42285 3.5332C3.15625 3.63574 2.88232 3.78955 2.60107 3.99463V2.81689C2.88818 2.65283 3.17822 2.52979 3.47119 2.44775C3.76709 2.36279 4.06299 2.32031 4.35889 2.32031C4.95068 2.32031 5.41504 2.45801 5.75195 2.7334C6.08887 3.00879 6.25732 3.38818 6.25732 3.87158C6.25732 4.09424 6.20752 4.30225 6.10791 4.49561C6.0083 4.68604 5.8208 4.91602 5.54541 5.18555L5.15869 5.56348C4.95947 5.75684 4.83203 5.91504 4.77637 6.03809C4.7207 6.16113 4.69287 6.31201 4.69287 6.49072C4.69287 6.51709 4.69141 6.54785 4.68848 6.58301C4.68848 6.61816 4.68701 6.65625 4.68408 6.69727V7.23779Z" fill="white"/></svg>');
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-inline-breakpoint-conditional,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-inline-breakpoint-conditional {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.75489 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.75489 11.2583 6.29382 11.5 5.80138 11.5H0.5V0.5Z" fill="%23e9a33a" stroke="%23E37400"/><path d="M3.51074 7.75635H4.68408V9H3.51074V7.75635ZM4.68408 7.23779H3.51074V6.56104C3.51074 6.271 3.55615 6.02344 3.64697 5.81836C3.73779 5.61328 3.90039 5.39648 4.13477 5.16797L4.53027 4.77686C4.71484 4.59814 4.83936 4.4502 4.90381 4.33301C4.97119 4.21582 5.00488 4.09424 5.00488 3.96826C5.00488 3.77197 4.9375 3.62402 4.80273 3.52441C4.66797 3.4248 4.46582 3.375 4.19629 3.375C3.9502 3.375 3.69238 3.42773 3.42285 3.5332C3.15625 3.63574 2.88232 3.78955 2.60107 3.99463V2.81689C2.88818 2.65283 3.17822 2.52979 3.47119 2.44775C3.76709 2.36279 4.06299 2.32031 4.35889 2.32031C4.95068 2.32031 5.41504 2.45801 5.75195 2.7334C6.08887 3.00879 6.25732 3.38818 6.25732 3.87158C6.25732 4.09424 6.20752 4.30225 6.10791 4.49561C6.0083 4.68604 5.8208 4.91602 5.54541 5.18555L5.15869 5.56348C4.95947 5.75684 4.83203 5.91504 4.77637 6.03809C4.7207 6.16113 4.69287 6.31201 4.69287 6.49072C4.69287 6.51709 4.69141 6.54785 4.68848 6.58301C4.68848 6.61816 4.68701 6.65625 4.68408 6.69727V7.23779Z" fill="white"/></svg>');
}

.cm-inline-breakpoint.cm-inline-breakpoint-conditional.cm-inline-disabled,
.breakpoints-deactivated .cm-inline-breakpoint.cm-inline-breakpoint-conditional {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.75489 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.75489 11.2583 6.29382 11.5 5.80138 11.5H0.5V0.5Z" fill="%23F9AB00" fill-opacity="0.2" stroke="%23E37400"/><path d="M3.51074 7.75635H4.68408V9H3.51074V7.75635ZM4.68408 7.23779H3.51074V6.56104C3.51074 6.271 3.55615 6.02344 3.64697 5.81836C3.73779 5.61328 3.90039 5.39648 4.13477 5.16797L4.53027 4.77686C4.71484 4.59814 4.83936 4.4502 4.90381 4.33301C4.97119 4.21582 5.00488 4.09424 5.00488 3.96826C5.00488 3.77197 4.9375 3.62402 4.80273 3.52441C4.66797 3.4248 4.46582 3.375 4.19629 3.375C3.9502 3.375 3.69238 3.42773 3.42285 3.5332C3.15625 3.63574 2.88232 3.78955 2.60107 3.99463V2.81689C2.88818 2.65283 3.17822 2.52979 3.47119 2.44775C3.76709 2.36279 4.06299 2.32031 4.35889 2.32031C4.95068 2.32031 5.41504 2.45801 5.75195 2.7334C6.08887 3.00879 6.25732 3.38818 6.25732 3.87158C6.25732 4.09424 6.20752 4.30225 6.10791 4.49561C6.0083 4.68604 5.8208 4.91602 5.54541 5.18555L5.15869 5.56348C4.95947 5.75684 4.83203 5.91504 4.77637 6.03809C4.7207 6.16113 4.69287 6.31201 4.69287 6.49072C4.69287 6.51709 4.69141 6.54785 4.68848 6.58301C4.68848 6.61816 4.68701 6.65625 4.68408 6.69727V7.23779Z" fill="%23E37400"/></svg>');
}

.cm-inline-breakpoint.cm-inline-logpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%23F439A0" stroke="%23D01884"/><circle cx="3" cy="6" r="1" fill="white"/><circle cx="7" cy="6" r="1" fill="white"/></svg>');
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-inline-logpoint,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-inline-logpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%23E54D9B" stroke="%23D01884"/><circle cx="3" cy="6" r="1" fill="white"/><circle cx="7" cy="6" r="1" fill="white"/></svg>');
}

.cm-inline-breakpoint.cm-inline-logpoint.cm-inline-disabled,
.breakpoints-deactivated .cm-inline-breakpoint.cm-inline-logpoint {
  content: url('data:image/svg+xml,<svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M0.5 0.5H5.80139C6.29382 0.5 6.7549 0.741701 7.03503 1.14669L10.392 6L7.03503 10.8533C6.7549 11.2583 6.29382 11.5 5.80139 11.5H0.5V0.5Z" fill="%23F439A0" fill-opacity="0.2" stroke="%23D01884"/><circle cx="3" cy="6" r="1" fill="%23D01884"/><circle cx="7" cy="6" r="1" fill="%23D01884"/></svg>');
}

.cm-execution-line-tail + .CodeMirror-widget {
  --override-auto-gen-cmexecutionlinetailcodemirrorwidget-backgroundcolor: #abbffe;

  background-color: var(--override-auto-gen-cmexecutionlinetailcodemirrorwidget-backgroundcolor);
}

.-theme-with-dark-background .cm-execution-line-tail + .CodeMirror-widget,
:host-context(.-theme-with-dark-background) .cm-execution-line-tail + .CodeMirror-widget {
  --override-auto-gen-cmexecutionlinetailcodemirrorwidget-backgroundcolor: rgb(1 21 84);
}

.source-frame-eval-expression + .CodeMirror-widget {
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-backgroundcolor: rgb(255 255 194);
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-border: rgb(163 41 34);

  border: 1px solid var(--override-auto-gen-sourceframeevalexpressioncodemirrorwidget-border);
  border-left-width: 0;
  border-right-width: 0;
  background-color: var(--override-auto-gen-sourceframeevalexpressioncodemirrorwidget-backgroundcolor);
}

.-theme-with-dark-background .source-frame-eval-expression + .CodeMirror-widget,
:host-context(.-theme-with-dark-background) .source-frame-eval-expression + .CodeMirror-widget {
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-border: rgb(221 99 92);
  --override-auto-gen-sourceframeevalexpressioncodemirrorwidget-backgroundcolor: rgb(61 61 0);
}

.cm-inline-breakpoint.cm-execution-line-tail {
  --override-auto-gen-cminlinebreakpointcmexecutionlinetail-backgroundcolor: #698cfe;

  background-color: var(--override-auto-gen-cminlinebreakpointcmexecutionlinetail-backgroundcolor);
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-execution-line-tail,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-execution-line-tail {
  --override-auto-gen-cminlinebreakpointcmexecutionlinetail-backgroundcolor: rgb(1 36 150);
}

.cm-execution-line-tail .cm-inline-breakpoint {
  background-color: var(--color-background);
}

.cm-inline-breakpoint.cm-inline-conditional {
  --override-auto-gen-cminlinebreakpointcminlineconditional-backgroundcolor: #ef9d0d;

  background-color: var(--override-auto-gen-cminlinebreakpointcminlineconditional-backgroundcolor);
}

.-theme-with-dark-background .cm-inline-breakpoint.cm-inline-conditional,
:host-context(.-theme-with-dark-background) .cm-inline-breakpoint.cm-inline-conditional {
  --override-auto-gen-cminlinebreakpointcminlineconditional-backgroundcolor: rgb(242 160 16);
}

.cm-continue-to-location {
  cursor: pointer;
  opacity: 80%;
  position: relative;
  top: 2px;
}

.cm-continue-to-location:hover {
  opacity: 100%;
}

div.CodeMirror:focus-within span.CodeMirror-matchingbracket {
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-borderbottom: rgb(0 0 0 / 50%);
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-backgroundcolor: rgb(0 0 0 / 7%);

  background-color: var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-backgroundcolor);
  border-bottom: 1px solid var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrormatchingbracket-borderbottom);
}

div.CodeMirror:focus-within span.CodeMirror-nonmatchingbracket {
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-borderbottom: rgb(255 0 0 / 50%);
  --override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-backgroundcolor: rgb(255 0 0 / 7%);

  background-color: var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-backgroundcolor);
  border-bottom: 1px solid var(--override-auto-gen-divcodemirrorfocuswithinspancodemirrornonmatchingbracket-borderbottom);
}

.-theme-with-dark-background div.CodeMirror:focus-within span.CodeMirror-matchingbracket,
:host-context(.-theme-with-dark-background) div.CodeMirror:focus-within span.CodeMirror-matchingbracket {
  border-bottom: 1px solid rgb(217 217 217);
  background-color: initial;
}

.-theme-with-dark-background div.CodeMirror:focus-within span.CodeMirror-nonmatchingbracket,
:host-context(.-theme-with-dark-background) div.CodeMirror:focus-within span.CodeMirror-nonmatchingbracket {
  border-bottom: 1px solid rgb(255 26 26);
  background-color: initial;
}

.cm-whitespace::before {
  --override-auto-gen-cmwhitespacebefore-color: rgb(175 175 175);

  position: absolute;
  pointer-events: none;
  color: var(--override-auto-gen-cmwhitespacebefore-color);
}

.-theme-with-dark-background .cm-whitespace::before,
:host-context(.-theme-with-dark-background) .cm-whitespace::before {
  --override-auto-gen-cmwhitespacebefore-color: rgb(80 80 80);
}

.cm-tab {
  display: inline-block;
  text-decoration: inherit;
  position: relative;
}

.cm-tab::before {
  --override-auto-gen-cmtabbefore-borderbottom: rgb(175 175 175);

  display: none;
  content: ".";
  color: transparent;
  border-bottom: 1px solid var(--override-auto-gen-cmtabbefore-borderbottom);
  position: absolute;
  width: 90%;
  bottom: 50%;
  left: 5%;
}

.-theme-with-dark-background .cm-tab::before,
:host-context(.-theme-with-dark-background) .cm-tab::before {
  --override-auto-gen-cmtabbefore-borderbottom: rgb(80 80 80);
}

.show-whitespaces .CodeMirror .cm-tab::before {
  display: block !important; /* stylelint-disable-line declaration-no-important */
}

.cm-execution-line {
  --override-auto-gen-cmexecutionline-backgroundcolor: rgb(0 59 255 / 10%);

  background-color: var(--override-auto-gen-cmexecutionline-backgroundcolor);
}

.cm-execution-line-outline {
  --override-auto-gen-cmexecutionlineoutline-outline: rgb(64 115 244);

  outline: 1px solid var(--override-auto-gen-cmexecutionlineoutline-outline);
}

.cm-execution-line-tail {
  --override-auto-gen-cmexecutionlinetail-backgroundcolor: rgb(171 191 254);

  background-color: var(--override-auto-gen-cmexecutionlinetail-backgroundcolor);
}

.-theme-with-dark-background .cm-execution-line,
:host-context(.-theme-with-dark-background) .cm-execution-line {
  background-color: #14522b;
}

.-theme-with-dark-background .cm-execution-line-outline,
:host-context(.-theme-with-dark-background) .cm-execution-line-outline {
  outline: 1px solid #33cc6b;
}

.-theme-with-dark-background .cm-execution-line-tail,
:host-context(.-theme-with-dark-background) .cm-execution-line-tail {
  background-color: #347132;
}

.cm-token-highlight {
  position: relative;
}

.cm-token-highlight::before {
  position: absolute;
  border: 1px solid var(--override-search-highlight-border-color);
  border-radius: 3px;
  top: 0;
  bottom: -1px;
  left: 0;
  right: 0;
  content: "";
}

.cm-line-with-selection .cm-column-with-selection::before {
  border: none;
}

.cm-search-highlight {
  position: relative;
}

.cm-search-highlight::before {
  position: absolute;
  border-top-style: solid;
  border-bottom-style: solid;
  border-top-color: var(--override-search-highlight-border-color);
  border-bottom-color: var(--override-search-highlight-border-color);
  border-top-width: 1px;
  border-bottom-width: 1px;
  top: -1px;
  bottom: 0;
  left: 0;
  right: 0;
  content: "";
}

.cm-search-highlight-full::before {
  border: 1px solid var(--override-search-highlight-border-color);
  border-radius: 3px;
}

.cm-search-highlight-start::before {
  border-left-width: 1px;
  border-top-left-radius: 2px;
  border-bottom-left-radius: 2px;
  border-left-style: solid;
  border-left-color: var(--override-search-highlight-border-color);
}

.cm-search-highlight-end::before {
  border-right-width: 1px;
  border-top-right-radius: 2px;
  border-bottom-right-radius: 2px;
  border-right-style: solid;
  border-right-color: var(--override-search-highlight-border-color);
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight-full::before {
  border-radius: 1px;
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight-start::before {
  border-top-left-radius: 1px;
  border-bottom-left-radius: 1px;
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight-end::before {
  border-top-right-radius: 1px;
  border-bottom-right-radius: 1px;
}

.cm-line-with-selection .cm-column-with-selection.cm-search-highlight::before {
  --override-auto-gen-cmlinewithselectioncmcolumnwithselectioncmsearchhighlightbefore-backgroundcolor: rgb(241 234 0);

  margin: -1px -1px -1px -1px;
  background-color: var(--override-auto-gen-cmlinewithselectioncmcolumnwithselectioncmsearchhighlightbefore-backgroundcolor);
  z-index: -1;
}

.-theme-with-dark-background .cm-line-with-selection .cm-column-with-selection.cm-search-highlight::before,
:host-context(.-theme-with-dark-background) .cm-line-with-selection .cm-column-with-selection.cm-search-highlight::before {
  background-color: hsl(133deg 100% 30%);
}

.-theme-with-dark-background .cm-line-with-selection .cm-search-highlight,
:host-context(.-theme-with-dark-background) .cm-line-with-selection .cm-search-highlight {
  color: #eee;
}

.CodeMirror .text-editor-line-marker-text {
  text-align: right;
  padding-right: 3px;
  height: 12px;
}

.CodeMirror .text-editor-line-marker-text span.line-marker-units {
  color: var(--color-text-secondary);
  font-size: 75%;
  margin-left: 3px;
}

.CodeMirror .text-editor-coverage-unused-marker {
  text-align: right;
  padding-right: 2px;
  background-color: var(--color-accent-red);
}

.CodeMirror .text-editor-coverage-unused-marker::after {
  content: "\200B";
}

.CodeMirror .text-editor-coverage-used-marker {
  --override-auto-gen-codemirrortexteditorcoverageusedmarker-backgroundcolor: #63acbe;

  text-align: right;
  padding-right: 2px;
  background-color: var(--override-auto-gen-codemirrortexteditorcoverageusedmarker-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .text-editor-coverage-used-marker,
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-coverage-used-marker {
  --override-auto-gen-codemirrortexteditorcoverageusedmarker-backgroundcolor: rgb(65 138 156);
}

.CodeMirror .text-editor-coverage-used-marker::after {
  content: "\200B";
}

.CodeMirror .text-editor-line-decoration {
  position: absolute;
}

.CodeMirror .text-editor-line-decoration-wave {
  position: absolute;
  top: -2px;
  right: -4px;
  left: 4px;
  cursor: pointer;
  height: 4px;
  background-image: var(--image-file-errorWave);
  background-repeat: repeat-x;
  background-size: contain;
}

.CodeMirror .text-editor-value-decoration {
  --override-auto-gen-codemirrortexteditorvaluedecoration-backgroundcolor: #ffe3c7;

  position: absolute;
  bottom: 0;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  max-width: 1000px;
  opacity: 80%;
  background-color: var(--override-auto-gen-codemirrortexteditorvaluedecoration-backgroundcolor);
  margin-left: 10px;
  padding-left: 5px;
  color: var(--color-text-primary);
  user-select: text;
}

.-theme-with-dark-background .CodeMirror .text-editor-value-decoration,
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-value-decoration {
  --override-auto-gen-codemirrortexteditorvaluedecoration-backgroundcolor: rgb(56 28 0);
}

.CodeMirror .cm-execution-line .text-editor-value-decoration {
  background-color: transparent;
  opacity: 50%;
}

.CodeMirror .text-editor-line-decoration-icon {
  cursor: pointer;
}

.CodeMirror .text-editor-line-decoration-icon > * {
  vertical-align: text-bottom;
  margin-left: 2px;
}

.CodeMirror .text-editor-line-decoration-icon-issue {
  cursor: pointer;
}

.CodeMirror .text-editor-line-with-warning:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewithwarningnotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(241 230 0 / 10%);

  background-color: var(--override-auto-gen-codemirrortexteditorlinewithwarningnotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .text-editor-line-with-warning:not(.cm-execution-line):not(.cm-readonly-highlight),
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-line-with-warning:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewithwarningnotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(255 244 14 / 10%);
}

.CodeMirror .text-editor-line-with-error:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewitherrornotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(255 0 0 / 5%);

  background-color: var(--override-auto-gen-codemirrortexteditorlinewitherrornotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor);
}

.-theme-with-dark-background .CodeMirror .text-editor-line-with-error:not(.cm-execution-line):not(.cm-readonly-highlight),
:host-context(.-theme-with-dark-background) .CodeMirror .text-editor-line-with-error:not(.cm-execution-line):not(.cm-readonly-highlight) {
  --override-auto-gen-codemirrortexteditorlinewitherrornotcmexecutionlinenotcmreadonlyhighlight-backgroundcolor: rgb(255 0 0 / 5%);
}

.CodeMirror .CodeMirror-vscrollbar,
.CodeMirror .CodeMirror-hscrollbar {
  transform: translateZ(0);
}

.cm-trailing-whitespace {
  --override-auto-gen-cmtrailingwhitespace-backgroundcolor: rgb(255 0 0 / 5%);

  background-color: var(--override-auto-gen-cmtrailingwhitespace-backgroundcolor);
}

.-theme-with-dark-background .cm-trailing-whitespace,
:host-context(.-theme-with-dark-background) .cm-trailing-whitespace {
  --override-auto-gen-cmtrailingwhitespace-backgroundcolor: rgb(255 0 0 / 5%);
}

.CodeMirror-activeline .cm-trailing-whitespace {
  background-color: transparent;
}

.CodeMirror .CodeMirror-selected {
  background-color: var(--legacy-item-selection-inactive-bg-color);
}

.CodeMirror-focused .CodeMirror-selected {
  background-color: var(--legacy-item-selection-bg-color);
}

.-theme-with-dark-background .CodeMirror .CodeMirror-selected,
:host-context(.-theme-with-dark-background) .CodeMirror .CodeMirror-selected {
  background-color: #454545;
}

.-theme-with-dark-background span.CodeMirror-selectedtext,
:host-context(.-theme-with-dark-background) span.CodeMirror-selectedtext {
  background-color: #454545;
}

.CodeMirror .auto-complete-text {
  color: var(--color-text-secondary);
}

.CodeMirror .placeholder-text {
  height: 0;
  color: var(--color-text-secondary);
}

.CodeMirror textarea {
  resize: none;
  overflow: hidden;
}

.CodeMirror-lines {
  padding: 4px 0; /* Vertical padding around content */
}

.CodeMirror pre {
  padding: 0 4px; /* Horizontal padding of content */
}

.CodeMirror-scrollbar-filler,
.CodeMirror-gutter-filler {
  /* The little square between H and V scrollbars */
  background-color: var(--color-background);
}

.CodeMirror div.CodeMirror-secondarycursor {
  --override-auto-gen-codemirrordivcodemirrorsecondarycursor-borderleft: #c0c0c0;

  border-left: 1px solid var(--override-auto-gen-codemirrordivcodemirrorsecondarycursor-borderleft);
}

.-theme-with-dark-background .CodeMirror div.CodeMirror-secondarycursor,
:host-context(.-theme-with-dark-background) .CodeMirror div.CodeMirror-secondarycursor {
  --override-auto-gen-codemirrordivcodemirrorsecondarycursor-borderleft: rgb(63 63 63);
}

.CodeMirror-composing {
  border-bottom: 2px solid;
}

.CodeMirror-foldmarker {
  cursor: pointer;
  font-size: 0;
  line-height: 0;
  height: 0;
}

.CodeMirror-foldmarker::before {
  content: '\2026';
  font-size: 13px;
  color: var(--color-text-secondary);
}

.CodeMirror-foldgutter {
  width: 1.5em;
}

.CodeMirror-gutters:hover .CodeMirror-foldgutter {
  background-color: transparent;
}

.CodeMirror-foldgutter-open,
.CodeMirror-foldgutter-folded {
  cursor: pointer;
  position: relative;
}

.CodeMirror-foldgutter-open {
  transition: opacity 0.2s;
  opacity: 0%;
}

.CodeMirror-gutter-hovered .CodeMirror-foldgutter-open {
  opacity: 100%;
}

.CodeMirror-foldgutter-open::before,
.CodeMirror-foldgutter-folded::before {
  background-color: var(--color-text-secondary);
  user-select: none;
  -webkit-mask-image: var(--image-file-treeoutlineTriangles);
  -webkit-mask-size: 32px 24px;
  content: "";
  display: block;
  width: 8px;
  color: transparent;
  text-shadow: none;
  height: 12px;
  position: absolute;
  right: 4px;
}

.CodeMirror-foldgutter-open::before {
  -webkit-mask-position: -16px 0;
}

.CodeMirror-foldgutter-folded::before {
  -webkit-mask-position: 0 0;
}

.CodeMirror .CodeMirror-line::selection,
.CodeMirror .CodeMirror-line > span::selection,
.CodeMirror .CodeMirror-line > span > span::selection {
  background: var(--legacy-item-selection-bg-color);
}

@media (forced-colors: active) {
  .cm-token-highlight::before {
    forced-color-adjust: none;
    border-color: Highlight;
  }
}

/* stylelint-enable no-descending-specificity */

/*# sourceURL=ui/legacy/components/text_editor/cmdevtools.css */x<script src="files/assets/140310720/1/ammo.wasm.js"></script>
