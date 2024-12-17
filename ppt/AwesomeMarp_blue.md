---
marp: true
size: 16:9
theme: am_blue
paginate: true
headingDivider: [2,3]
footer: \ 大数据原理与技术小组作业
style: |
    section.pin-3-change1 {
    overflow: visible;
    display: grid;
    gap: 1rem;
    grid-template-rows: 7% 20% 73%;
    grid-template-columns: 50% 50%;
    grid-template-areas:
        "slideheading slideheading"
        "toppanel  toppanel"
        "leftpanel rightpanel";
    }
    section.pin-3-change1 h2, section.pin-3-change1 h3 {
    grid-area: slideheading;
    font-size: var(--font-size-2-3);
    }
    section.pin-3-change1 .tdiv { 
    grid-area: toppanel; 
    }
    section.pin-3-change1 .ldiv { 
    grid-area: leftpanel; 
    }
    section.pin-3-change1 .rdiv { 
    grid-area: rightpanel; 
    }
    section.pin-3-change1 .timg { 
    grid-area: toppanel; 
    display: flex;
    align-items: center;  
    justify-content: center;
    }
    section.pin-3-change1 .limg { 
    grid-area: leftpanel;
    display: flex;
    align-items: center;  
    justify-content: center;
    }
    section.pin-3-change1 .rimg { 
    grid-area: rightpanel;
    display: flex;
    align-items: center;  
    justify-content: center;
    }

    section.pin-3-change2 {
    overflow: visible;
    display: grid;
    gap: 1rem;
    grid-template-rows: 7% 13% 80%;
    grid-template-columns: 50% 50%;
    grid-template-areas:
        "slideheading slideheading"
        "toppanel  toppanel"
        "leftpanel rightpanel";
    }
    section.pin-3-change2 h2, section.pin-3-change2 h3 {
    grid-area: slideheading;
    font-size: var(--font-size-2-3);
    }
    section.pin-3-change2 .tdiv { 
    grid-area: toppanel; 
    }
    section.pin-3-change2 .ldiv { 
    grid-area: leftpanel; 
    }
    section.pin-3-change2 .rdiv { 
    grid-area: rightpanel; 
    }
    section.pin-3-change2 .timg { 
    grid-area: toppanel; 
    display: flex;
    align-items: center;  
    justify-content: center;
    }
    section.pin-3-change2 .limg { 
    grid-area: leftpanel;
    display: flex;
    align-items: center;  
    justify-content: center;
    }
    section.pin-3-change2 .rimg { 
    grid-area: rightpanel;
    display: flex;
    align-items: center;  
    justify-content: center;
    }

    section.cols-2-change1 {
    overflow: visible;
    display: grid;
    gap: 1.5rem;
    grid-template-columns: 60% 40%;
    grid-template-rows: 10% 90%;
    grid-template-areas:
        "slideheading slideheading"
        "leftpanel    rightpanel";
    }

    section.cols-2-change1 h2, section.cols-2-change1 h3 {
    grid-area: slideheading;
    font-size: var(--font-size-2-3);
    }

    section.cols-2-change1 .ldiv { 
    grid-area: leftpanel; 
    margin-top: -5%;
    }
    section.cols-2-change1 .rdiv { 
    grid-area: rightpanel; 
    margin-top: -5%;
    }
    section.cols-2-change1 .limg { 
    grid-area: leftpanel; 
    margin-top: -5%;
    display: flex;
    align-items: center;  
    justify-content: center;
    }
    section.cols-2-change1 .rimg { 
    grid-area: rightpanel; 
    margin-top: -5%;
    display: flex;
    align-items: center;  
    justify-content: center;
    }

---

<style>
/* @theme am_template */

