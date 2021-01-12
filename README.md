# CSS_

```css
:root {
  --iframe-font-size-title: 14px;
  --iframe-font-size-titi: 13px;
  --iframe-font-size-rage: 18px;
  --iframe-font-family: "Proza Libre";
  --iframe-logo-family: "Oswald";
  --iframe-blue-color: rgba(0, 0, 255, 0.74);
  --iframe-gray-color: rgba(0, 0, 0, 0.527);
  --iframe-dark-gray-color: rgba(0, 0, 0, 0.644);
  --iframe-light-gray-color: rgba(0, 0, 0, 0.315);
  --iframe-font-color: rgba(0, 0, 0, 0.925);
  --iframe-red-color: rgba(255, 0, 0, 0.884);
  --iframe-padding: 10px;
  --iframe-margin: 3px;
}

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

body {
  font-family: var(---iframe-font-family);
  color: var(--iframe-font-color);
}

li {
  list-style: none;
}

button,
button:focus {
  border: none;
  cursor: pointer;
  outline: none;
  background-color: white;
  font-size: var(--iframe-font-size-rage);
}

header {
  display: flex;
  justify-content: space-between;
  padding: 16px;
  background-color: rgba(0, 0, 0, 0.74);
  color: white;
  align-items: center;
}

header .logo {
  font-size: var(--iframe-font-size-rage);
  font-family: var(--iframe-logo-family);
}

header .logo a {
  color: white;
  text-decoration: none;
}

header .logo i {
  color: red;
}

header .icons i {
  margin-right: var(--iframe-padding);
}

header .icons_input {
  display: none;
  width: 350px;
  height: 20px;
}

header .icons .icons_bt1 {
  color: white;
  background-color: #07070700;
}

header .icons .icons_bt2 {
  color: white;
  background-color: #07070700;
}

.header_movie {
  position: sticky;
  top: 0;
}

.movie {
  text-align: center;
  background-color: black;
}

.movie video {
  text-align: center;
  border: solid black;
  width: 100%;
  height: 100%;
  max-height: 300px;
}

.info .data {
  padding: var(--iframe-padding);
  margin: var(--iframe-margin);
}

.info .data .hash {
  display: flex;
  color: var(--iframe-blue-color);
}

.info .data .hash li {
  margin-bottom: var(--iframe-margin);
  margin-right: var(--iframe-margin);
  font-size: small;
}

.info .data .title {
  display: flex;
  justify-content: space-between;
  cursor: pointer;s
}

.info .data .title span {
  font-size: var(--iframe-font-size-rage);
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-line-clamp: 1;
  overflow: hidden;
  margin-right: var(--iframe-margin);
}

.info .data .title .title_bt {
  height: 100%;
}

.info .data .views span {
  font-size: var(--iframe-font-size-titi);
  color: var(--iframe-gray-color);
}

.info .actions {
  display: flex;
  justify-content: space-around;
  margin: var(--iframe-padding);
  margin-top: 10px;
}

.info .actions i {
  display: flex;
  flex-direction: column;
  font-size: var(--iframe-font-size-rage);
  color: var(--iframe-gray-color);
}

.info .actions li span {
  display: flex;
  flex-direction: column;
  font-size: var(--iframe-font-size-titi);
  padding: var(--iframe-margin);
}

.info .channer {
  display: flex;
  justify-content: space-between;
  border-top: 1px solid var(--iframe-light-gray-color);
  border-bottom: 1px solid var(--iframe-light-gray-color);
  padding: var(--iframe-padding);
}

.info .channer .channer_data {
  display: flex;
  align-items: center;
  cursor: pointer;
}

.info .channer .channer_data .channer_info {
  display: flex;
  flex-direction: column;
}
.info .channer .channer_data .channer_info .chenner_title {
  font-size: var(--iframe-font-size-title);
}
.info .channer .channer_data .channer_info .chenner_titi {
  font-size: var(--iframe-font-size-titi);
  color: var(--iframe-gray-color);
}

.info .channer .channer_data img {
  width: 48px;
  height: 48px;
  border-radius: 50%;
  margin-right: var(--iframe-margin);
}

.info .channer .channer_bt {
  color: var(--iframe-red-color);
  font-size: var(--iframe-font-size-title);
}

.last {
  padding: var(--iframe-padding);
}

.last .last_title{
  display: flex;
  justify-content : space-between;
}

.last .last_btn{
  border-top-left-radius : 15px;
  border-top-right-radius : 15px;
  border-bottom-right-radius : 15px;
  border-bottom-left-radius : 15px;
  background-color: var(--iframe-light-gray-color);
  width: 40px;
  text-align : left; 
}

.last .last_btn .last_btnsub{
  display: inline;
  border-radius: 50%;
  background-color:var(--iframe-gray-color);
  color: rgba(24, 23, 22, 0.068) ;
  width: 100%;
}

.last .item {
  display: flex;
  margin-top: var(--iframe-padding);
}

.last .item_text {
  display: flex;
  flex-direction: column;
}

.last .item .item_text {
  flex: 1 65%;
  margin: var(--iframe-margin);
}

.last .item .item_img {
  flex: 1 35%;
  margin-top: var(--iframe-margin);
}

.last img {
  width: 100%;
  height: 100%;
}

.last .item .item_title {
  font-size: var(--iframe-font-size-title);
}

.last .item_content {
  color: var(--iframe-gray-color);
  font-size: var(--iframe-font-size-titi);
}

.last .item .item_titi {
  font-size: var(--iframe-font-size-titi);
  color: var(--iframe-gray-color);
}

.info_last {
  display: flex;
  flex-direction: column;
  margin: var(--iframe-margin);
}

@media screen and (min-width: 900px) {
  .info_last {
    flex-direction: row;
    margin: var(--iframe-padding);
  }
}

@media screen and (max-width: 500px) {
  header .icons_input {
    display: none;
    width: 150px;
    height: 20px;
  }
}

/*제목 화살표 버튼*/
.info .data .title_span.buttonText {
  -webkit-line-clamp: 3;
}

.buttonColor {
  color: red;
}

/*입력창 이벤트*/
.serch_header {
  display: none;
  padding: 16px;
  padding-top: 10px;
  background-color: rgb(255, 255, 255);
  align-items: baseline;
}

.fa-arrow-left,
.fafa {
  color: var(--iframe-dark-gray-color);
}

.serch_bt {
  margin: var(--iframe-margin);
}

.serch_input {
  width: 80%;
  height: 20px;
  margin-top: var(--iframe-padding);
  padding-bottom: var(--iframe-margin);
  border: none;
  border-bottom: 1px solid var(--iframe-dark-gray-color);
}

input:focus {
  outline: none;
}

/*자동재생 버튼*/
.last .last_btn.rightMove{
  text-align : right; 
  background-color: rgba(0, 0, 255, 0.541);
}

.wrapper{
  position: absolute;
  width: 50vh;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  display: none;
}
.wrapper.wrapperMenu{
  display: block;
  opacity: 1;
 
}

.wrapper div {
  padding: 15px 20px;
  background-color: #ffffff;
}

.wrapper button {
  display: flex;
  align-items: left;
  width: 100%;
  font-size: var(--iframe-font-size-title);
}
```
