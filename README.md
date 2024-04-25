<body>
  <img fill="none">
    <style>
      @charset "UTF-8";
      *:focus {
        outline: none !important;
      }
      /*
      Original forked from following user
      https://codepen.io/levise*/
      body {
        background-color: #C8C2AA;
        background-size: 4px 4px;
        background-image: linear-gradient(90deg, transparent, transparent 3px, rgba(0, 0, 0, 0.07) 4px), linear-gradient(transparent, transparent 3px, rgba(0, 0, 0, 0.07) 4px);
        color: #4D493E;
        font-family: "Noto Sans", sans-serif;
        font-weight: 300;
        margin: 0;
        min-height: 100vh;
        box-shadow: inset 0 0 150px rgba(77, 73, 62, 0.4), inset 0 0 150px rgba(77, 73, 62, 0.3);
        display: flex;
        min-height: 100vh;
        flex-direction: column;
        letter-spacing: 0.1rem;
      }
      .container {
        padding: 0 4rem;
      }
      header {
        padding: 1rem 0;
      }
      h1 {
        text-transform: uppercase;
        font-weight: 300;
        letter-spacing: 0.7rem;
        text-shadow: 0.3rem 0.3rem 0 rgba(77, 73, 62, 0.3);
      }
      h1 span {
        margin-right: -0.7rem;
      }
      h1 small {
        font-weight: 500;
        text-transform: none;
        text-shadow: none;
        letter-spacing: 0.1rem;
      }
      h1 small::before {
        content: "–";
      }
      .pattern {
        border-top: 2px solid #4D493E;
      }
      .pattern-inner {
        height: 40px;
        background-size: 50px 3px, 50px 1px, 50px 1px, 50px 1px, 50px 1px, 50px 1px, 50px 1px, 50px 1px, 50px 1px;
        background-position: 0 0, 22px 4px, 22px 5px, 22px 6px, 22px 7px, 28px 12px, 28px 13px, 28px 14px, 28px 15px;
        background-image: linear-gradient(90deg, #4D493E, #4D493E 10px, transparent 10px), linear-gradient(90deg, rgba(77, 73, 62, 0.4), rgba(77, 73, 62, 0.4) 1px, rgba(77, 73, 62, 0.8) 1px, rgba(77, 73, 62, 0.8) 2px, rgba(77, 73, 62, 0.9) 2px, rgba(77, 73, 62, 0.9) 3px, rgba(77, 73, 62, 0.4) 3px, rgba(77, 73, 62, 0.4) 4px, transparent 4px, transparent 12px, rgba(77, 73, 62, 0.4) 12px, rgba(77, 73, 62, 0.4) 13px, rgba(77, 73, 62, 0.8) 13px, rgba(77, 73, 62, 0.8) 14px, rgba(77, 73, 62, 0.9) 14px, rgba(77, 73, 62, 0.9) 15px, rgba(77, 73, 62, 0.4) 15px, rgba(77, 73, 62, 0.4) 16px, transparent 16px), linear-gradient(90deg, rgba(77, 73, 62, 0.9), rgba(77, 73, 62, 0.9) 1px, #4d493e 1px, #4d493e 2px, #4d493e 2px, #4d493e 3px, rgba(77, 73, 62, 0.9) 3px, rgba(77, 73, 62, 0.9) 4px, transparent 4px, transparent 12px, rgba(77, 73, 62, 0.9) 12px, rgba(77, 73, 62, 0.9) 13px, #4d493e 13px, #4d493e 14px, #4d493e 14px, #4d493e 15px, rgba(77, 73, 62, 0.9) 15px, rgba(77, 73, 62, 0.9) 16px, transparent 16px), linear-gradient(90deg, rgba(77, 73, 62, 0.9), rgba(77, 73, 62, 0.9) 1px, #4d493e 1px, #4d493e 2px, #4d493e 2px, #4d493e 3px, rgba(77, 73, 62, 0.9) 3px, rgba(77, 73, 62, 0.9) 4px, transparent 4px, transparent 12px, rgba(77, 73, 62, 0.9) 12px, rgba(77, 73, 62, 0.9) 13px, #4d493e 13px, #4d493e 14px, #4d493e 14px, #4d493e 15px, rgba(77, 73, 62, 0.9) 15px, rgba(77, 73, 62, 0.9) 16px, transparent 16px), linear-gradient(90deg, rgba(77, 73, 62, 0.4), rgba(77, 73, 62, 0.4) 1px, rgba(77, 73, 62, 0.8) 1px, rgba(77, 73, 62, 0.8) 2px, rgba(77, 73, 62, 0.9) 2px, rgba(77, 73, 62, 0.9) 3px, rgba(77, 73, 62, 0.4) 3px, rgba(77, 73, 62, 0.4) 4px, transparent 4px, transparent 12px, rgba(77, 73, 62, 0.4) 12px, rgba(77, 73, 62, 0.4) 13px, rgba(77, 73, 62, 0.8) 13px, rgba(77, 73, 62, 0.8) 14px, rgba(77, 73, 62, 0.9) 14px, rgba(77, 73, 62, 0.9) 15px, rgba(77, 73, 62, 0.4) 15px, rgba(77, 73, 62, 0.4) 16px, transparent 16px), linear-gradient(90deg, rgba(77, 73, 62, 0.4), rgba(77, 73, 62, 0.4) 1px, rgba(77, 73, 62, 0.8) 1px, rgba(77, 73, 62, 0.8) 2px, rgba(77, 73, 62, 0.9) 2px, rgba(77, 73, 62, 0.9) 3px, rgba(77, 73, 62, 0.4) 3px, rgba(77, 73, 62, 0.4) 4px, transparent 4px), linear-gradient(90deg, rgba(77, 73, 62, 0.9), rgba(77, 73, 62, 0.9) 1px, #4d493e 1px, #4d493e 2px, #4d493e 2px, #4d493e 3px, rgba(77, 73, 62, 0.9) 3px, rgba(77, 73, 62, 0.9) 4px, transparent 4px), linear-gradient(90deg, rgba(77, 73, 62, 0.9), rgba(77, 73, 62, 0.9) 1px, #4d493e 1px, #4d493e 2px, #4d493e 2px, #4d493e 3px, rgba(77, 73, 62, 0.9) 3px, rgba(77, 73, 62, 0.9) 4px, transparent 4px), linear-gradient(90deg, rgba(77, 73, 62, 0.4), rgba(77, 73, 62, 0.4) 1px, rgba(77, 73, 62, 0.8) 1px, rgba(77, 73, 62, 0.8) 2px, rgba(77, 73, 62, 0.9) 2px, rgba(77, 73, 62, 0.9) 3px, rgba(77, 73, 62, 0.4) 3px, rgba(77, 73, 62, 0.4) 4px, transparent 4px);
        background-repeat: repeat-x;
      }
      button {
        cursor: pointer;
        font: inherit;
        border: none;
        padding: 0.4rem 1rem;
        background-color: rgba(77, 73, 62, 0.35);
        color: #4D493E;
        box-sizing: content-box;
        position: relative;
        border: 1px solid transparent;
        border-left: none;
        border-right: none;
      }
      button::before {
        content: "";
        position: absolute;
        z-index: -1;
        left: 0;
        top: 3px;
        bottom: 3px;
        width: 0;
        background-color: #4D493E;
        transition: width 0.2s;
      }
      button::after {
        content: "";
        display: none;
        position: absolute;
        background: #4D493E;
        width: 100%;
        height: 2px;
        left: 0;
        bottom: -4px;
      }
      button:hover, button:focus {
        background-color: transparent;
        color: #C8C2AA;
        border-color: #4D493E;
      }
      button:hover::before, button:focus::before {
        width: 100%;
      }
      main {
        flex: 1;
      }
      .content {
        padding-left: 4rem;
        background-image: linear-gradient(90deg, rgba(77, 73, 62, 0.2), rgba(77, 73, 62, 0.2) 14px, transparent 14px, transparent 20px, rgba(77, 73, 62, 0.2) 20px, rgba(77, 73, 62, 0.2) 23px, transparent 23px);
        margin-bottom: 2rem;
      }
      img {
        box-shadow: 3px 3px 0 rgba(77, 73, 62, 0.6);
      }
    </style>
  </img>
<table border="0">
  <tr>
    <td>
      <img height="auto" width="100%" class="center" src="https://static.wikia.nocookie.net/meme/images/1/15/Wine.gif/revision/latest?cb=20171029023215">
    </td>
    <td>
      <table>
        <tr>
          <td>
            <img width="100%" src="https://github-readme-stats.vercel.app/api/top-langs?username=tniromin&show_icons=true&locale=en&layout=compact&theme=tokyonight" alt="tniromin" />
          </td>
        <tr>
          <td>
            <img width="100%" src="https://github-readme-stats.vercel.app/api?username=tniromin&show_icons=true&locale=en&theme=tokyonight" alt="tniromin" />
          </td>
        </tr>
       </table>
     </td>
   </tr>
</table>
</p>

<h3 align="middle">[Under Construction]---LULZ &nbsp;&nbsp;
<!--<img src="https://www.freeiconspng.com/uploads/construction-icon-11.png" width="70" alt="Construction Symbols" /> 
  Image taken down cause it doesnt suite the page
--> </h3>

<!--<h1 align="center">Hi 👋, I'm Thimira Niromin</h1>
<h3 align="center">A Developer and linux user from Sri Lanka</h3>-->
<a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"><img width="100%" src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif"></a>
<p align="left">
  <a href="https://github.com/ryo-ma/github-profile-trophy">
    <img width="100%" src="https://github-profile-trophy.vercel.app/?username=tniromin&theme=tokyonight" alt="tniromin" />
  </a> 
</p>

<a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"><img width="100%" src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif"></a>

<h3 align="left">Connect with me:</h3>
<p align="left">
  <a href="https://linkedin.com/in/thimira-niromin" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="thimira-niromin" height="30" width="40" /></a>
  <a href="https://www.hackerrank.com/@tniromin2" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/hackerrank.svg" alt="@tniromin2" height="30" width="40" /></a>
</p>

<a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"><img width="100%" src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif"></a>

<h3 align="left">Languages and Tools:</h3>
<p align="left">
  <a href="https://www.gnu.org/software/bash/" target="_blank" rel="noreferrer">
    <img src="https://www.vectorlogo.zone/logos/gnu_bash/gnu_bash-icon.svg" alt="bash" width="40" height="40"/>
  </a>
  <a href="https://www.blender.org/" target="_blank" rel="noreferrer">
    <img src="https://download.blender.org/branding/community/blender_community_badge_white.svg" alt="blender" width="40" height="40"/>
  </a>
  <a href="https://www.cprogramming.com/" target="_blank" rel="noreferrer">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="c" width="40" height="40"/>
  </a>
  <a href="https://www.w3schools.com/cpp/" target="_blank" rel="noreferrer">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="cplusplus" width="40" height="40"/>    
  </a>
  <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/>
  </a>
  <a href="https://www.docker.com/" target="_blank" rel="noreferrer"> 
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="40"/> 
  </a> 
  <a href="https://golang.org" target="_blank" rel="noreferrer"> 
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/go/go-original.svg" alt="go" width="40" height="40"/> 
  </a> 
  <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> 
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/>
  </a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> 
  </a> 
  <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> 
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> 
  </a> 
  <a href="https://postman.com" target="_blank" rel="noreferrer"> 
    <img src="https://www.vectorlogo.zone/logos/getpostman/getpostman-icon.svg" alt="postman" width="40" height="40"/> 
  </a> 
  <a href="https://www.python.org" target="_blank" rel="noreferrer"> 
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> 
  </a>
</p>

<a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"><img width="100%" src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif"></a>



<!--
**tniromin/tniromin** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
</body>