@charset "UTF-8";
@import 'default';
@import 'https://cdn.bootcdn.net/ajax/libs/font-awesome/6.4.0/css/all.min.css';
@import url(https://fonts.bunny.net/css?family=charm:700);
@auto-scaling true;


:root{
  --font-family-main: 'Latin Modern Math','Adobe Garamond','方正宋刻本秀楷简体','Calibri','楷体','华文中宋','楷体','霞鹜文楷 屏幕阅读版';  
  --font-family-title: 'Optima LT Medium','Arial','方正苏新诗柳楷简体','黑体'; 
  --font-family-footer: 'Charm','Calibri','叶根友毛笔行书修正版','方正苏新诗柳楷简体','楷体';
  --font-family-code: 'Fira Code','HYMingChanKeBen W','Consolas','霞鹜文楷等宽','华文中宋','宋体';
  --font-size-1: 55px;
  --foot-size-subtitle: 42px;
  --font-size-2-3: 38px; 
  --font-size-4-5: 30px; 
  --font-size-main: 25px;
  --font-size-footer: 22px;
  --font-size-page: 12px;
  --font-size-code: 22px;
}



section {
  font-family: var(--font-family-main);
  font-size: var(--font-size-main);
  color: var(--color-main);
  text-align: justify; 
  }

h1 {
  font-family: var(--font-family-title); 
  font-size: var(--font-size-1);
  color: var(--color-title);   
}  


h2,h3 {
  font-family: var(--font-family-title); 
  font-size: var(--font-size-2-3);
  color: var(--color-much);
}

h4, h5 {
  font-family: var(--font-family-title); 
  font-size: var(--font-size-4-5);
  color: var(--color-much);
}

header {
  top: 12px;
}

ol {
  line-height: 1.4rem;
  padding-left: 35px; 
}
ol li::marker {
  color: var(--color-much);
}
ul {
  line-height: 1.4rem;
  padding-left: 35px; 
}


ul>li>ul>li {
  font-size: 0.9rem;
}
ul>li>ul>li>ul>li {
  font-size: 0.85rem;
}

ul.a {
  list-style-type:disc;
}
ul.b {
  list-style-type:circle;
}
ul.c {
  list-style-type:square;
}
ul li::marker {
  color: var(--color-much);
}

blockquote {
  border-left: 8px solid var(--color-much);
  padding: 10px 25px;
  border-radius: 8px;
  background-color: var(--color-quote);
  font-size: 0.9rem;
  font-family: var(--font-family-main);
}

blockquote strong {
  font-family: var(--font-family-main);
}

blockquote>p::before {
  color: var(--color-much);
  padding-right: 2%;
  content: "\f10d"; 
  font-family: "FontAwesome";
}

a {
  font-size: 0.9rem;
  padding:0 .2rem;
  color: var(--color-main);
  font-family: var(--font-family-main);
}
a:hover {
  color: var(--color-much);
  text-decoration: underline;  
}
a::after {
  font-size: 0.6em;
  padding-left: 0.5%;
  content: "\f148"; /* f148 f0c1 f08e f14c f0c6 */
  font-family: "FontAwesome";
  color: var(--color-much);
}

section::after {
  font-family: "FontAwesome";
  font-size: var(--font-size-page);
  margin-right: -10px;
  margin-bottom: -14px;
  content: attr(data-marpit-pagination) "\f101 " attr(data-marpit-pagination-total); 
  letter-spacing: 3px;
  padding: 4px 10px;
  border-radius: 5px;
  border: 1px solid var(--color-footer);
  color: var(--color-footer);
}

footer{
  color: var(--color-footer);
  bottom: 1%;
  left: 2%;
  width: 100%;
  height: 4%;
  display: flex;
  justify-content: space-between;
}

footer>em {
  font-family: var(--font-family-footer);
  font-size: var(--font-size-footer);
  letter-spacing: 1px;
  font-style: normal;
}

footer::after {
  content: "";
}

.MathJax { 
  font-size: 0.95rem;
}

h2 .MathJax, h3 .MathJax, h4 .MathJax, h3 .MathJax {
  font-size: 1.5rem;
}

h4 .MathJax, h5 .MathJax {
  font-size: 1.2rem;
}

pre {
  text-align: left;
  border: 0.3px solid var(--color-few);
  border-radius: 10px;
  padding: 28px;
  line-height: 115%;
  overflow: auto;  
  font-size: var(--font-size-footer);
  font-size: 0.9rem;
}

*::-webkit-scrollbar {
  width: 3px;
  height: 3px;
}
*::-webkit-scrollbar-track {
  border-radius: 3px;
  background-color: #f6f8fa;  
}
*::-webkit-scrollbar-track:hover {
  background-color: var(--color-few);
}
*::-webkit-scrollbar-track:active {
  background-color: var(--color-few);
}
*::-webkit-scrollbar-thumb {
  border-radius: 3px;
  background-color: var(--color-few);
}
*::-webkit-scrollbar-thumb:hover {
  background-color: var(--color-few);
}
*::-webkit-scrollbar-thumb:active {
  background-color: var(--color-few);
}
  
code {
  padding: 2px;
  border-radius: 1px;
  background-color: var(--color-code-bg);
  font-family: var(--font-family-code);
  font-size: 0.8rem;
  letter-spacing: -1px;
}

strong {
  font-size: 1.03rem;
  font-weight: bolder;
  color: var(--color-much);
}
st {
  font-size: 0.9rem;
  font-style: normal;
}
em {
  font-size: 0.9rem;
  font-style: italic;
}
ins {
  text-decoration-color: var(--color-much);
}

img {
  max-width: 95% ;
  border-radius: 8px;
  margin: auto;
}

img[alt*='#l'] {
    float: left;
}
img[alt*='#r'] {
    float: right;
}
img[alt*='#c'] {
    display: block;
    margin: auto;
}


section.cover_a {
  width: 100%;
  background: linear-gradient(to bottom, var(--color-coverbg) 60%, white 40%);
  text-align:center; 
}

section.cover_a h1 {
  background-color: var(--color-coverbg);
  vertical-align:middle;   
  padding: 0px 80px;
  top: 28%;
  width: 88%;
  transform: translateX(-6%);
  position: absolute;  
}

section.cover_a h6 {
  font-family: var(--font-family-title);
  font-size: var(--foot-size-subtitle);
  color: var(--color-title);
  padding: 0px 80px;
  top: 38%;
  width: 90%;
  transform: translateX(-6%);
  position: absolute;  
} 

section.cover_a p {
  bottom: 8%;
  width: 100%;
  transform: translateX(-6%);
  position: absolute;
  justify-content: center;
  align-items: center;
}

section.cover_a strong {
  color: var(--color-main);
}

section.cover_a a::after {
  content: "";
}


section.cover_e {
  width: 100%;
  background: linear-gradient(108deg, white 70%,  var(--color-coverbg) 30%);
  text-align: left; 
}

section.cover_e h1 {
  top: 28%;
  width: 70%;
  transform: translateX(-1.2%);
  position: absolute;    
  color: var(--color-much);
}

section.cover_e h6 {
  font-family: var(--font-family-title);
  font-size: var(--foot-size-subtitle);
  color: var(--color-much);
  top: 38%;
  width: 68%;
  position: absolute;
} 

section.cover_e p {
  bottom: 15%;
  transform: translateX(5%);
  justify-content: center;
  align-items: center;
  position: absolute;
}

section.cover_e strong {
  color: var(--color-main);
}

section.cover_e footer>img {
  transform: scale(1.2);
  background-color: rgba(255, 255, 255, 0);
  background-blend-mode: lighten;
  filter: brightness(2000%) grayscale(60%);
} 

section.cover_e header>img {
  transform: scale(0.88);
  background-color: rgba(255, 255, 255, 0);
  background-blend-mode: lighten;
  filter: brightness(3000%) grayscale(100%);
} 

section.cover_e a::after {
  content: "";
}

section.cover_e footer{
  height: 128px;
  width: 26%;
  padding-bottom: 0px;
  padding-left: 0px;
  left: 72%;
  bottom: 0px;
}

section.cover_e header {
  background-color: var(--color-coverbg); 
  height: 100px; 
  width: 100px;
  top: 0px;
  left: 80px;
  text-align: center;
  vertical-align:middle; 
}


section.cover_b h1 {
  background-color: var(--color-coverbg);
  padding: 30px;
  width: auto;
  height: 26%;
  top: 15%;
  right: 5%; 
  left: 5%;
  position: absolute;
  text-align: center; 
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 20px;
}

section.cover_b h6 {
  font-family: var(--font-family-title);
  font-size: var(--foot-size-subtitle);
  color: var(--color-title);
  background-color: var(--color-coverbg);
  padding-top: 30px;
  width: auto;
  height: 13%;
  top: 33%;
  right: 5%; 
  left: 5%;
  position: absolute;  
  text-align: center;
  border-bottom-right-radius: 20px;
  border-bottom-left-radius: 20px;
} 

section.cover_b p {
  text-align: center; 
  bottom: 13%;
  width: 100%;
  transform: translateX(-6%);
  position: absolute;
  justify-content: center;
  align-items: center;
}

section.cover_b strong {
  color: var(--color-main);
}

section.cover_b a::after {
  content: "";
}


section.cover_c {
  width: 100%;
  background: linear-gradient(to bottom, white 20%, var(--color-coverbg) 20% 88%, white 88%);
  text-align: left;
}

section.cover_c img {
  background-color: rgba(255, 255, 255, 0);
  background-blend-mode: lighten;  
  filter: brightness(0%) contrast(60%) grayscale(80%);
}

section.cover_c h1 {
  width: 95%;
  padding-top: 8%;
  transform: translateX(0%);
}

section.cover_c h6 {
  font-family: var(--font-family-title);
  font-size: var(--foot-size-subtitle);
  color: var(--color-title);
  transform: translateX(1%);
  margin-top: 0px;  
  width: 95%;
}

section.cover_c p {
  margin-top: 5%;
  transform: translateX(1.5%);
  color: var(--color-title);
}

section.cover_c strong, section.cover_c a  {
  color: var(--color-title);
}

section.cover_c a::after {
  content: "";
}

section.cover_c footer {
  font-size: larger;
  left: 68%;
  bottom: 30px;
}

section.cover_c header {
  background-color: rgba(255, 255, 255, 0);
  background-blend-mode: lighten;    
  height: 150px; 
  width: 380px;
  text-align: left;
  padding: 2% 4%;
}

section.cover_d {
  width: 100%;
  background-image: linear-gradient(to bottom, white 5%, var(--color-coverbg) 5% 60%, white 60%);
  text-align: left;
}

section.cover_d h1 {
  width: 95%;
  /* padding-top: 8%; */
  transform: translateX(0%);
  position: relative;
  bottom: 2%;
}

section.cover_d h6 {
  font-family: var(--font-family-title);
  font-size: var(--foot-size-subtitle);
  color: var(--color-title);
  transform: translateX(1%);
  margin-top: 0px;  
  width: 95%;
  position: relative;
  bottom: 0%;
}

section.cover_d p {
  position: relative;
  bottom: -22%;
  transform: translateX(1.5%);
}

section.cover_d strong {
  color: var(--color-main);
}

section.cover_d a::after {
  content: "";
}

section.cover_d footer {
  font-size: larger;
  left: 68%;
  bottom: 30px;
}


section.toc_a ul {
  list-style-type: none; 
  padding: 30px;
  margin: 30px;
  position: relative; 
  border-radius: 0px 0px 20px 20px;
  border-top: 8px solid var(--color-navbar-font);
  background-color: white;
  box-shadow: 3px 3px 25px  rgb(215, 224, 235);
} 

section.toc_a ul li {
  counter-increment: toc_a;
} 

section.toc_a ul li::before {
  font-family: var(--font-family-title);
  color:white;
  content: counter(toc_a);
  margin-right: 20px;
  margin-bottom: 10px;
  width:35px;
  height:35px;
  display:inline-flex;
  position: relative; 
  align-items:center;
  justify-content: center;
  background-color:var(--color-much);
  border-radius:50%;
} 

section.toc_a ul li:hover::before {
  -moz-transition: all 0.5s ease-out;
  transition: all 0.3s ease-out;
  -moz-transform: rotate(360deg); 
  -webkit-transform: rotate(360deg); 
  -o-transform: rotate(360deg); 
  -ms-transform: rotate(360deg); 
  transform: rotate(360deg);
}

section.toc_a header {
  height: 100%;
  width: 150%;
  font-family: 'Fira Code';
  font-weight: bolder;
  font-size: 1080%;
  left: -8px;
  text-align: center;
  display: flex;
  line-height: 162px;  
  -webkit-text-fill-color: transparent;   
  -webkit-text-stroke: 0.75px var(--color-navbar-font);
}


section.toc_b {
  width: 100%;
  background: linear-gradient(to right, white 6%, var(--color-coverbg) 6% 30%, white 30%);
}

section.toc_b>ul,section.toc_b>ol {
  list-style-type: none;
  display: table;
  align-items:center;
  justify-content: center;
  width: 63%;
  left: 30%;
  position: absolute;
  line-height: 200%;
} 

section.toc_b ul li {
  counter-increment: toc_b;
} 

section.toc_b ul li::before {
  content: counter(toc_b);
  margin: 0px 20px 0px 0px;
  width:35px;
  height:35px;
  display:inline-flex;
  position: relative; 
  align-items:center;
  justify-content: center;
  font-family: var(--font-family-title);
  background-color:var(--color-much);
  border-radius:50%;
  color:white;
} 

section.toc_b ul li:hover::before {
  -moz-transition: all 0.5s ease-out;
  transition: all 0.3s ease-out;
  -moz-transform: rotate(360deg); 
  -webkit-transform: rotate(360deg); 
  -o-transform: rotate(360deg); 
  -ms-transform: rotate(360deg); 
  transform: rotate(360deg);
} 

section.toc_b header {
  text-align: center;
  width: 20%;
  left: 8%;
  top: 25%;
  font-size: var(--font-size-2-3);
  color: var(--color-title);
  font-weight: bolder;
  line-height: 200%;
  letter-spacing: 3px;
  font-family: "Fira Code", var(--font-family-main);
}

section.toc_b img {
  background-color: rgba(255, 255, 255, 0);
  background-blend-mode: lighten;  
  padding-top: 30px;
  width: 70%;
  filter: brightness(1000%)  grayscale(100%);
}

section.fglass ul {
  padding: 20px 20px 20px 60px;
  margin-left: -25px;
  border-radius: 0px 0px 20px 20px;
  border-top: 8px solid var(--color-navbar-font);
  background-color: white;
  box-shadow: 1px 1px 12px  rgb(215, 224, 235);
}



section.col1_ol_sq h2, section.col1_ol_sq h3 {
  margin-left: -2%;
}
section.col1_ol_sq p {
  padding-bottom: 1%;
  margin-left: -1.5%;
}
section.col1_ol_sq>ul,section.col1_ol_sq>ul {
  list-style-type: none;
  display: table;
  align-items:center;
  justify-content: center;
  line-height: 180%;
} 
section.col1_ol_sq ul li {
  counter-increment: col1_ol_sq;
} 
section.col1_ol_sq ul li::before {
  content: counter(col1_ol_sq);
  margin: 0px 20px 0px 0px;
  width:27px;
  height:27px;
  display:inline-flex;
  position: relative; 
  align-items:center;
  justify-content: center;
  font-size: 20px;
  font-family: var(--font-family-title);
  background-color:var(--color-much);
  /* border-radius:50%; */
  color:white;
  margin-left: -1.5%;
} 
section.col1_ol_sq ul li:hover::before {
  -moz-transition: all 0.5s ease-out;
  transition: all 0.3s ease-out;
  -moz-transform: rotate(360deg); 
  -webkit-transform: rotate(360deg); 
  -o-transform: rotate(360deg); 
  -ms-transform: rotate(360deg); 
  transform: rotate(360deg);
} 

section.col1_ol_ci h2, section.col1_ol_ci h3 {
  margin-left: -2%;
}
section.col1_ol_ci p {
  padding-bottom: 1%;
  margin-left: -1.5%;
}
section.col1_ol_ci>ul,section.col1_ol_ci>ol {
  list-style-type: none;
  display: table;
  align-items:center;
  justify-content: center;
  line-height: 180%;
} 
section.col1_ol_ci ul li {
  counter-increment: col1_ol_sq;
} 
section.col1_ol_ci ul li::before {
  content: counter(col1_ol_sq);
  margin: 0px 20px 0px 0px;
  width:27px;
  height:27px;
  display:inline-flex;
  position: relative; 
  align-items:center;
  justify-content: center;
  font-size: 20px;
  font-family: var(--font-family-title);
  background-color:var(--color-much);
  border-radius:50%; 
  color:white;
  margin-left: -1.5%;
} 
section.col1_ol_ci ul li:hover::before {
  -moz-transition: all 0.5s ease-out;
  transition: all 0.3s ease-out;
  -moz-transform: rotate(360deg); 
  -webkit-transform: rotate(360deg); 
  -o-transform: rotate(360deg); 
  -ms-transform: rotate(360deg); 
  transform: rotate(360deg);
} 

section.cols2_ol_sq h2, section.cols2_ol_sq h3 {
  margin-left: -2%;
}

section.cols2_ol_sq p {
  padding-bottom: 1%;
  margin-left: -1.5%;
}

section.cols2_ol_sq ol, section.cols2_ol_sq ul {
  left: 1%;
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 0.7em;
  list-style-type: none;
  width: 98%;
  column-gap: 3em;
} 

section.cols2_ol_sq ol li, section.cols2_ol_sq ul li {
  counter-increment: cols2_ol_sq;
} 

section.cols2_ol_sq ol li::before, section.cols2_ol_sq ul li::before {
  content: counter(cols2_ol_sq);
  margin: 0px 20px 0px 0px;
  width: 30px;
  height: 30px;
  display:inline-flex;
  position: relative; 
  align-items:center;
  justify-content: center;
  font-size: 20px;
  font-family: var(--font-family-title);
  background-color:var(--color-much);
  /* border-radius: 50%; */
  color:white;
  margin-left: -8%;
} 

section.cols2_ol_sq ol li:hover::before, section.cols2_ol_sq ul li:hover::before {
  -moz-transition: all 0.5s ease-out;
  transition: all 0.7s ease-out;
  -moz-transform: rotate(360deg); 
  -webkit-transform: rotate(360deg); 
  -o-transform: rotate(360deg); 
  -ms-transform: rotate(360deg); 
  transform: rotate(360deg);
} 


section.cols2_ol_ci h2, section.cols2_ol_ci h3 {
  margin-left: -2%;
}

section.cols2_ol_ci p {
  padding-bottom: 1%;
  margin-left: -1.5%;
}

section.cols2_ol_ci ol, section.cols2_ol_ci ul {
  left: 1%;
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 0.7em;
  list-style-type: none;
  width: 98%;
  column-gap: 3em;
} 

section.cols2_ol_ci ol li, section.cols2_ol_ci ul li {
  counter-increment: cols2_ol_ci;
} 

section.cols2_ol_ci ol li::before, section.cols2_ol_ci ul li::before {
  content: counter(cols2_ol_ci);
  margin: 0px 20px 0px 0px;
  width: 30px;
  height: 30px;
  display:inline-flex;
  position: relative; 
  align-items:center;
  justify-content: center;
  font-size: 20px;
  font-family: var(--font-family-title);
  background-color:var(--color-much);
  border-radius: 50%;
  color:white;
  margin-left: -8%;
} 

section.cols2_ol_ci ol li:hover::before, section.cols2_ol_ci ul li:hover::before {
  -moz-transition: all 0.5s ease-out;
  transition: all 0.7s ease-out;
  -moz-transform: rotate(360deg); 
  -webkit-transform: rotate(360deg); 
  -o-transform: rotate(360deg); 
  -ms-transform: rotate(360deg); 
  transform: rotate(360deg);
} 


section.cols2_ul_sq h2, section.cols2_ul_sq h3 {
  margin-left: -2%;
}

section.cols2_ul_sq p {
  padding-bottom: 1%;
  margin-left: -1.5%;
}

section.cols2_ul_sq ul {
  left: 1%;
  /* margin-left: -2%; */
  width: 98%;
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 0.7em;
  list-style-type: none;
  column-gap: 3em;
} 

section.cols2_ul_sq ul li {
  display: block;
  position: relative;
}

section.cols2_ul_sq ul li:before {
  content: "";
  display: inline-flex;
  position: absolute;
  top: 1.2em;
  left: -30px;
  margin-top: -0.9em;
  align-items: center;
  justify-content: center;
  font-family: var(--font-family-title);
  background-color: var(--color-much);
  height: 10px;
  width: 10px;
  /* border-radius: 50%; */
}

section.cols2_ul_ci h2, section.cols2_ul_ci h3 {
  /* top: 13%;
  position: absolute; */
  margin-left: -2%;
}

section.cols2_ul_ci p {
  padding-bottom: 1%;
  margin-left: -1.5%;
}

section.cols2_ul_ci ul {
  left: 1%;
  /* margin-left: -2%; */
  width: 98%;
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 0.7em;
  list-style-type: none;
  column-gap: 3em;
} 

section.cols2_ul_ci ul li {
  display: block;
  position: relative;
}

section.cols2_ul_ci ul li:before {
  content: "";
  display: inline-flex;
  position: absolute;
  top: 1.2em;
  left: -30px;
  margin-top: -0.9em;
  align-items: center;
  justify-content: center;
  font-family: var(--font-family-title);
  background-color: var(--color-much);
  height: 10px;
  width: 10px;
  border-radius: 50%;
}



section.cols-2 {
  overflow: visible;
  display: grid;
  gap: 1.5rem;
  grid-template-columns: 50% 50%;
  grid-template-rows: 10% 90%;
  grid-template-areas:
      "slideheading slideheading"
      "leftpanel    rightpanel";
}

section.cols-2 h2, section.cols-2 h3 {
  grid-area: slideheading;
  font-size: var(--font-size-2-3);
}

section.cols-2 .ldiv { 
  grid-area: leftpanel; 
  margin-top: -5%;
}
section.cols-2 .rdiv { 
  grid-area: rightpanel; 
  margin-top: -5%;
}
section.cols-2 .limg { 
  grid-area: leftpanel; 
  margin-top: -5%;
  display: flex;
  align-items: center;  
  justify-content: center;
}
section.cols-2 .rimg { 
  grid-area: rightpanel; 
  margin-top: -5%;
  display: flex;
  align-items: center;  
  justify-content: center;
}

section.cols-3 {
  overflow: visible;
  display: grid;
  gap: 1rem;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 10% 90%;
  grid-template-areas:
      "slideheading slideheading slideheading"
      "leftpanel    middlepanel  rightpanel";
}

section.cols-3 h2, section.cols-3 h3 {
  grid-area: slideheading;
  font-size: var(--font-size-2-3);
}

section.cols-3 .ldiv { 
  grid-area: leftpanel; 
  margin-top: -5%;
}
section.cols-3 .mdiv { 
  grid-area: middlepanel; 
  margin-top: -5%;
}
section.cols-3 .rdiv { 
  grid-area: rightpanel; 
  margin-top: -5%;
}
section.cols-3 .limg { 
  grid-area: leftpanel; 
  margin-top: -5%;
  display: flex;
  align-items: center;  
  justify-content: center;
}
section.cols-3 .mimg { 
  grid-area: middlepanel; 
  margin-top: -5%;
  display: flex;
  align-items: center;  
  justify-content: center;
}
section.cols-3 .rimg { 
  grid-area: rightpanel; 
  margin-top: -5%;
  display: flex;
  align-items: center;  
  justify-content: center;
}

section.cols-2-73 {
  overflow: visible;
  display: grid;
  gap: 1rem;
  grid-template-columns: 70% 30%;
  grid-template-rows: 10% 90%;
  grid-template-areas:
      "slideheading slideheading"
      "leftpanel    rightpanel";
}

section.cols-2-73 h2, section.cols-2-73 h3 {
  grid-area: slideheading;
  font-size: var(--font-size-2-3);
}

section.cols-2-73 .ldiv { 
  grid-area: leftpanel; 
  margin-top: -2%;
}
section.cols-2-73 .rdiv { 
  grid-area: rightpanel; 
  margin-top: -2%;
}
section.cols-2-73 .limg { 
  grid-area: leftpanel; 
  margin-top: -2%;
  display: flex;
  align-items: center;  
  justify-content: center;
}
section.cols-2-73 .rimg { 
  grid-area: rightpanel; 
  margin-top: -2%;
  display: flex;
  align-items: center;  
  justify-content: center;
}

section.cols-2-64 {
  overflow: visible;
  display: grid;
  gap: 1rem;
  grid-template-columns: 60% 40%;
  grid-template-rows: 10% 90%;
  grid-template-areas:
      "slideheading slideheading"
      "leftpanel    rightpanel";
}

section.cols-2-64 h2, section.cols-2-64 h3 {
  grid-area: slideheading;
  font-size: var(--font-size-2-3);
}

section.cols-2-64 .ldiv { 
  grid-area: leftpanel; 
  margin-top: -2%;

}
section.cols-2-64 .rdiv { 
  grid-area: rightpanel; 
  margin-top: -2%;
}

section.cols-2-64 .limg { 
  grid-area: leftpanel; 
  margin-top: -2%;
  display: flex;
  align-items: center;  
  justify-content: center;
}
section.cols-2-64 .rimg { 
  grid-area: rightpanel; 
  margin-top: -2%;
  display: flex;
  align-items: center;  
  justify-content: center;
}

section.cols-2-37 {
  overflow: visible;
  display: grid;
  gap: 1rem;
  grid-template-columns: 30% 70%;
  grid-template-rows: 10% 90%;
  grid-template-areas:
      "slideheading slideheading"
      "leftpanel    rightpanel";
}

section.cols-2-37 h2, section.cols-2-37 h3 {
  grid-area: slideheading;
  font-size: var(--font-size-2-3);
}

section.cols-2-37 .ldiv { 
  grid-area: leftpanel; 
  margin-top: -2%;
}
section.cols-2-37 .rdiv { 
  grid-area: rightpanel; 
  margin-top: -2%;
}
section.cols-2-37 .limg { 
  grid-area: leftpanel; 
  margin-top: -2%;
  display: flex;
  align-items: center;  
  justify-content: center;
}
section.cols-2-37 .rimg { 
  grid-area: rightpanel; 
  margin-top: -2%;
  display: flex;
  align-items: center;  
  justify-content: center;
}

section.cols-2-46 {
  overflow: visible;
  display: grid;
  gap: 1rem;
  grid-template-columns: 40% 60%;
  grid-template-rows: 10% 90%;
  grid-template-areas:
      "slideheading slideheading"
      "leftpanel    rightpanel";
}

section.cols-2-46 h2, section.cols-2-46 h3 {
  grid-area: slideheading;
  font-size: var(--font-size-2-3);
}

section.cols-2-46 .ldiv { 
  grid-area: leftpanel; 
  margin-top: -2%;

}
section.cols-2-46 .rdiv { 
  grid-area: rightpanel; 
  margin-top: -2%;
}

section.cols-2-46 .limg { 
  grid-area: leftpanel; 
  margin-top: -2%;
  display: flex;
  align-items: center;  
  justify-content: center;
}
section.cols-2-46 .rimg { 
  grid-area: rightpanel; 
  margin-top: -2%;
  display: flex;
  align-items: center;  
  justify-content: center;
}

section.rows-2 {
  overflow: visible;
  display: grid;
  gap: 1rem;
  grid-template-rows: 7% 45% 45%;
  grid-template-columns: 100%;
  grid-template-areas:
      "slideheading"
      "toppanel"
      "bottompanel";
}
section.rows-2 h2, section.rows-2 h3 {
  grid-area: slideheading;
}
section.rows-2 .tdiv { 
  grid-area: toppanel; 
}
section.rows-2 .bdiv { 
  grid-area: bottompanel; 
}
section.rows-2 .timg { 
  grid-area: toppanel; 
  display: flex;
  align-items: center;  
  justify-content: center;
}
section.rows-2 .bimg { 
  grid-area: bottompanel;
  display: flex;
  align-items: center;  
  justify-content: center;
}

section.pin-3 {
  overflow: visible;
  display: grid;
  gap: 1rem;
  grid-template-rows: 7% 42% 48%;
  grid-template-columns: 50% 50%;
  grid-template-areas:
      "slideheading slideheading"
      "toppanel  toppanel"
      "leftpanel rightpanel";
}
section.pin-3 h2, section.pin-3 h3 {
  grid-area: slideheading;
  font-size: var(--font-size-2-3);
}
section.pin-3 .tdiv { 
  grid-area: toppanel; 
}
section.pin-3 .ldiv { 
  grid-area: leftpanel; 
}
section.pin-3 .rdiv { 
  grid-area: rightpanel; 
}
section.pin-3 .timg { 
  grid-area: toppanel; 
  display: flex;
  align-items: center;  
  justify-content: center;
}
section.pin-3 .limg { 
  grid-area: leftpanel;
  display: flex;
  align-items: center;  
  justify-content: center;
}
section.pin-3 .rimg { 
  grid-area: rightpanel;
  display: flex;
  align-items: center;  
  justify-content: center;
}


section.bq-blue blockquote, section.bq-red blockquote, section.bq-green blockquote, section.bq-purple blockquote, section.bq-black blockquote {
  padding: 1%;
  letter-spacing: 0px;
  border-left: none;
  background-color: white;
}

section.bq-purple blockquote p>strong {
  color: var(--color-main);
  font-size: 0.9rem;
}


section.bq-blue blockquote>p::before, section.bq-red blockquote>p::before, section.bq-green blockquote>p::before, section.bq-purple blockquote>p::before, section.bq-black blockquote>p::before {
  padding-right: 0px;
  content: "";
  color: white;
}

section.bq-blue blockquote>p:nth-child(1), section.bq-red blockquote>p:nth-child(1), section.bq-green blockquote>p:nth-child(1), section.bq-purple blockquote>p:nth-child(1), section.bq-black blockquote>p:nth-child(1) {
  margin-bottom: -1px;
  line-height: 2rem;
  padding: 0.5% 0.5% 0.5% 1.5%;
  color: white;
  font-size: 1.03rem;
}

section.bq-blue blockquote>p:not(:nth-child(1)), section.bq-red blockquote>p:not(:nth-child(1)), section.bq-green blockquote>p:not(:nth-child(1)), section.bq-purple blockquote>p:not(:nth-child(1)), section.bq-black blockquote>p:not(:nth-child(1)) {
  padding: 1% 2%;
  background-color: rgb(228, 234, 246);
}


section.bq-blue blockquote>p:nth-child(1) {
  background-color: rgb(129, 161, 193);
}

section.bq-red blockquote>p:nth-child(1) {
  background-color: rgb(191, 97, 106);
} 

section.bq-green blockquote>p:nth-child(1) {
  background-color: rgb(172, 206, 141);
}

section.bq-purple blockquote>p:nth-child(1) {
  background-color: rgb(180, 142, 173);
}

section.bq-black blockquote>p:nth-child(1) {
  background-color: rgb(67, 76, 94);
}

section.bq-blue blockquote>p:nth-child(1)::before {
  content: "\f518";
  padding-right: 2%;
  font-family: "FontAwesome";
}

section.bq-red blockquote>p:nth-child(1)::before {
  content: "\f0eb";
  padding-right: 2%;
  font-family: "FontAwesome";
}

section.bq-green blockquote>p:nth-child(1)::before {
  content: "\e0bb";
  padding-right: 2%;
  font-family: "FontAwesome";
}

section.bq-purple blockquote>p:nth-child(1)::before {
  content: "\f7e4";
  padding-right: 2%;
  font-family: "FontAwesome";
}

section.bq-black blockquote>p:nth-child(1)::before {
  content: "\f5ad";
  padding-right: 2%;
  font-family: "FontAwesome";
}

section.lastpage  {
  background: linear-gradient(to bottom,white 20%,var(--color-coverbg) 20% 60%,white 55%);
  padding: 0;
  display: grid;
  grid-template-rows: 80% 20%;
  grid-template-columns: auto;
  grid-template-areas: 
      "heading"
      "icons";
}

section.lastpage h6 {
  height: 80px; 
  margin-bottom: 10px;
  text-align: center;
  vertical-align: middle;
  font-family: var(--font-family-title); 
  font-size: var(--font-size-1);
  color: var(--color-title);

  display: grid;
  padding: 0;
  height: 100%;
  width: 100%;
  align-content: center;
  justify-content: center;
}

section.lastpage h6 {
  grid-area: heading;
}

section.lastpage .icons {
  grid-area: icons;
}

section.lastpage div>ul {
  font-family: var(--font-family-main);
  width: 100%;
  display: grid;
  grid-template-columns: 1.8fr 1fr 1fr;
  gap: 5em;
  align-content: center;
  list-style: none;
  
}
section.lastpage ul>li>ul>li {
  margin-left: -120px;
}
section.lastpage div>ul>li>ul>li {
  list-style: none;
}

.fa-envelope, .fa-weixin, .fa-phone-volume, .fa-house {
  border: 2px solid;
  padding: 10px;
  border-radius: 50%;
  font-size: 1.2rem;
}

section.lastpage a {
  font-size: var(--font-size-main);
}

section.lastpage a::after, section.lastpage::after {
  position: relative;
  content: "";
  border: none;
  color: white;
}

section.navbar header {
  background-color: var(--color-navbar-bg);
  width: 100%;
  height: 5%;
  padding: 6px 0px 3px 0px;
  left: 0px;
  top: 0px;
  display: flex;
  justify-content: space-between;
  color: var(--color-navbar-font);
  white-space: pre;
}

section.navbar header>em, section.navbar header>strong,section.navbar header>em>strong {
  font-style: normal;
  font-size: 0.9rem;
  font-weight: normal;
  color: var(--color-navbar-font);
}

section.navbar header>strong {
  border: 1px solid white;
  border-radius: 12px;
  padding: 0px 15px 5px 15px;
  background-color: white;
}

section.navbar header::before, section.navbar header::after {
  content: "";
}

section.navbar header>em>strong {
  display: block;
  width: 400px;
  text-align: left;
  margin-left: -20px;
}


section.trans  {
  background-color: var(--color-trans);
}
section.trans h2{
  text-align: center; 
  color: var(--color-title);
  font-size: 2rem;
}


section.caption .caption {
  padding-top: 20px;
  text-align: center;
  font-size: smaller;
  color: var(--color-footer);
}

table {
  border-collapse: collapse;
  text-align: center;
  word-break: initial;
  font-size: 0.8rem;
  margin: 0 auto;
}

table code {
  font-size: 0.7rem;
}
th, thead {
  height: 40px;
  border-top: 3px solid var(--color-main);
  font-size: 105%;
  padding: 6px;
}
th, thead:first-child {
  border-bottom: 3px solid var(--color-main);
}
table tr:nth-child(2n) {
  background-color: white;
}
tbody:last-child {
  border-bottom: 3px solid var(--color-main)
}
table > thead > tr > th,
table > thead > tr > td,
table > tbody > tr > th,
table > tbody > tr > td,
table > tfoot > tr > th,
table > tfoot > tr > td {
  border: 0px solid white;
}

.hljs {
  display: block;
  overflow-x: auto;
  padding: 0.5em;
  font-size: small;
}
.hljs-comment {
  color: #28a828;
}
.hljs-string {
  color: #fd8f3f;
}
.hljs-number {
  color: rgb(158, 158, 62);
}
.hljs-keyword {
  color: #1111e2;
}
.hljs-symbol {
  color: #ac1212;
}
.hljs-variable {
  color: #fc5fa3;
}
.hljs-built_in {
  color: #960ab9;
}
.hljs-emphasis {
  font-style: italic;
}
.hljs-meta {
  color: #2c2cff;
}
.hljs-literal {
  color: #2c2cff;
}
.hljs-name {
  color: #2c2cff;
}
.in-prompt { color: #99bb88; }
.in-prompt-number { font-weight: bold; }
.out-prompt { color: #ff9090; }
.out-prompt-number { font-weight: bold; }
.inverted { background-color: white; color: #232629; }

section.fixedtitleA {
  justify-content: start;
}
section.fixedtitleB {
  justify-content: start;
  display: grid;
  gap: 1.5rem;
  grid-template-rows: 10% 90%;
  grid-template-areas: 
      "slideheading"
      "content";
}
section.fixedtitleB>h2, section.fixedtitleB>h3, section.fixedtitleB>h4, section.fixedtitleB>h5{
  grid-area: slideheading;
  position: absolute;
  padding: 10px;
  background-color: var(--color-much);
  color: white;
  border-radius: 8px;
  font-size: 1.25rem;
}
section.fixedtitleB .div {
  grid-area: content;
} 
section.fixedtitleB code {
  color: var(--color-much);
}

section.footnote {
  display: grid;
  gap: 0.7em;
  grid-template-rows: 1fr auto;
  grid-template-areas: "content" "footnote";
} 
section.footnote .tdiv {
  grid-area: "content"; 
  justify-content: start;
}
section.footnote .tdiv>h2,section.footnote .tdiv>h3,section.footnote .tdiv>h4,section.footnote .tdiv>h5 {
  margin-bottom: 1rem;
  margin-top: -1rem;
}
section.footnote .bdiv {
  grid-area: "footnote";
  font-size: 85%;
  bottom: 5%;
}
section.footnote .bdiv::before {
  border-top: 1.8px dashed var(--color-coverbg);
  content: "";
  display: block;
  margin-bottom: 1em;
}

section.tinytext>p, section.tinytext>ul, section.tinytext>ol, section.tinytext>table, section.tinytext>blockquote {
  font-size: 80%;
}
section.tinytext code {
  font-size: 90%;
}
section.tinytext strong {
  font-size: 100%;
}
section.tinytext em {
  font-size: 90%;
}
section.tinytext pre {
  font-size: 70%;
}
section.smalltext>p, section.smalltext>ul, section.smalltext>ol, section.smalltext>table, section.smalltext>blockquote {
  font-size: 90%;
}
section.smalltext code {
  font-size: 90%;
}
section.smalltext strong {
  font-size: 100%;
}
section.smalltext em {
  font-size: 90%;
}
section.smalltext pre {
  font-size: 80%;
}
section.largetext>p, section.largetext>ul, section.largetext>ol, section.largetext>table, section.largetext>blockquote{
  font-size: 115%;
}
section.largetext strong {
  font-size: 100%;
}
section.largetext code {
  font-size: 90%;
}
section.largetext em {
  font-size: 90%;
}
section.largetext pre {
  font-size: 105%;
}
section.hugetext>p, section.hugetext>ul, section.hugetext>ol, section.hugetext>table, section.hugetext>blockquote {
  font-size: 130%;
}
section.hugetext strong {
  font-size: 100%;
}
section.hugetext code {
  font-size: 90%;
}
section.hugetext em {
  font-size: 90%;
}
section.hugetext pre {
  font-size: 120%;
}


/* @theme am_blue */

@import 'am_template';

:root {
  --color-code-bg: #e8f4f6;
  --color-coverbg: #2c9cb1;
  --color-few: #91a814;
  --color-footer: #8c8c8c;
  --color-main: #041d22;
  --color-much: #1482a8;
  --color-navbar-bg: #d0e9ee;
  --color-navbar-font: rgb(108, 95, 91);
  --color-quote: rgba(254, 176, 98, 0.1);
  --color-title: rgb(255, 255, 255);
  --color-trans: #72bdcb;
  --filter-b: brightness(30%) contrast(70%) grayscale(100%);
  --filter-c: brightness(0%) contrast(60%) grayscale(80%);
  --filter-e: brightness(0%) contrast(70%) grayscale(100%);
}
</style>


<!-- _class: cover_a -->
<!-- _header: "" --> 
<!-- _footer: "" --> 
<!-- _paginate: "" --> 

# 大数据实践：纽约地铁地铁人流量预测

###### 面向特色化领域的实践1-大数据软件课设

赵羿弦、王皓、贺佳明、菅佳玥
2024 年 12 月 17 日


## 目录 Content

<!-- _class: cols2_ol_ci fglass toc_a  -->
<!-- _footer: "" -->
<!-- _header: "CONTENTS" -->
<!-- _paginate: "" -->

- [效果演示](#3)
- [业务介绍](#10) 
- [架构设计](#16)
- [数据来源](#20)
- [实现细节](#38)



## 1. 效果演示

<!-- _class: trans -->
<!-- _footer: "" -->
<!-- _paginate: "" -->


## 2. 业务介绍

主要工作：

1. 为站点建立主要以时间周期为参数的出入人数（吞吐量）预测模型；
2. 实现历史 OD 每小时、每日、若干小时、若干天统计；
3. 实现线路拥挤度预测模型。

业务价值：

1. 对交通研究者：分析 OD 历史统计数据；
2. 对交通研究者：根据预测的站点吞吐量、线路拥挤度执行相应调度策略；
3. 对公众：提供站点吞吐量、线路拥挤度预测信息查询。

## 3. 架构设计

<img src="https://s2.loli.net/2024/12/17/nc3MZ8RNYT12Si7.png" alt="b8db2e14649ba86f8860c92755138b44" style="zoom:35%;" />

## 4. 数据来源与初步预处理方向

<!-- _class: trans -->
<!-- _footer: "" -->
<!-- _paginate: "" -->

### 4.1 数据来源与字段说明

纽约地铁来源-目标数据：

- Timestamp: 时间戳
- OriginStationId: 来源站点 ID
- DestinationStationId：目标站点 ID
- Ridership: 乘客人数

站点与线路所属关系数据：

- StationId：站点 ID
- StationName：站点名称
- Routes：途经线路

GTFS 数据：

- 辅助构建线路图，字段详见 GTFS 标准。

### 4.2 数据初步预处理：两种方向

- 站点视角：
  - 按站点、出入站、时间戳（精确到小时）聚合：站点预测数据源
  - 拆分时间戳：利用日期的周期性
  - 添加星期几（Day In Week）、是否为假期字段，进一步挖掘数据潜在的周期性

- 路线视角：
  - 在换手点拆分带有换乘的来源-目标数据；
  - 将来源-目标数据平摊到可能的多条线路上；
  - 按时间戳（精确到小时）、线路、来源-目标对聚合：线路拥挤度预测数据源

## 5. 实现细节：站点人流量预测

<!-- _class: trans -->
<!-- _footer: "" -->
<!-- _paginate: "" -->
### 5.1. 站点人流量预测

采用随机森林回归器实现对地铁系统各个站点的人流量预测：

- 每站点建模，请求时按需加载站点模型
- 模型特征：

  - 年、月、日、星期、是否节假日、小时、出/入站

- 模型标签：

  - 出站人数、入站人数

### 5.2. 参数调节与优化

随机选取 10 站，使用参数组分别计算对应模型的 RMSE（站点间取均值）：

|树数目\最大深度|5|10|15|20|25|
|---|---|---|---|---|---|
|10|32.318|26.305|**23.377**|23.802|23.796|
|20|34.594|25.908|25.182|25.034|25.022|
|30|30.257|24.985|25.875|26.066|26.109|
|40|31.432|24.922|23.546|23.802|23.811|
|50|31.586|25.325|25.123|25.399|25.4|

在 $树数目 = 10 且深度 = 15$ 时效果较为良好。


## 6. 实现细节：OD数据预处理与统计

<!-- _class: trans -->
<!-- _fooater: "" -->
<!-- _paginate: "" -->

## 6.1 构建纽约地铁图结构

#### 6.1.1 构建图结构的原因

- **问题**：**希望从现有的OD数据中提取更多信息**，如乘车路径、经过的线路和换乘情况。  
- **解决方案**：基于现有信息，**构建纽约地铁的图结构**，并**使用最短路径算法估计乘客的乘车路径**。


<img src="https://s2.loli.net/2024/12/17/9CueHNDoIUtzV5Y.png" alt="image-20241217083649963" style="zoom:80%;" />




## 6.1.2 已有数据集

<!-- _class: cols-2 -->  

<div class=ldiv>  

- `MTA_Subway_Stations.csv`
  - 纽约所有**站点的详细信息**，包括其站点名，id，服务的线路集合，经纬度等。

<div style="text-align: center;">
<img src="https://s2.loli.net/2024/12/16/MDiSoYJEluqKVTU.png" alt="image-20241216224345537" style="zoom:45%;" />
</div>
</div>

<div class=rdiv>

- `Subway_Lines.geojson`
  - 纽约所有**地铁线路的轨迹信息**。

<div style="text-align: center;">
<img src="https://s2.loli.net/2024/12/16/UuZePrx5ItASjQq.png" alt="image-20241216224115062" style="zoom:50%;" />
</div>
</div>


## 6.1.3 数据集初步处理

<!-- _class: cols-2 -->  

<div class=ldiv>  

- 美中不足的是，**纽约地铁的轨迹数据集中没有标注站点**。由于轨迹数据集的不完美性，我们也**无法将站点直接标注到轨迹中**。所以我们准备**自行建立纽约地铁图结构**。

- 在检查数据集时，**发现了一条特殊的线路：S线。**

> 纽约地铁的**S线**（Shuttle）是接驳线，方便乘客换乘。共有三条路线：**42街接驳线**（连接时报广场与大中央车站）、**富兰克林大道接驳线**（位于布鲁克林，连接富兰克林大道站与展望公园站）和**洛克威公园接驳线**（位于皇后区，连接宽水道站与洛克威公园-海滩116街站）。


</div>

<div class=rdiv>

- 为了方便之后的处理，我们**将其分割为三条线路**。


<div style="text-align: center;">
<img src="https://s2.loli.net/2024/12/17/igfXcQoYWNltCVz.png" alt="image-20241217094040265" style="zoom:70%;" />
</div>

</div>


## 6.1.4 图构建方法



<!-- _class: pin-3-change1 -->

<div class="tdiv">

- 将每条线路的**站点经纬度标注在图上**，手动标注起终点，并**将其转化为旅行商问题（TSP）**。我们使用谷歌开源的`OR-Tools`求解，**大多数线路可直接得到正确的连线方式，少数形状特殊的线路只需对图结构稍作调整**。

</div>

<div class="ldiv">

- 例如，对于1号线，在图中标注所有点：

<img src="https://s2.loli.net/2024/12/17/Oai5Nv1VShQxUoK.png" alt="subway_line_1_initial_plot" style="zoom:80%;" />

</div>

<div class="rdiv">


- 使用`OR-Tools`计算出的路径为：

<img src="https://s2.loli.net/2024/12/17/qC2aBtfhUAH5iWL.png" alt="subway_line_1_optimized_path" style="zoom:80%;" />

</div>


## 6.1.4 图构建方法



<!-- _class: cols-3 -->



<div class=ldiv>

- 真实的5号线地铁线路图：

<div style="text-align: center;">
<img src="https://s2.loli.net/2024/12/17/fc1rUkevwpMCNPn.png" alt="image-20241217082228401" style="zoom:60%;" />
</div>
</div>

<div class=mdiv>

- 由`OR-Tools`初步处理后：

<div style="text-align: center;">

<img src="https://s2.loli.net/2024/12/17/6S7qzy895PR1Tu3.png" alt="subway_line_5_optimized_path" style="zoom:35%;" />
</div>
</div>



<div class=rdiv>

- 按照真实路线图，手动调整原图的部分边，将图结构调整为真实路线的结构：

<div style="text-align: center;">
<img src="https://s2.loli.net/2024/11/18/cfCASnbuyrWhH9L.png" alt="Figure_2" style="zoom:80%;" />
</div>
</div>


## 6.1.4 图构建方法

- 在构建每条地铁线路的图结构后，将其**合并为完整的纽约地铁图结构**。**节点之间的边权重为两站点间的直线距离**，计算方式采用 Haversine 公式。

<img src="https://s2.loli.net/2024/12/17/fM4BEOipXHe3oTh.png" alt="image-20241217081334396" style="zoom:40%;" />



## 6.2 数据预处理与OD数据的统计分析

<!-- _class: cols-2 -->  

<div class=ldiv>  


#### 6.2.1 按换乘拆分OD数据

- 输入：原始的OD数据。
- 输出：无换乘记录的，按小时聚合的OD数据。

<br>

- 原始的OD数据可能包含换乘，涉及多条线路，难以直接分析，我们可以将**一条有换乘数据拆成多条无换乘的数据**。

</div>

<div class=rimg>

<img src="https://s2.loli.net/2024/12/17/veD6HEA8NayVGQI.png" alt="image-20241217084555949" style="zoom:80%;" />

</div>

## 6.2.1 按换乘拆分OD数据

<!-- _class: cols-2-change1 -->  

<div class=ldiv>  



**换乘检测算法**

1. **核心思想**：**逆向遍历站点序列，若某站点的可能线路集合为空，则标记为换乘点，并将其可能线路集合重置为当前边的线路集合。**

2. **计算步骤**：  
   - 初始可能线路集合为最后一段边的线路集合。  
   - 逆向遍历每个站点 $S[i]$，更新可能线路集合：  
     $$
     \text{PossibleLines}[i] = \text{EdgeLines}[i] \cap \text{PossibleLines}[i + 1]
     $$
   - 若 $\text{PossibleLines}[i] = \varnothing$，则 $S[i+1]$ 为换乘点，重置：  
     $$
     \text{PossibleLines}[i] = \text{EdgeLines}[i]
     $$

</div>

<div class=rimg>

<img src="https://s2.loli.net/2024/12/17/k2Fv4ZnNd7BetpI.png" alt="image-20241217085222881" style="zoom:70%;" />

</div>



## 6.2.2 OD数据可视化的实现

**OD矩阵的数据结构**

OD矩阵是一个 $n \times n$ 的矩阵，表示 $n$ 个站点间的客流情况。  

- **行 $i$**：出发站点 $i$ 的客流数据。  
- **列 $j$**：到达站点 $j$ 的客流数据。  
- **元素 $OD_{i,j}$**：表示从站点 $i$ 到站点 $j$ 的乘客人数，且 $OD_{i,i} = 0$（不考虑站内流动）。  

矩阵结构如下：  
$$
\mathbf{OD} = 
\begin{bmatrix}
0          & OD_{1,2} & \cdots & OD_{1,n} \\
OD_{2,1}   & 0        & \cdots & OD_{2,n} \\
\vdots     & \vdots   & \ddots & \vdots   \\
OD_{n,1}   & OD_{n,2} & \cdots & 0
\end{bmatrix}
$$


## 6.2.2 OD数据可视化的实现


1. **数据存储**：每条线路的OD矩阵按每小时、每天的粒度存储在关系型数据库中。

2. **数据查询**：前端可指定线路和时间段，后端汇总该时间段内的OD矩阵并将结果返回前端，前端以密度图的形式进行可视化展示。



<img src="https://s2.loli.net/2024/12/17/NKOfT9dU6mjvLE3.png" alt="image-20241217115355435" style="zoom:70%;" />



## 6.2.3 提取地铁"最小段"人流量与站点换乘人数

<!-- _class: pin-3-change2 -->

<div class="tdiv">


- 输入：按换乘拆分的OD数据。
- 输出：每一个"最小段"的地铁线路的人流量与换乘站点的换乘人数。

</div>

<div class="ldiv">

- 根据最短路径算法的结果，判断乘客所走的线路，并将人流量分配至该线路，若有多条可能线路则平分。


<div style="text-align: center;">
<img src="https://s2.loli.net/2024/12/17/aosWmfwg8xDryiF.png" alt="image-20241217090429240" style="zoom:50%;" />
</div>



</div>

<div class="rdiv">

- 根据换乘检测算法的结果，判断乘客的换乘方式，并将人流量分配至该换乘方式，若有多种可能方式则平分。

<div style="text-align: center;">
<img src="https://s2.loli.net/2024/12/17/XNBexQ9468mGH7z.png" alt="image-20241217091028831" style="zoom:50%;" />
</div>



</div>

## 7. 实现细节：线路拥挤度预测

<!-- _class: trans -->
<!-- _footer: "" -->
<!-- _paginate: "" -->

## 7.1 线路拥挤度预测

<!-- _class: cols-2-64 -->

<div class=ldiv>


|         数据名           | 用到的列 |                   作用                      |
|        ---------         | ------- |                -----------                 | 
| `merged_transit_data`    | `month`, `day`, `hour`, `day_of_week`, `line`, `` | 获得`时间`、`线路`、`星期`等信息          |
| `line_ridership`         | `month`, `day`, `hour`, `day_of_week`, `line`, `segment_ridership`| 获得`时间`、`线路`、`星期`等基本信息，及`每小段人数`                     |
| `StationDivided`         | `destination_entry`, `destination_exit` | 获取每站的进出人数                           |
| `transfer`               |  `total_transfer`   | 获得每站的`换乘人数`                         |
| `subway_lines_start_end` |         | 获取每个站是否是起点或终点                    |

</div>

<div class=rimg>

<!-- ![#c](../images/line_predict_1.png) -->
![#c](../images/line_predict_1.png)
</div>


## 7.2 线路拥挤度预测——数据合并
<!-- _class:  bq-green -->
> data.py 
> 
> 1.加载线路客流数据line_ridership，站点数据StationDivided，换乘数据transfer
> 2.以line_ridership为基准，和其他表进行左连接
> 3.计算换乘人数：分别按 Transfer Station Complex ID 和 from_line 分组，和Transfer Station Complex ID 和 to_line 分组，计算换入和换出的人数。再与前面合并好的表进行左连接（时间相等、id相等）。初始化total_transfers为0，加上换入人数，减去换出人数，就是换乘总人数

![#c](../images/line_predict_2.png)

## 7.3 线路拥挤度预测——数据预处理
<!-- _class:  bq-blue -->
> process.py
> 
> 1.按小时合并数据。创建time_id列（是year，month，day，hour的合并），time_id相同的合并
> 2.找到 `destination_station_id` 和 `End Station ID`或`Start Station ID` 匹配的记录，并添加标记列为待删除，在后面统一删除（如果最后一站就是终点站，那么“下一段人数”必为0）
> 3.使用SQL查询，找到next_segment_ridership：进行自连接，如果t1.destination_station_id = t2.origin_station_id且两条记录的line值相等（再同一地铁线上），且t1.origin_station_id != t2.destination_station_id（非反方向行驶），则认为t1的next_segment_ridership就是t2的segment_ridership
> 4.数据预处理：进行数据类型转化，把所有的数据转为double，把星期的字符串（"Sunday"）转为int（7）

![#c](../images/line_predict_2.png)

## 7.4 线路拥挤度预测——设置特征值
<!-- _class:  bq-purple -->
> feature.py
> 
> 1.对月份、日期、小时、星期进行归一化处理：
> 2.选定特征列和标签列："segment_ridership", "destination_entry", "destination_exit",  "total_transfers", "hour_sin",  "hour_cos", "month_sin", "month_cos", "day_of_week_sin", "day_of_week_cos"以及"next_segment_ridership"
> 3.把所有特征值转为数字便于计算

![#c](../images/line_predict_2.png)

## 7.5 线路拥挤度预测——训练模型

<!-- _class: cols-2-37 -->

<div class=ldiv>

> **predict_forest.py**
1.分批训练：讲数据分为4批避免内存溢出
2.使用随机森林算法：numTrees=150,maxDepth=12，next_segment_ridership作为label
3.使用MAE评价指标。
4.保存最佳模型

![#c](../images/line_predict_2.png)
</div>

<div class=rimg>

<!-- ![#c](../images/line_predict_4.png) -->
![#c](../images/line_predict_4.png)
</div>

## 7.6 线路拥挤度预测——后端接入
<div style="display: flex; justify-content: space-between;">
  <img src="../images/line_predict_5.png" alt="Left Image" width="45%" />
  <img src="../images/line_predict_6.png" alt="Right Image" width="35%" />
</div>

## 7.7 线路拥挤度预测——问题与优化
递归过深，栈溢出
**→** 改为`左连接`+`spark_sum`

![#c](../images/line_predict_3.png)



## 7.7 线路拥挤度预测——问题与优化
**运行时间过长**：每次预测都要调用n次线路预测模型和n次站点人流量预测模型
**优化方案**：改为输入前面所有站的上车、下车、换乘人数的总和+时间

---

<!-- _class: lastpage -->
<!-- _footer: "" -->

###### 感谢您的观看

大数据实践：纽约地铁地铁人流量预测
赵羿弦、王皓、贺佳明、菅佳玥
2024 年 12 月 17 日

## END 

<!-- _class: trans -->
<!-- _footer: "" -->