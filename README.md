Contents of the documentation

Steps | Title
------------ | -------------
1 | Preparing basic html structure
2 | Adding Scripts and Styles with <head></head> tags
3 | Adding basic styles 
4 | Design Section 1
5 | Design Section 2
6 | Design Section 3

![Image of Section1](https://github.com/iwilfried/Amp-Mag-Sound/blob/master/images/1.PNG)
![Image of Section1](https://github.com/iwilfried/Amp-Mag-Sound/blob/master/images/2.PNG)
### Step 1:Preparing basic html structure
```
<!doctype html>
<html AMP>
<head>
<title> <!-- Give appropriate title to the page  --> </title>
<!-- Required scripts and styles -->
</head>
<body>
<!-- Page contents -->
</body>
</html>
```
### Step 2:Adding Scripts and Styles with ```<head></head>``` tags
```
<meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=Edge"/>
<meta name="viewport" content="width=device-width,minimum-scale=1,initial-scale=1">
<link rel="canonical" href="https://sound-json.firebaseapp.com/">
<script custom-element="amp-font" src="https://cdn.ampproject.org/v0/amp-font-0.1.js" async></script>
<script custom-element="amp-sidebar" src="amp-sidebar-0.1.js" async></script>
<script custom-element="amp-accordion" src="https://cdn.ampproject.org/v0/amp-accordion-0.1.js" async></script>
<script src="https://cdn.ampproject.org/v0.js" async></script>

```

### Step 3:Adding basic styling within ```<style amp-custom></style>``` tags:
```
html{
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased
}
body{
    font-family:Georgia, serif;
    font-size:100%;
    line-height:1.5;
    color:#121212;
    background:rgba(51,51,51,0.05)
}
.main-body{
    background:#ffffff;
    max-width:37.5rem;
    margin:0 auto;
    
    overflow-x:hidden;
}
html,body{
    text-rendering:optimizeSpeed
}
h1,h2,h3,h4,h5,h6{
    margin:0
}
p{
    font-size:1rem;
    font-weight:300;
    margin-top:0;
    margin-bottom:0.5rem;
    text-align: justify;
}
h3{
    font-size:1rem;
    line-height:1.5rem;
    font-weight:normal;
    margin-bottom:0.4375rem
}


a{
    color:#005689;
    cursor:pointer;
    text-decoration:none
}
a:hover,a:focus{
    text-decoration:underline
}
a:active{
    color:#4bc6df;
    text-decoration:none
}

menu,ol,ul{
    padding:0;
    margin-left:1.5625rem
}
nav ul,nav ol{
    list-style:none;
    list-style-image:none
}
.margin-top-14
{
  margin-top:14px;
}
```
# Step 4: Design Section 1
![Image of Section1](https://github.com/iwilfried/Amp-Mag-Sound/blob/master/images/header.PNG)

### Code:
```
 <header class="header">
    <nav>
      <div class="header_position">
        <a class="header_linkstyle" href="">
          <span class="header_drawcircle"></span>
          <span class="header_circletext">
            Read<br>Visit-Angkor<br>Blog</span>
          </span>
        </a>
      </div>
      <a href="" class="header_logo">
        <span class="header_logo">
           <amp-img
  src="img/test.png"
  height="54" width="180" class="margin-top-14"></amp-img>
      </span>
    </a>
    <ul class="ul_nav">
      <li class="li_nav">
        <a class="nav_link special_1" href="#" >
          Greetings
        </a>
      </li>
      <li class="li_nav">
        <a class="nav_link" href="#">
          Food
        </a>
      </li>
      <li class="li_nav">
        <a class="nav_link" href="#">
          Culture
        </a>
      </li>
      <li class="li_nav">
        <a class="nav_link" href="#">
          Lifestyle
        </a>
      </li>
    </ul>
 <script>
function myFunction(x) {
    x.classList.toggle("change");
}
</script>

    
<div class="container12" onclick="myFunction(this)" on='tap:sidebar1.toggle'>
  <div class="bar1"></div>
  <div class="bar2"></div>
  <div class="bar3"></div>
</div>
    

  </nav>
</header>

<amp-sidebar class="menu" layout="nodisplay" id="sidebar1">
 
  <amp-accordion disable-session-states class="top_padding_20">
    <section>
      <h2 class="sidebarstyle padding_120 padding_15">Home</h2>
      <div class="side_menu_5">
        <ul>
          <li class="side_menu_3"><a href="#" class="side_menu_sub_link">Dialog</a></li>
          <li class="side_menu_3"><a href="#" class="side_menu_sub_link">Numbers</a></li>
        </ul>
      </div>
    </section>
    <section>
      <h2 class="sidebarstyle">Service</h2>
      <div class="side_menu_5">
        <ul>
          <li class="side_menu_3"><a href="#" class="side_menu_sub_link">How we Work</a></li>
        </ul>
      </div>
    </section>
    <section>
      <h2 class="sidebarstyle">Portfolio</h2>
      <div class="side_menu_5">
        <ul>
          <li class="side_menu_3"><a href="#" class="side_menu_sub_link">Find Answers Here</a></li>
        </ul>
      </div>
    </section>
    <section>
      <h2 class="sidebarstyle">Contact</h2>
      <div class="side_menu_5">
        <ul>
          <li class="side_menu_3"><a href="#" class="side_menu_sub_link">Article 1</a></li>
          <li class="side_menu_3"><a href="#" class="side_menu_sub_link">Article 2</a></li>
          <li class="side_menu_3"><a href="#" class="side_menu_sub_link">Article 3</a></li>
        </ul>
      </div>
    </section>
  </amp-accordion>

</amp-sidebar>


```
### Create a amp-sidebar-0.1.js file and store it in the same project folder and add the following script to the file:
```
(self.AMP = self.AMP || []).push({
    n: "amp-sidebar",
    v: "1522276799752",
    f: (function(AMP) {
        var h;

        function m(a, b) {
            function d() {}
            d.prototype = b.prototype;
            a.prototype = new d;
            a.prototype.constructor = a;
            for (var c in b)
                if (Object.defineProperties) {
                    var f = Object.getOwnPropertyDescriptor(b, c);
                    f && Object.defineProperty(a, c, f)
                } else a[c] = b[c]
        };

        function n(a) {
            if (!a) return [];
            for (var b = Array(a.length), d = 0; d < a.length; d++) b[d] = a[d];
            return b
        };
        self.log = self.log || {
            user: null,
            dev: null,
            userForEmbed: null
        };
        var p = self.log;

        function q() {
            var a = "\u200b\u200b\u200b";
            throw Error("failed to call initLogConstructor");
        };

        function r(a) {
            this.P = a;
            this.h = Object.create(null)
        }
        r.prototype.get = function(a) {
            if (this.h[a]) return this.h[a].access = Date.now(), this.h[a].payload
        };
        r.prototype.put = function(a, b) {
            var d = this;
            this.h[a] = {
                payload: b,
                access: Date.now()
            };
            var c = Object.keys(this.h);
            if (c.length > this.P) {
                if (p.dev) a = p.dev;
                else throw Error("failed to call initLogConstructor");
                a.warn("lru-cache", "Trimming template cache");
                c.sort(function(a, b) {
                    return d.h[b].access - d.h[a].access
                });
                delete this.h[c[c.length - 1]]
            }
        };
        var t, u;

        function v(a) {
            var b = a.indexOf("#");
            return -1 == b ? a : a.substring(0, b)
        };

        function w(a) {
            if (a.nodeType) {
                var b = (a.ownerDocument || a).defaultView;
                if (b = b != (b.__AMP_TOP || b) && x(b, "action") ? y(b, "action") : null) return b
            }
            return z(a, "action")
        }

        function A(a, b) {
            a = a.__AMP_TOP || a;
            return y(a, b)
        }

        function z(a, b) {
            a = B(a);
            a = B(a);
            a = a.isSingleDoc() ? a.win : a;
            return y(a, b)
        }

        function B(a) {
            return a.nodeType ? A((a.ownerDocument || a).defaultView, "ampdoc").getAmpDoc(a) : a
        }

        function y(a, b) {
            x(a, b);
            var d = a.services;
            d || (d = a.services = {});
            var c = d;
            a = c[b];
            a.obj || (a.obj = new a.ctor(a.context), a.ctor = null, a.context = null, a.resolve && a.resolve(a.obj));
            return a.obj
        }

        function x(a, b) {
            a = a.services && a.services[b];
            return !(!a || !a.ctor && !a.obj)
        };
        /*
         https://mths.be/cssescape v1.5.1 by @mathias | MIT license */
        function C(a, b) {
            for (var d, c = a; c && c !== d; c = c.parentElement)
                if (b(c)) return c;
            return null
        }

        function D(a) {
            var b = "A";
            if (a.closest) return a.closest(b);
            b = b.toUpperCase();
            return C(a, function(a) {
                return a.tagName == b
            })
        }

        function E(a) {
            var b = a.body.getAttribute("dir") || a.documentElement.getAttribute("dir") || "ltr";
            return "rtl" == b
        };
        var F, G = "Webkit webkit Moz moz ms O o".split(" ");

        function H(a, b) {
            var d = void 0;
            if (2 > b.length ? 0 : 0 == b.lastIndexOf("--", 0)) return b;
            F || (F = Object.create(null));
            var c = F[b];
            if (!c || d) {
                c = b;
                if (void 0 === a[b]) {
                    var f = b.charAt(0).toUpperCase() + b.slice(1);
                    a: {
                        for (var g = 0; g < G.length; g++) {
                            var k = G[g] + f;
                            if (void 0 !== a[k]) {
                                f = k;
                                break a
                            }
                        }
                        f = ""
                    }
                    var l = f;
                    void 0 !== a[l] && (c = l)
                }
                d || (F[b] = c)
            }
            return c
        }

        function I(a, b, d) {
            var c;
            (b = H(a.style, b)) && (a.style[b] = c ? d + c : d)
        }

        function J(a, b) {
            if (void 0 === b) {
                var d;
                d = (d = H(a.style, "display")) ? a.style[d] : void 0;
                b = "none" == d
            }
            I(a, "display", b ? "" : "none")
        };

        function K(a, b) {
            function d() {
                c = 0;
                var k = 350 - (a.Date.now() - f);
                if (0 < k) c = a.setTimeout(d, k);
                else {
                    var l = g;
                    g = null;
                    b.apply(null, l)
                }
            }
            var c = 0,
                f = 0,
                g = null;
            return function(b) {
                for (var l = [], e = 0; e < arguments.length; ++e) l[e - 0] = arguments[e];
                f = a.Date.now();
                g = l;
                c || (c = a.setTimeout(d, 350))
            }
        };

        function L(a, b, d) {
            this.c = a;
            this.W = void 0;
            this.m = b;
            this.I = d;
            this.V = this.c.getAttribute("toolbar");
            this.G = null;
            this.l = void 0;
            this.H = !1;
            this.c.classList.add("amp-sidebar-toolbar-target-hidden");
            M(this)
        }
        L.prototype.onLayoutChange = function(a) {
            var b = this.I.win.matchMedia(this.V).matches;
            if (b) {
                var d = N(this);
                d && d.then(a)
            } else O(this)
        };

        function M(a) {
            a.G = a.c.cloneNode(!0);
            p.user || (p.user = q());
            var b = p.user.assert(a.c.getAttribute("toolbar-target"), '"toolbar-target" is required', a.c);
            a.I.whenReady().then(function() {
                var d = a.I.getElementById(b);
                if (d) a.l = d, a.G.classList.add("i-amphtml-toolbar"), J(a.l, !1);
                else throw Error("Could not find the toolbar-target element with an id: " + b);
            })
        }

        function N(a) {
            if (!a.H) return a.m.mutatePromise(function() {
                a.l && (J(a.l, !0), a.l.contains(a.G) || a.l.appendChild(a.G), a.c.classList.add("amp-sidebar-toolbar-target-shown"), a.c.classList.remove("amp-sidebar-toolbar-target-hidden"), a.H = !0)
            })
        }

        function O(a) {
            a.H && a.m.mutate(function() {
                a.l && (J(a.l, !1), a.c.classList.add("amp-sidebar-toolbar-target-hidden"), a.c.classList.remove("amp-sidebar-toolbar-target-shown"), a.H = !1)
            })
        };

        function P(a) {
            a = AMP.BaseElement.call(this, a) || this;
            a.w = null;
            a.m = A(a.win, "vsync");
            a.K = null;
            a.A = null;
            a.o = a.win.document;
            a.R = a.o.documentElement;
            a.B = null;
            a.O = [];
            var b = A(a.win, "platform");
            a.N = b.isIos();
            a.S = b.isSafari();
            a.D = -1;
            a.L = !1;
            a.X = null;
            a.C = K(a.win, a.T.bind(a));
            a.J = null;
            a.M = 0;
            return a
        }
        m(P, AMP.BaseElement);
        h = P.prototype;
        h.isLayoutSupported = function(a) {
            return "nodisplay" == a
        };
        h.buildCallback = function() {
            var a = this;
            this.element.classList.add("i-amphtml-overlay");
            this.B = this.element.getAttribute("side");
            this.w = this.getViewport();
            this.K = w(this.element);
            "left" != this.B && "right" != this.B && (this.B = E(this.o) ? "right" : "left", this.element.setAttribute("side", this.B));
            var b = this.getAmpDoc(),
                d = n(this.element.querySelectorAll("nav[toolbar]"));
            d.forEach(function(d) {
                try {
                    a.O.push(new L(d, a.m, b))
                } catch (k) {
                    a.user().error("amp-sidebar toolbar", "Failed to instantiate toolbar", k)
                }
            });
            this.N &&
                Q(this);
            R(this) ? this.F() : this.element.setAttribute("aria-hidden", "true");
            this.element.hasAttribute("role") || this.element.setAttribute("role", "menu");
            this.element.tabIndex = -1;
            this.R.addEventListener("keydown", function(b) {
                27 == b.keyCode && a.j()
            });
            var c = this.element.getAttribute("data-close-button-aria-label") || "Close the sidebar",
                f = this.o.createElement("button");
            f.textContent = c;
            f.classList.add("i-amphtml-screen-reader");
            f.tabIndex = -1;
            f.addEventListener("click", function() {
                a.j()
            });
            this.element.appendChild(f);
            this.registerAction("toggle", this.U.bind(this));
            this.registerAction("open", this.F.bind(this));
            this.registerAction("close", this.j.bind(this));
            this.element.addEventListener("click", function(b) {
                if ((b = D(b.target)) && b.href) {
                    var d;
                    d = b.href;
                    t || (t = self.document.createElement("a"), u = self.UrlCache || (self.UrlCache = new r(100)));
                    var c = u.get(d);
                    if (c) d = c;
                    else {
                        c = t;
                        c.href = d;
                        c.protocol || (c.href = c.href);
                        var e = {
                            href: c.href,
                            protocol: c.protocol,
                            host: c.host,
                            hostname: c.hostname,
                            port: "0" == c.port ? "" : c.port,
                            pathname: c.pathname,
                            search: c.search,
                            hash: c.hash,
                            origin: null
                        };
                        "/" !== e.pathname[0] && (e.pathname = "/" + e.pathname);
                        if ("http:" == e.protocol && 80 == e.port || "https:" == e.protocol && 443 == e.port) e.port = "", e.host = e.hostname;
                        e.origin = c.origin && "null" != c.origin ? c.origin : "data:" != e.protocol && e.host ? e.protocol + "//" + e.host : e.href;
                        u.put(d, e);
                        d = e
                    }
                    var f = d,
                        g = a.getAmpDoc().win.location.href;
                    v(b.href) == v(g) && f.hash && a.j()
                }
            }, !0);
            this.element.addEventListener("transitionend", this.C);
            this.element.addEventListener("animationend", this.C)
        };
        h.activate = function(a) {
            this.F(a)
        };
        h.onLayoutMeasure = function() {
            var a = this;
            this.getAmpDoc().whenReady().then(function() {
                a.O.forEach(function(b) {
                    b.onLayoutChange(function() {
                        a.j()
                    })
                })
            })
        };

        function R(a) {
            return a.element.hasAttribute("open")
        }
        h.U = function(a) {
            R(this) ? this.j() : this.F(a)
        };
        h.F = function(a) {
            var b = this;
            R(this) || (this.w.enterOverlayMode(), this.m.mutate(function() {
                J(b.element, !0);
                b.w.addToFixedLayer(b.element, !0);
                b.N && b.S && S(b);
                b.element.scrollTop = 1;
                b.m.mutate(function() {
                    T(b);
                    b.element.setAttribute("open", "");
                    b.C();
                    b.element.setAttribute("aria-hidden", "false")
                })
            }), z(this.getAmpDoc(), "history").push(this.j.bind(this)).then(function(a) {
                b.D = a
            }), a && (this.J = a.caller, this.M = this.w.getScrollTop()))
        };
        h.j = function() {
            var a = this;
            if (R(this)) {
                this.w.leaveOverlayMode();
                var b = this.M == this.w.getScrollTop(),
                    d = this.element.contains(this.o.activeElement);
                this.m.mutate(function() {
                    a.A && J(a.A, !1);
                    a.element.removeAttribute("open");
                    a.C();
                    a.element.setAttribute("aria-hidden", "true")
                }); - 1 != this.D && (z(this.getAmpDoc(), "history").pop(this.D), this.D = -1);
                if (this.J && d && b) try {
                    this.J.focus()
                } catch (c) {}
            }
        };

        function T(a) {
            if (!a.A) {
                var b = a.o.createElement("div");
                b.classList.add("i-amphtml-sidebar-mask");
                b.addEventListener("click", function() {
                    a.j()
                });
                a.element.ownerDocument.body.appendChild(b);
                b.addEventListener("touchmove", function(a) {
                    a.preventDefault()
                });
                a.A = b
            }
            J(a.A, !0)
        }

        function Q(a) {
            a.element.addEventListener("scroll", function(b) {
                R(a) && (1 > a.element.scrollTop ? (a.element.scrollTop = 1, b.preventDefault()) : a.element.scrollHeight == a.element.scrollTop + a.element.offsetHeight && (--a.element.scrollTop, b.preventDefault()))
            })
        }

        function S(a) {
            if (!a.L) {
                var b = a.o.createElement("div"),
                    d = {
                        height: "10vh",
                        width: "100%",
                        "background-color": "transparent"
                    },
                    c;
                for (c in d) I(b, c, d[c]);
                a.element.appendChild(b);
                a.L = !0
            }
        }
        h.T = function() {
            var a = this;
            if (R(this)) {
                var b = this.getRealChildren();
                this.scheduleLayout(b);
                this.scheduleResume(b);
                try {
                    this.element.focus()
                } catch (d) {}
                U(this, "sidebarOpen")
            } else this.m.mutate(function() {
                J(a.element, !1);
                a.schedulePause(a.getRealChildren());
                U(a, "sidebarClose")
            })
        };

        function U(a, b) {
            var d;
            var c = a.win;
            d = "amp-sidebar toolbar." + b;
            var f = {},
                g = {
                    detail: f
                };
            Object.assign(g, void 0);
            "function" == typeof c.CustomEvent ? d = new c.CustomEvent(d, g) : (c = c.document.createEvent("CustomEvent"), c.initCustomEvent(d, !!g.bubbles, !!g.cancelable, f), d = c);
            a.K.trigger(a.element, b, d, 100)
        }(function(a) {
            a.registerElement("amp-sidebar", P, "amp-sidebar{position:fixed!important;top:0;max-height:100vh!important;height:100vh;max-width:92vw!important;background-color:#efefef;min-width:45px!important;outline:none;overflow-x:hidden!important;overflow-y:auto!important;-webkit-overflow-scrolling:touch;will-change:transform}amp-sidebar[side=left]{left:0!important;-webkit-transform:translateX(-100%)!important;transform:translateX(-100%)!important}amp-sidebar[side=right]{right:0!important;-webkit-transform:translateX(100%)!important;transform:translateX(100%)!important}amp-sidebar[side][open]{-webkit-transform:translateX(0)!important;transform:translateX(0)!important}amp-sidebar[side]{-webkit-transition:-webkit-transform 233ms cubic-bezier(0,0,.21,1);transition:-webkit-transform 233ms cubic-bezier(0,0,.21,1);transition:transform 233ms cubic-bezier(0,0,.21,1);transition:transform 233ms cubic-bezier(0,0,.21,1),-webkit-transform 233ms cubic-bezier(0,0,.21,1)}.i-amphtml-toolbar>ul{display:-webkit-box;display:-ms-flexbox;display:flex;-webkit-box-pack:start;-ms-flex-pack:start;justify-content:flex-start;-ms-flex-wrap:wrap;flex-wrap:wrap;overflow:auto;list-style-type:none;padding:0;margin:0}.i-amphtml-sidebar-mask{position:fixed!important;top:0!important;left:0!important;width:100vw!important;height:100vh!important;opacity:0.2;background-image:none!important;background-color:#000;}\n/*# sourceURL=/extensions/amp-sidebar/0.1/amp-sidebar.css*/")
        })(self.AMP);
    })
});
//# sourceMappingURL=amp-sidebar-0.1.js.map
```
### Add classes within ```<style amp-custom></style>``` tags:
```
 .header{
    background-color:#e9eff1;
    border-bottom:0.0625rem solid #abc2c9;
    color:#121212;
    position:relative;
    max-width:37.5rem;
    margin:0 auto
  }
.header_position{
    left:-0.625rem;
    position:absolute;
    top:0
  }
  @media (min-width: 30em){
    .header_position{
      left:0
    }
  }
.header_linkstyle{
    color:#e9eff1
  }
.header_drawcircle{
    bottom:-0.75rem;
    left:0;
    overflow:hidden;
    position:absolute;
    right:0;
    top:0;
    -webkit-transition:-webkit-transform 250ms ease-out;
    transition:-webkit-transform 250ms ease-out;
    transition:transform 250ms ease-out;
    transition:transform 250ms ease-out, -webkit-transform 250ms ease-out;
    -webkit-transform-origin:top center;
    transform-origin:top center
  }
  .header_drawcircle:before{
    background:#121212;
    -webkit-border-radius:50%;
    border-radius:50%;
    bottom:0;
    content:'';
    display:block;
    left:0;
    padding-top:100%;
    position:absolute;
    right:0
  }
  .header_circletext{
    -webkit-box-sizing:border-box;
    -moz-box-sizing:border-box;
    box-sizing:border-box;
    display:block;
    padding:0.5625rem 1.25rem 0.1875rem;
    position:relative;
    font-size:0.8125rem;
    line-height:1.2;
    text-align:center;
    font-weight: bold;
  }
 .header_logo{
    display:-webkit-box;
    display:-webkit-flex;
    display:-ms-flexbox;
    display:flex;
    float:none;
    margin-left:auto;
    margin-bottom: 9px;
  }
  .ul_nav{
    height:1.875rem;
    margin:0;
    padding:0 0.625rem
  }
  @media (min-width: 30em){
    .ul_nav{
      padding-left:1.25rem;

    }
  }
 .li_nav{
    display:block;
    float:left;
    font-weight:500;
    font-family: Roboto;
  }
  .li_nav:first-child .nav_link{
    padding-left:0;
    
  }
  .li_nav:first-child .nav_link:before{
    content:none
  }
  .li_nav:nth-child(1){
    color:#c70000;
  }
  .li_nav:nth-child(2){
    color:#e05e00;
  }
  .li_nav:nth-child(3){
    color:#0084c6
  }
  .li_nav:nth-child(4){
    color:#bb3b80
  }
  .li_nav:nth-child(5){
    color:#bb3b80
  }
.nav_link{

    font-size:0.9375rem;
    font-weight:900;
    display:block;
    height:1.875rem;
    /*line-height:1;*/
    padding:0 0.55rem;
    position:relative;
    color:currentColor;
    cursor:pointer
  }
  @media (min-width: 22.5em){
    .nav_link{
     /* font-size:1rem*/
   }
 }
 .nav_link:before{
  content:'';
  display:block;
  left:0;
  bottom:0;
  position:absolute;
  border-left:0.0625rem solid #abc2c9;
  top:0.1875rem
}
.special_1
{
  border-bottom-color: #c70000;
  border-bottom-width: 3px;
  border-bottom-style: solid;
  display: inline;
  padding-bottom: 6px;
}
.bar1, .bar2, .bar3 {
    width: 21px;
    height: 3px;
    background-color: #fff;
    margin: 4px auto;
    transition: 0.4s;
    text-align: center;
}

.change .bar1 {
    -webkit-transform: rotate(-42deg) translate(-4px, 4px);
    transform: rotate(-42deg) translate(-4px, 4px);
}

.change .bar2 {opacity: 0;}

.change .bar3 {
    -webkit-transform: rotate(42deg) translate(-5px, -6px);
    transform: rotate(42deg) translate(-5px, -6px);
}

.container12 {
    display: inline-block;
    cursor: pointer;
    background-color: black;
    height: 45px;
    width: 45px;
    border-radius: 50%;
    float: right;
    position: absolute;
    right: 6px;
    top: 76px;
    padding-top: 9px;
    box-sizing: border-box;
    z-index: 1000;
}
.top_padding_20 {
 margin-top: 20px;
}
.sidebarstyle
  {
    font-family:Roboto;
    text-align:center;
    background-color:#385574;
    color:white;
    border:none;
    font-weight: 100;
    font-weight:300;
    font-size:45px;
  }
  .padding_15 {
    padding-left: 15px;
}
.side_menu_5 {
 background-color:lightgray;
}
.side_menu_3 {
 list-style: none;
 margin-bottom: 8px;
}
.side_menu_sub_link{
 text-decoration: none;
 color:black;
 font-weight:100;
}
amp-sidebar.menu{
  background-color:#385574;
  color:white;
  width:100vw;
  z-index: 100;
}
.menu div:first-of-type{
  overflow-y:scroll
}
<style amp-boilerplate>body{-webkit-animation:-amp-start 8s steps(1,end) 0s 1 normal both;-moz-animation:-amp-start 8s steps(1,end) 0s 1 normal both;-ms-animation:-amp-start 8s steps(1,end) 0s 1 normal both;animation:-amp-start 8s steps(1,end) 0s 1 normal both}@-webkit-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@-moz-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@-ms-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@-o-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}</style><noscript><style amp-boilerplate>body{-webkit-animation:none;-moz-animation:none;-ms-animation:none;animation:none}</style></noscript>
```
# Step 5: Design Section 2

![Image of Section 2](https://github.com/iwilfried/Amp-Mag-Sound/blob/master/images/test.PNG)

### Code:
```
<div class="main-body">
  <div class="side-margins">
    <article id="article">
      <header>
        <div class="content__header">
          <div class="container">

            <div>
              <a href="#" class="side_menu_sub_link_1">Fashion</a>
              <a href="#" class="side_menu_sub_link_1">Food</a>
              <a href="#" class="side_menu_sub_link_1">Recipes</a>
              <a href="#" class="side_menu_sub_link_1">Love & Sex</a>
              <span [class]="visible ? 'show' : 'hide'" class="hide">
            <hr class="style1">
            
              <a href="#" class="side_menu_sub_link_1">Health & fitness</a>
              <a href="#" class="side_menu_sub_link_1">Home & garden</a>
              <a href="#" class="side_menu_sub_link_1">Women</a>
            
            <hr class="style1">
            
              <a href="#" class="side_menu_sub_link_1">Family</a>
              <a href="#" class="side_menu_sub_link_1">Travel</a>
              <a href="#" class="side_menu_sub_link_1">Money</a>
           
             </span>
               <a [class]="visible ? 'pink' : 'gray'" [text]="visible ? 'Less' : 'More'" on="tap:AMP.setState({visible: !visible})" class="side_menu_sub_link_1 gray">More</a>
            </div>

  
            <hr class="style1">
            <hr class="style1">
            <hr class="style1">
            <hr class="style1">

```
### Add External fontawesome stylesheet inside the ```<head></head>``` tags:
```
 <link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet" integrity="sha384-wvfXpqpZZVQGK6TAh5PVlGOfQNHSoD2xbE+QkPxCAFlNEevoEH3Sl0sibVcOQVnN" crossorigin="anonymous">
 
```
### Add classes within ```<style amp-custom></style>``` tags:
```
.main-body{
    background:#ffffff;
    max-width:37.5rem;
    margin:0 auto;
    overflow-x:hidden;
  }
.side-margins
{
  margin-left: 0px;
}

.content__header{
  background-image:-webkit-repeating-linear-gradient(top, #dcdcdc, #dcdcdc 0.0625rem, transparent 0.0625rem, transparent 0.25rem);
  background-image:repeating-linear-gradient(to bottom, #dcdcdc, #dcdcdc 0.0625rem, transparent 0.0625rem, transparent 0.25rem);
  background-repeat:repeat-x;
  background-position:bottom;
  -webkit-background-size:0.0625rem 1.8125rem;
  background-size:0.0625rem 1.8125rem
}
.container
{
 padding-left:0.625rem;
 padding-right:0.625rem;
 -webkit-box-sizing:border-box;
 -moz-box-sizing:border-box;
 box-sizing:border-box
}
.side_menu_sub_link_1
{  
 padding-top: 10px;
 padding-left: 5px;
 display:inline-block;
 color:#000;
 font-family: Roboto;
 font-weight: bold;
}
hr.style1
{
  border-top: 1px solid #8c8b8b85;
  margin-bottom: -6px;
  margin-left: -11px;
  margin-right: -11px;
}
.pink
  {
    padding-top: 10px;
    padding-left: 10px;
    display: inline-block;
    font-family: Roboto;
    font-weight: bold;
    color:#bb3b80;
    text-decoration: none;
  }
  .gray
  {
    padding-top: 10px;
    padding-left: 10px;
    display: inline-block;
    font-family: Roboto;
    font-weight: bold;
    color:gray;
    text-decoration: none;
    
  }
  .gray:after
  {
    padding-top: 0px;
    padding-left: 3px;
    display: inline-block;
    color:gray;
    text-decoration: none;
    content:'\f107';
    font-family: Fontawesome; 
    font-size:20px; 
  }
```
# Step 6: Design Section 3

![Image of Section 2](https://github.com/iwilfried/Amp-Mag-Sound/blob/master/images/content.PNG)

### Code:
```
             <!-- sound card -->
            <div class="tabs-content">
              <amp-selector role="tablist" layout="container" class="" style="">

                <div role="tab" class="tabButton" selected option="a">Home</div>
                <div role="tabpanel" class="tabContent">
                  <div class="tint-block tint-block-top bg-body-1 home-card">
                    <div class="tint bg-red-light">

                      <div class="tint-position">
                        <h1 class="tint-header">
                          GREETINGS
                        </h1>
                        <span class="tint-span">
                          PRESENTING SAMPEAH IS A SIGN OF RESPECT AND POLITENESS.
                        </span>

                      </div>
                    </div>
                  </div>

                  <div class="content page-content-card page-content-card-bottom">
                    <h4 class="icon-heading uppercase ultrabold half-bottom">SAMPEAH</h4>
                    <p>
                      Sampeah is either used when you want to greet ( in KhmerL ->ផ៣បសវ joom reab sour) somebody or when you want to say goodbye (in Khmer:ផ៣បសវ ->joom reab lea). First of all, we need to place our both palms together like a lotus flower in front of our chest. Both are the formal way to gret and to say goodbye.
                      <amp-img alt="" src="img/s-07.png" height="145px"></amp-img>
                    </p>

                    <amp-list width="auto"
                    height="1790"
                    layout="fixed-height"
                    src="https://sound-json.firebaseapp.com/json/audio.json">
                    <template type="amp-mustache">
 
    <div id="widget" class="widget g-background-default g-shadow-inset">
      <p class="p1-text">{{title1}}</p>
      <p class="p2-text">{{title2}}</p>
      <p class="p3-text">{{title3}}</p>
      <p class="p4-text">{{title4}}</p>
      <div class="audio-container">
        <amp-audio  class="audio-player" width="auto" height="50" 
        src="{{url}}"  controlsList="nodownload" >
        <div fallback>
          <p>Your browser doesn’t support HTML5 audio</p>
        </div>
      </amp-audio>
    </div>
  </div>

</template>
</amp-list>
<div class="decoration"></div>
</div>      
</div>
</amp-selector>
</div>
<!-- sound card -->
</div>
</div>

</header>
</article>

</div>
</div>
```
### Add classes within ```<style amp-custom></style>``` tags:
```
 .tabs-content
  {
    padding-top:10px;
    margin:-10px;
  }

  .tabButton[selected] {
    display: none;
  }

  .tabButton {
    display: none;
  }
  .tabContent {
    display: none;
    width: 100%;
    order: 1; 
    border: 1px solid #ccc;
    padding: 5px;
    line-height: 24px;
  }

  .tabButton[selected]+.tabContent {
    display: block;
  }
.tint-block .tint{
    position:absolute;
    top:0px;
    left:0px;
    right:0px;
    bottom:0px;
    /* opacity:0.7;*/
    z-index:3;
    width:115%;
    height: 380px;
    background-image: linear-gradient( rgba(255, 0, 0, 0.49), rgba(195, 78, 63, 1) ),url(img/bg1.jpg);
    background-repeat:no-repeat;
    background-size:cover;
    background-position-x: -36px;
    background-position-y: -59px;

  }
  .tint-block{background-size:cover;}
.bg-body-1{background-position:150px right;}
  .tint-block-top{padding: 50px 0px 120px 0px;}
.home-card{
    padding: 260px 0px 120px 0px;
  }
.bg-red-light{background-color: #e74c3c; color:#FFFFFF;}
.tint-position
  {
    padding-top: 127px;padding-left: 17px;
  }
 .tint-header
  {
   font-family:Roboto;
   margin-top: -56px;
   margin-bottom: 12px;
   font-weight: 900;
 }

.tint-span
  {
    font-family: Roboto;
    font-size: 12px;
    float: left;
    width: 143px;
    font-weight: bold;
  }

  .page-content-card{
    font-family: Roboto;
    z-index: 97;
    position: relative;
    background-color: #fefefe;
    margin-left: 5px;
    margin-right: 16px;
    padding-top: 20px;
    padding-left: 10px;
    padding-right: 10px;
    /* border: solid 1px rgba(0,0,0,0.1); */
    margin-top: -169px;
    box-shadow: 0px 2px 5px 0px rgba(0,0,0,0.05);
  }

.uppercase{text-transform: uppercase;}
.ultrabold{font-weight:800;}

.half-bottom{margin-bottom: 3px;
  margin-top: -10px;}
p{
    line-height:20px; 
    font-weight:400; 
    color:#666666; 
    font-size:16px; 
    margin-bottom:15px;

  }
  .widget {
    width: 79%;
    background-repeat: no-repeat;
    background-position: 50%;
    background-size: 100px 60px;
    border-radius: 4px;
    border: 1px solid #e5e5e5;
    overflow: hidden;
    margin-bottom: 5%;
    margin-left: 8%;
  }
.g-background-default {
    background-color: #f5f5f5;
  }
  .g-shadow-inset {
    box-shadow: inset 0 0 0 1px hsla(0,0%,100%,.5);
  }

  .p1-text{
    font-size: 17px;
    padding: 20px 20px 0px;
    margin: auto;
    line-height: 1px;
  }
.audio-container{
    padding: 20px 20px;
  }
.decoration{
    height:1px; 
    background-color:rgba(0,0,0,0.1);
  }





```
### Add script and Roboto Font link for sound integration in the ```<head></head>``` section:
```
<script async custom-element="amp-audio" src="https://cdn.ampproject.org/v0/amp-audio-0.1.js"></script>
  <script async custom-element="amp-list" src="https://cdn.ampproject.org/v0/amp-list-0.1.js"></script>
  <script async custom-template="amp-mustache" src="https://cdn.ampproject.org/v0/amp-mustache-0.1.js"></script>
<link href='http://fonts.googleapis.com/css?family=Roboto:400,100,100italic,300,300italic,400italic,500,500italic,700,700italic,900italic,900' rel='stylesheet' type='text/css'>
```
