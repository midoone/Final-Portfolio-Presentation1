# Final-Portfolio-Presentation1
<!DOCTYPE HTML>
<html lang="en-US">
<head>
  <meta charset="UTF-8" /><script type="text/javascript">(window.NREUM||(NREUM={})).loader_config={licenseKey:"e7fb1b89a0",applicationID:"750147145"};window.NREUM||(NREUM={}),__nr_require=function(e,t,n){function r(n){if(!t[n]){var i=t[n]={exports:{}};e[n][0].call(i.exports,function(t){var i=e[n][1][t];return r(i||t)},i,i.exports)}return t[n].exports}if("function"==typeof __nr_require)return __nr_require;for(var i=0;i<n.length;i++)r(n[i]);return r}({1:[function(e,t,n){function r(){}function i(e,t,n){return function(){return o(e,[u.now()].concat(c(arguments)),t?null:this,n),t?void 0:this}}var o=e("handle"),a=e(6),c=e(7),f=e("ee").get("tracer"),u=e("loader"),s=NREUM;"undefined"==typeof window.newrelic&&(newrelic=s);var d=["setPageViewName","setCustomAttribute","setErrorHandler","finished","addToTrace","inlineHit","addRelease"],p="api-",l=p+"ixn-";a(d,function(e,t){s[t]=i(p+t,!0,"api")}),s.addPageAction=i(p+"addPageAction",!0),s.setCurrentRouteName=i(p+"routeName",!0),t.exports=newrelic,s.interaction=function(){return(new r).get()};var m=r.prototype={createTracer:function(e,t){var n={},r=this,i="function"==typeof t;return o(l+"tracer",[u.now(),e,n],r),function(){if(f.emit((i?"":"no-")+"fn-start",[u.now(),r,i],n),i)try{return t.apply(this,arguments)}catch(e){throw f.emit("fn-err",[arguments,this,e],n),e}finally{f.emit("fn-end",[u.now()],n)}}}};a("actionText,setName,setAttribute,save,ignore,onEnd,getContext,end,get".split(","),function(e,t){m[t]=i(l+t)}),newrelic.noticeError=function(e,t){"string"==typeof e&&(e=new Error(e)),o("err",[e,u.now(),!1,t])}},{}],2:[function(e,t,n){function r(){return c.exists&&performance.now?Math.round(performance.now()):(o=Math.max((new Date).getTime(),o))-a}function i(){return o}var o=(new Date).getTime(),a=o,c=e(8);t.exports=r,t.exports.offset=a,t.exports.getLastTimestamp=i},{}],3:[function(e,t,n){function r(e,t){var n=e.getEntries();n.forEach(function(e){"first-paint"===e.name?d("timing",["fp",Math.floor(e.startTime)]):"first-contentful-paint"===e.name&&d("timing",["fcp",Math.floor(e.startTime)])})}function i(e,t){var n=e.getEntries();n.length>0&&d("lcp",[n[n.length-1]])}function o(e){e.getEntries().forEach(function(e){e.hadRecentInput||d("cls",[e])})}function a(e){if(e instanceof m&&!g){var t=Math.round(e.timeStamp),n={type:e.type};t<=p.now()?n.fid=p.now()-t:t>p.offset&&t<=Date.now()?(t-=p.offset,n.fid=p.now()-t):t=p.now(),g=!0,d("timing",["fi",t,n])}}function c(e){d("pageHide",[p.now(),e])}if(!("init"in NREUM&&"page_view_timing"in NREUM.init&&"enabled"in NREUM.init.page_view_timing&&NREUM.init.page_view_timing.enabled===!1)){var f,u,s,d=e("handle"),p=e("loader"),l=e(5),m=NREUM.o.EV;if("PerformanceObserver"in window&&"function"==typeof window.PerformanceObserver){f=new PerformanceObserver(r);try{f.observe({entryTypes:["paint"]})}catch(v){}u=new PerformanceObserver(i);try{u.observe({entryTypes:["largest-contentful-paint"]})}catch(v){}s=new PerformanceObserver(o);try{s.observe({type:"layout-shift",buffered:!0})}catch(v){}}if("addEventListener"in document){var g=!1,y=["click","keydown","mousedown","pointerdown","touchstart"];y.forEach(function(e){document.addEventListener(e,a,!1)})}l(c)}},{}],4:[function(e,t,n){function r(e,t){if(!i)return!1;if(e!==i)return!1;if(!t)return!0;if(!o)return!1;for(var n=o.split("."),r=t.split("."),a=0;a<r.length;a++)if(r[a]!==n[a])return!1;return!0}var i=null,o=null,a=/Version\/(\S+)\s+Safari/;if(navigator.userAgent){var c=navigator.userAgent,f=c.match(a);f&&c.indexOf("Chrome")===-1&&c.indexOf("Chromium")===-1&&(i="Safari",o=f[1])}t.exports={agent:i,version:o,match:r}},{}],5:[function(e,t,n){function r(e){function t(){e(a&&document[a]?document[a]:document[i]?"hidden":"visible")}"addEventListener"in document&&o&&document.addEventListener(o,t,!1)}t.exports=r;var i,o,a;"undefined"!=typeof document.hidden?(i="hidden",o="visibilitychange",a="visibilityState"):"undefined"!=typeof document.msHidden?(i="msHidden",o="msvisibilitychange"):"undefined"!=typeof document.webkitHidden&&(i="webkitHidden",o="webkitvisibilitychange",a="webkitVisibilityState")},{}],6:[function(e,t,n){function r(e,t){var n=[],r="",o=0;for(r in e)i.call(e,r)&&(n[o]=t(r,e[r]),o+=1);return n}var i=Object.prototype.hasOwnProperty;t.exports=r},{}],7:[function(e,t,n){function r(e,t,n){t||(t=0),"undefined"==typeof n&&(n=e?e.length:0);for(var r=-1,i=n-t||0,o=Array(i<0?0:i);++r<i;)o[r]=e[t+r];return o}t.exports=r},{}],8:[function(e,t,n){t.exports={exists:"undefined"!=typeof window.performance&&window.performance.timing&&"undefined"!=typeof window.performance.timing.navigationStart}},{}],ee:[function(e,t,n){function r(){}function i(e){function t(e){return e&&e instanceof r?e:e?f(e,c,o):o()}function n(n,r,i,o){if(!p.aborted||o){e&&e(n,r,i);for(var a=t(i),c=v(n),f=c.length,u=0;u<f;u++)c[u].apply(a,r);var d=s[w[n]];return d&&d.push([b,n,r,a]),a}}function l(e,t){h[e]=v(e).concat(t)}function m(e,t){var n=h[e];if(n)for(var r=0;r<n.length;r++)n[r]===t&&n.splice(r,1)}function v(e){return h[e]||[]}function g(e){return d[e]=d[e]||i(n)}function y(e,t){u(e,function(e,n){t=t||"feature",w[n]=t,t in s||(s[t]=[])})}var h={},w={},b={on:l,addEventListener:l,removeEventListener:m,emit:n,get:g,listeners:v,context:t,buffer:y,abort:a,aborted:!1};return b}function o(){return new r}function a(){(s.api||s.feature)&&(p.aborted=!0,s=p.backlog={})}var c="nr@context",f=e("gos"),u=e(6),s={},d={},p=t.exports=i();p.backlog=s},{}],gos:[function(e,t,n){function r(e,t,n){if(i.call(e,t))return e[t];var r=n();if(Object.defineProperty&&Object.keys)try{return Object.defineProperty(e,t,{value:r,writable:!0,enumerable:!1}),r}catch(o){}return e[t]=r,r}var i=Object.prototype.hasOwnProperty;t.exports=r},{}],handle:[function(e,t,n){function r(e,t,n,r){i.buffer([e],r),i.emit(e,t,n)}var i=e("ee").get("handle");t.exports=r,r.ee=i},{}],id:[function(e,t,n){function r(e){var t=typeof e;return!e||"object"!==t&&"function"!==t?-1:e===window?0:a(e,o,function(){return i++})}var i=1,o="nr@id",a=e("gos");t.exports=r},{}],loader:[function(e,t,n){function r(){if(!E++){var e=b.info=NREUM.info,t=p.getElementsByTagName("script")[0];if(setTimeout(u.abort,3e4),!(e&&e.licenseKey&&e.applicationID&&t))return u.abort();f(h,function(t,n){e[t]||(e[t]=n)});var n=a();c("mark",["onload",n+b.offset],null,"api"),c("timing",["load",n]);var r=p.createElement("script");r.src="https://"+e.agent,t.parentNode.insertBefore(r,t)}}function i(){"complete"===p.readyState&&o()}function o(){c("mark",["domContent",a()+b.offset],null,"api")}var a=e(2),c=e("handle"),f=e(6),u=e("ee"),s=e(4),d=window,p=d.document,l="addEventListener",m="attachEvent",v=d.XMLHttpRequest,g=v&&v.prototype;NREUM.o={ST:setTimeout,SI:d.setImmediate,CT:clearTimeout,XHR:v,REQ:d.Request,EV:d.Event,PR:d.Promise,MO:d.MutationObserver};var y=""+location,h={beacon:"bam.nr-data.net",errorBeacon:"bam.nr-data.net",agent:"js-agent.newrelic.com/nr-1184.min.js"},w=v&&g&&g[l]&&!/CriOS/.test(navigator.userAgent),b=t.exports={offset:a.getLastTimestamp(),now:a,origin:y,features:{},xhrWrappable:w,userAgent:s};e(1),e(3),p[l]?(p[l]("DOMContentLoaded",o,!1),d[l]("load",r,!1)):(p[m]("onreadystatechange",i),d[m]("onload",r)),c("mark",["firstbyte",a.getLastTimestamp()],null,"api");var E=0},{}],"wrap-function":[function(e,t,n){function r(e){return!(e&&e instanceof Function&&e.apply&&!e[a])}var i=e("ee"),o=e(7),a="nr@original",c=Object.prototype.hasOwnProperty,f=!1;t.exports=function(e,t){function n(e,t,n,i){function nrWrapper(){var r,a,c,f;try{a=this,r=o(arguments),c="function"==typeof n?n(r,a):n||{}}catch(u){p([u,"",[r,a,i],c])}s(t+"start",[r,a,i],c);try{return f=e.apply(a,r)}catch(d){throw s(t+"err",[r,a,d],c),d}finally{s(t+"end",[r,a,f],c)}}return r(e)?e:(t||(t=""),nrWrapper[a]=e,d(e,nrWrapper),nrWrapper)}function u(e,t,i,o){i||(i="");var a,c,f,u="-"===i.charAt(0);for(f=0;f<t.length;f++)c=t[f],a=e[c],r(a)||(e[c]=n(a,u?c+i:i,o,c))}function s(n,r,i){if(!f||t){var o=f;f=!0;try{e.emit(n,r,i,t)}catch(a){p([a,n,r,i])}f=o}}function d(e,t){if(Object.defineProperty&&Object.keys)try{var n=Object.keys(e);return n.forEach(function(n){Object.defineProperty(t,n,{get:function(){return e[n]},set:function(t){return e[n]=t,t}})}),t}catch(r){p([r])}for(var i in e)c.call(e,i)&&(t[i]=e[i]);return t}function p(t){try{e.emit("internal-error",t)}catch(n){}}return e||(e=i),n.inPlace=u,n.flag=a,n}},{}]},{},["loader"]);</script>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
      <meta name="twitter:card"  content="summary_large_image" />
      <meta name="twitter:site"  content="@AdobePortfolio" />
      <meta  property="og:title" content="AZIYAR AHMED SALEK" />
      <meta  property="og:image" content="https://pro2-bar-s3-cdn-cf1.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/2514c6fe-11fa-4264-bd52-43ab656a8fb7_car_4x3.png?h=9f7ffbde12069cf77f267a157c0895ff" />
      <link rel="icon" href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQAQMAAAAlPW0iAAAABGdBTUEAALGPC/xhBQAAAAFzUkdCAK7OHOkAAAADUExURUxpcU3H2DoAAAABdFJOUwBA5thmAAAADElEQVQI12NgIA0AAAAwAAHHqoWOAAAAAElFTkSuQmCC"  />
      <link rel="stylesheet" href="/dist/css/main.css" type="text/css" />
      <link rel="stylesheet" href="https://pro2-bar-s3-cdn-cf4.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/fec3263a366c87c569294ab3c5d29f151608065936.css?h=abea7ce2a4ff1966b682461efebc3590" type="text/css" />
    <link rel="canonical" href="https://aziyarahmedsalek.myportfolio.com/work" />
      <title>AZIYAR AHMED SALEK</title>
