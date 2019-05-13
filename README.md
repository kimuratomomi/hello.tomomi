# hello.tomomi
portfolio
/* nav */
header {
  width: 100%;
}
.nav {
  width: 95%;
	background-color: #ffffff;
	border: 1px solid #dedede;
	border-radius: 4px;
	color: #888888;
	display: block;
	margin: 1em 1%;
  position: fixed;
  /* overflow: hidden; */
}
.nav ul {
	margin: 0;
	padding: 0;
}

.nav li {
	display: inline-block;
	list-style-type: none;
	-webkit-transition: all 0.2s;
	        transition: all 0.2s;
  text-align: right;
}
.nav > ul > li > a > .caret {
	border-top: 4px solid #aaaaaa;
	border-right: 4px solid transparent;
	border-left: 4px solid transparent;
	content: '';
	display: inline-block;
	height: 0;
	width: 0;
	vertical-align: middle;
	-webkit-transition: color 0.1s linear;
	        transition: color 0.1s linear;
}
.nav > ul > li > a {
	color: #aaaaaa;
	display: block;
	line-height: 56px;
	padding: 0 10px;
	text-decoration: none;
}
.nav > ul > li:hover {
	background-color: rgb(218, 60, 65);
}
.nav > ul > li:hover > a {
	color: rgb( 255, 255, 255 );
}
.nav > ul > li:hover > a > .caret {
	border-top-color: rgb( 255, 255, 255 );
}
.nav > ul > li > div {
	background-color: rgb(218, 60, 65);
	border-top: 0;
	border-radius: 0 0 4px 4px;
	box-shadow: 0 2px 2px -1px rgba(0, 0, 0, 0.055);
	display: none;
	margin: 0;
	opacity: 0;
	position: absolute;
	width: 165px;
	visibility: hidden;
	-webkit-transiton: opacity 0.2s;
	       transition: opacity 0.2s;
}
.nav > ul > li:hover > div {
	display: block;
	opacity: 1;
	visibility: visible;
}
.nav > ul > li > li {
	display: block;
}
.nav > ul > li > li > a {
	color: #ffffff;
	display: block;
	padding: 12px 24px;
	text-decoration: none;
}
.nav > ul > li > li:hover > a {
	background-color: rgba( 255, 255, 255, 0.1);
}

/* メイン画像 */

.home {
  background-image: url(img/maintmy.png);
  object-fit: cover;
  text-align: center;
  padding-top: 250px;
  margin-bottom: 300px;
}

body {
  background-color: white;
  font-style: normal;
  font-family: sans-serif, 'Noto Sans', 'Lato', メイリオ;
}

/* About */
.personal-1 {
  width: 100%;
  height: auto;
  display: flex;
  flex-direction: row;
  margin: 100, 0px;
}

.ja p {
  margin-right: 20px;
  margin-left: 300px;
}

.en p {
  margin-right: 300px;
  margin-left: 20px;
}

.personal h4 {
  text-align: center;
}
 h2 {
  text-align: center;
}

.skill {
  text-align: center;
}
.skill img {
  margin-bottom: 60px;
}

/* Work */
 h2{
  text-align: center;
}
.work {
  display: flex;
}


.work img {
  margin-bottom: 60px;
  -webkit-transform: scale(1);
  transform: scale(1);
  -webkit-transition: .3s ease-in-out;
  transition: .3s ease-in-out;
}

.work img:hover {
  cursor: pointer;
  opacity: 0.5;
  background-color: white;
  -webkit-transform: scale(0.8);
  transform: scale(0.8)
}

/* gallery */
.gallery {
  text-align: center;
}









/* sociallink */
.sociallink h4 {
  text-align: center;
}

.sociallink ul {
  display: flex;
  list-style: none;
}

.sociallink li {
  margin: 10px;
  padding: 20px;
  text-align: center;
}

.link{
  text-align: center;
}


.sociallink img:hover {
  cursor: pointer;
  opacity: 0.5;
}

/* ボタン */
#btn-back {
    line-height: 90px;
    height: 100px;
    width: 100px;
    cursor: pointer;
    background-color:black;
    transition: all 0.5s;
    position: relative;
    float: right;
}

#btn-back a::before{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 1;
    background-color: rgba(255,255,255,0.1);
    transition: all 0.3s;
}

#btn-back a:hover::before {
    opacity: 0 ;
    transform: scale(0.5,0.5);
}
#btn-back a::after {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 1;
    opacity: 0;
    transition: all 0.3s;
    border: 1px solid rgba(255,255,255,0.5);
    transform: scale(1.2,1.2);
}
#btn-back a:hover::after {
    opacity: 1;
    transform: scale(1,1);
}

#btn-back a {
  font-family: 'Open Sans', sans-serif;
  font-size: 1.2em;
  text-decoration: none;
  color: #fff;
  font-style: italic;
  text-align: center;
  margin-left: 25px;
}