</head>
  <body class="transition-enabled">  <div class='page-background-video page-background-video-with-panel'>
  </div>
  <div class="js-responsive-nav">
    <div class="responsive-nav has-social">
      <div class="close-responsive-click-area js-close-responsive-nav">
        <div class="close-responsive-button"></div>
      </div>
          <nav class="nav-container" data-hover-hint="nav" data-hover-hint-placement="bottom-start">
                <div class="gallery-title"><a href="/work" class="active">Home</a></div>
                <div class="gallery-title"><a href="/about-me" >About Me</a></div>
      <div class="page-title">
        <a href="/contact" >Contact Me</a>
      </div>
          </nav>
        <div class="social pf-nav-social" data-context="theme.nav" data-hover-hint="navSocialIcons" data-hover-hint-placement="bottom-start">
          <ul>
          </ul>
        </div>
    </div>
  </div>
    <header class="site-header js-site-header  js-fixed-nav" data-context="theme.nav" data-hover-hint="nav" data-hover-hint-placement="top-start">
        <nav class="nav-container" data-hover-hint="nav" data-hover-hint-placement="bottom-start">
                <div class="gallery-title"><a href="/work" class="active">Home</a></div>
                <div class="gallery-title"><a href="/about-me" >About Me</a></div>
      <div class="page-title">
        <a href="/contact" >Contact Me</a>
      </div>
        </nav>
        <div class="logo-wrap" data-context="theme.logo.header" data-hover-hint="logo" data-hover-hint-placement="bottom-start">
          <div class="logo e2e-site-logo-text logo-text  ">
              <a href="/work" class="preserve-whitespace">AZIYAR AHMED </a>

          </div>
        </div>
        <div class="social pf-nav-social" data-context="theme.nav" data-hover-hint="navSocialIcons" data-hover-hint-placement="bottom-start">
          <ul>
          </ul>
        </div>
        <div class="hamburger-click-area js-hamburger">
          <div class="hamburger">
            <i></i>
            <i></i>
            <i></i>
          </div>
        </div>
    </header>
    <div class="header-placeholder"></div>
        <div class="masthead js-masthead-fixed" data-context="page.masthead" data-hover-hint="mastheadOptions" data-hover-hint-placement="top-start">
          <div class="masthead-contents">
            <div class="masthead-text js-masthead-text">
              <div data-context="page.masthead" data-hover-hint="mastheadTitle"><h1 decorator="inlineTextEditable" contenteditable="false" class="js-inline-text-editable preserve-whitespace main-text rich-text module-text" data-text-keypath="customizations.masthead.title.text" value="Welcome to Ahmed Portfolio">Welcome to Ahmed Portfolio</h1></div>
              <div data-context="page.masthead" data-hover-hint="mastheadText"><p decorator="inlineTextEditable" contenteditable="false" class="js-inline-text-editable preserve-whitespace main-text rich-text module-text" data-text-keypath="page.masthead.text.text" value=""></p></div>
              <div class="masthead-buttons">
                
              </div>
                <div class="social masthead-social" data-context="page.masthead" data-hover-hint="mastheadSocialIcons">
                  <ul>
                  </ul>
                </div>
                <div class="masthead-arrow-container js-masthead-arrow" data-context="page.masthead" data-hover-hint="scrollDownArrow">
                  <div class="masthead-arrow"></div>
                </div>
            </div>
          </div>
        </div>
        <div class="masthead masthead-placeholder">
          <div class="masthead-contents">
            <div class="masthead-text js-masthead-text">
              <div data-context="page.masthead" data-hover-hint="mastheadTitle"><h1 decorator="inlineTextEditable" contenteditable="false" class="js-inline-text-editable preserve-whitespace main-text rich-text module-text" data-text-keypath="customizations.masthead.title.text" value="Welcome to Ahmed Portfolio">Welcome to Ahmed Portfolio</h1></div>
              <div data-context="page.masthead" data-hover-hint="mastheadText"><p decorator="inlineTextEditable" contenteditable="false" class="js-inline-text-editable preserve-whitespace main-text rich-text module-text" data-text-keypath="page.masthead.text.text" value=""></p></div>
              <div class="masthead-buttons">
                
              </div>
                <div class="social masthead-social" data-context="page.masthead" data-hover-hint="mastheadSocialIcons">
                  <ul>
                  </ul>
                </div>
                <div class="masthead-arrow-container js-masthead-arrow" data-context="page.masthead" data-hover-hint="scrollDownArrow">
                  <div class="masthead-arrow"></div>
                </div>
            </div>
          </div>
        </div>
  <div class="site-wrap cfix js-site-wrap">
    <div class="site-container">
      <div class="site-content e2e-site-content">
        <main>
          <section class="project-covers" data-context="page.gallery.covers">
          <a class="project-cover js-project-cover-touch hold-space" href="/skills" data-context="pages" data-identity="id:p5f9b5f7e1d286d41fe5e10ef2bcef714d83a11f6eb5d5d60061ac" data-hover-hint-id="p5f9b5f7e1d286d41fe5e10ef2bcef714d83a11f6eb5d5d60061ac" data-hover-hint="galleryPageCover">
              <div class="cover-image-wrap">
                <div class="cover-image">
                    <div class="cover cover-normal">

            <img
              class="cover__img js-lazy"
              src="https://pro2-bar-s3-cdn-cf1.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/2514c6fe-11fa-4264-bd52-43ab656a8fb7_carw_4x3x32.png?h=bb4dcec69a3c902cafae38a82746ef00"
              data-src="https://pro2-bar-s3-cdn-cf1.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/2514c6fe-11fa-4264-bd52-43ab656a8fb7_car_4x3.png?h=9f7ffbde12069cf77f267a157c0895ff"
              data-srcset="https://pro2-bar-s3-cdn-cf1.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/2514c6fe-11fa-4264-bd52-43ab656a8fb7_carw_4x3x640.png?h=a9dfc85fc1f9498b3967274b9cb64bb0 640w, https://pro2-bar-s3-cdn-cf1.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/2514c6fe-11fa-4264-bd52-43ab656a8fb7_carw_4x3x1280.png?h=7fa8956f1615a37671a66234469b4c04 1280w, https://pro2-bar-s3-cdn-cf1.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/2514c6fe-11fa-4264-bd52-43ab656a8fb7_carw_4x3x1366.png?h=297f33167a0bf2b818720b03e6050245 1366w, https://pro2-bar-s3-cdn-cf1.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/2514c6fe-11fa-4264-bd52-43ab656a8fb7_carw_4x3x1920.png?h=42092b6cb38db35e41b1c7ba6ad017f4 1920w, https://pro2-bar-s3-cdn-cf1.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/2514c6fe-11fa-4264-bd52-43ab656a8fb7_carw_4x3x2560.png?h=cf6260a02710a67989ddccb763fb6795 2560w, https://pro2-bar-s3-cdn-cf1.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/2514c6fe-11fa-4264-bd52-43ab656a8fb7_carw_4x3x5120.png?h=f84394831c7b7875b259f94645efda0a 5120w"
              data-sizes="(max-width: 540px) 100vw, (max-width: 768px) 50vw, calc(1200px / 2)"
            >
                              </div>
                </div>
              </div>
            <div class="details-wrap">
              <div class="details">
                <div class="details-inner">
                    <div class="title preserve-whitespace">Skills</div>
                </div>
              </div>
            </div>
          </a>
          <a class="project-cover js-project-cover-touch hold-space" href="/accomplishments" data-context="pages" data-identity="id:p5f9a1ff486734a5c11f9a1b4ac1c8d2444ca83f5b44a037fcccb4" data-hover-hint-id="p5f9a1ff486734a5c11f9a1b4ac1c8d2444ca83f5b44a037fcccb4" data-hover-hint="galleryPageCover">
              <div class="cover-image-wrap">
                <div class="cover-image">
                    <div class="cover cover-normal">

            <img
              class="cover__img js-lazy"
              src="https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/0df21088-c524-4c1e-9c4e-9936583e688f_rwc_150x0x893x670x32.png?h=2797274ed181e3b031a4bb32b163d711"
              data-src="https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/0df21088-c524-4c1e-9c4e-9936583e688f_rwc_150x0x893x670x893.png?h=207dcb5208e5467d22217949083a146d"
              data-srcset="https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/0df21088-c524-4c1e-9c4e-9936583e688f_rwc_150x0x893x670x640.png?h=d3e02f66553d255e4a9a2ad79d6e9db2 640w, https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/0df21088-c524-4c1e-9c4e-9936583e688f_rwc_150x0x893x670x893.png?h=207dcb5208e5467d22217949083a146d 1280w, https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/0df21088-c524-4c1e-9c4e-9936583e688f_rwc_150x0x893x670x893.png?h=207dcb5208e5467d22217949083a146d 1366w, https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/0df21088-c524-4c1e-9c4e-9936583e688f_rwc_150x0x893x670x893.png?h=207dcb5208e5467d22217949083a146d 1920w, https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/0df21088-c524-4c1e-9c4e-9936583e688f_rwc_150x0x893x670x893.png?h=207dcb5208e5467d22217949083a146d 2560w, https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/0df21088-c524-4c1e-9c4e-9936583e688f_rwc_150x0x893x670x893.png?h=207dcb5208e5467d22217949083a146d 5120w"
              data-sizes="(max-width: 540px) 100vw, (max-width: 768px) 50vw, calc(1200px / 2)"
            >
                              </div>
                </div>
              </div>
            <div class="details-wrap">
              <div class="details">
                <div class="details-inner">
                    <div class="title preserve-whitespace">Accomplishments</div>
                </div>
              </div>
            </div>
          </a>
          <a class="project-cover js-project-cover-touch hold-space" href="/meet-ahmed" data-context="pages" data-identity="id:p5f921b3a13a24c0b0b27cb2c8dd3e92cf0e7884aeaa2eecedf388" data-hover-hint-id="p5f921b3a13a24c0b0b27cb2c8dd3e92cf0e7884aeaa2eecedf388" data-hover-hint="galleryPageCover">
              <div class="cover-image-wrap">
                <div class="cover-image">
                    <div class="cover cover-normal">

            <img
              class="cover__img js-lazy"
              src="https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/ad369358-e30c-4ade-a597-2a8052d5ad76_carw_4x3x32.png?h=a9459241aeececb47749cedba2a9e26c"
              data-src="https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/ad369358-e30c-4ade-a597-2a8052d5ad76_car_4x3.png?h=ba474e97b53c23a95f5a5b5b2ed11b34"
              data-srcset="https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/ad369358-e30c-4ade-a597-2a8052d5ad76_carw_4x3x640.png?h=ddd38340c15eacf5adf3ae2ef637b071 640w, https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/ad369358-e30c-4ade-a597-2a8052d5ad76_carw_4x3x1280.png?h=a25be59b622b28c991f4a4f7914ebf2e 1280w, https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/ad369358-e30c-4ade-a597-2a8052d5ad76_carw_4x3x1366.png?h=79d8b78da783547458e365d165bf7b29 1366w, https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/ad369358-e30c-4ade-a597-2a8052d5ad76_carw_4x3x1920.png?h=c333ae8ab2f1d3a55d276871254c456c 1920w, https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/ad369358-e30c-4ade-a597-2a8052d5ad76_carw_4x3x2560.png?h=7d9a2674bc484c8018623250747a80b5 2560w, https://pro2-bar-s3-cdn-cf6.myportfolio.com/da48e6dd-1b98-4de7-bc9a-f60ab8610190/ad369358-e30c-4ade-a597-2a8052d5ad76_carw_4x3x5120.png?h=13f49610f5a1c70f728e55aa5e038445 5120w"
              data-sizes="(max-width: 540px) 100vw, (max-width: 768px) 50vw, calc(1200px / 2)"
            >
                              </div>
                </div>
              </div>
            <div class="details-wrap">
              <div class="details">
                <div class="details-inner">
                    <div class="title preserve-whitespace">Meet Ahmed</div>
                </div>
              </div>
            </div>
          </a>
          </section>
              <section class="back-to-top" data-hover-hint="backToTop">
                <a href="#"><span class="arrow">&uarr;</span><span class="preserve-whitespace">Back to Top</span></a>
              </section>
              <a class="back-to-top-fixed js-back-to-top back-to-top-fixed-with-panel" data-hover-hint="backToTop" data-hover-hint-placement="top-start" href="#">
                <svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
                 viewBox="0 0 26 26" style="enable-background:new 0 0 26 26;" xml:space="preserve" class="icon icon-back-to-top">
                <g>
                  <path d="M13.8,1.3L21.6,9c0.1,0.1,0.1,0.3,0.2,0.4c0.1,0.1,0.1,0.3,0.1,0.4s0,0.3-0.1,0.4c-0.1,0.1-0.1,0.3-0.3,0.4
                    c-0.1,0.1-0.2,0.2-0.4,0.3c-0.2,0.1-0.3,0.1-0.4,0.1c-0.1,0-0.3,0-0.4-0.1c-0.2-0.1-0.3-0.2-0.4-0.3L14.2,5l0,19.1
                    c0,0.2-0.1,0.3-0.1,0.5c0,0.1-0.1,0.3-0.3,0.4c-0.1,0.1-0.2,0.2-0.4,0.3c-0.1,0.1-0.3,0.1-0.5,0.1c-0.1,0-0.3,0-0.4-0.1
                    c-0.1-0.1-0.3-0.1-0.4-0.3c-0.1-0.1-0.2-0.2-0.3-0.4c-0.1-0.1-0.1-0.3-0.1-0.5l0-19.1l-5.7,5.7C6,10.8,5.8,10.9,5.7,11
                    c-0.1,0.1-0.3,0.1-0.4,0.1c-0.2,0-0.3,0-0.4-0.1c-0.1-0.1-0.3-0.2-0.4-0.3c-0.1-0.1-0.1-0.2-0.2-0.4C4.1,10.2,4,10.1,4.1,9.9
                    c0-0.1,0-0.3,0.1-0.4c0-0.1,0.1-0.3,0.3-0.4l7.7-7.8c0.1,0,0.2-0.1,0.2-0.1c0,0,0.1-0.1,0.2-0.1c0.1,0,0.2,0,0.2-0.1
                    c0.1,0,0.1,0,0.2,0c0,0,0.1,0,0.2,0c0.1,0,0.2,0,0.2,0.1c0.1,0,0.1,0.1,0.2,0.1C13.7,1.2,13.8,1.2,13.8,1.3z"/>
                </g>
                </svg>
              </a>
        </main>
      </div>
    </div>
  </div>
<script type="text/javascript">window.NREUM||(NREUM={});NREUM.info={"beacon":"bam-cell.nr-data.net","licenseKey":"e7fb1b89a0","applicationID":"750147145","transactionName":"ZwZaYkJVDERXUxULCV5Me0NDQA1aGWsmJzJtQxdtS0QDQ14KT0gbbQ==","queueTime":0,"applicationTime":12,"atts":"S0FNFApPHxsUUUNYHU0e","errorBeacon":"bam-cell.nr-data.net","agent":""}</script></body>
<script type="text/javascript">
  // fix for Safari's back/forward cache
  window.onpageshow = function(e) {
    if (e.persisted) { window.location.reload(); }
  };
</script>
  <script type="text/javascript">var __config__ = {"page_id":"p5f920b4a8480130e52d595d68e722b0673a447939053771b691e7","theme":{"name":"lukas"},"pageTransition":true,"linkTransition":true,"disableDownload":false,"localizedValidationMessages":{"required":"This field is required","Email":"This field must be a valid email address"},"lightbox":{"enabled":true,"color":{"opacity":0.94,"hex":"#fff"}},"cookie_banner":{"enabled":false}};</script>
  <script type="text/javascript" src="/site/translations?cb="></script>
  <script type="text/javascript" src="/dist/js/main.js?cb="></script>
</html>
