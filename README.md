# LIKELIKE Online

The tiniest MMORPG. Choose an avatar and hang out with your friends in a virtual version of [LIKELIKE](http://likelike.org/shows) a videogame gallery in Pittsburgh, PA. Read [a blog post about LIKELIKE Online here](https://www.molleindustria.org/blog/likelike-online/).

This project was created during the COVID-19 quarantine and was meant to evoke the social aspect of LIKELIKE's exhibitions. You can mod it to create your own virtual exhibitions, multi-user environments or games. It's designed to be extensible by just editing the data.js file and a few settings at the beginning of server.js and client.js.  

The code is extensively commented but it was put together very quickly (about a 10 days) so it's not meant to be a robust, beginner-friendly tool. You'll need some node.js and javascript knowledge to adapt it to your needs. Use at your own risk.

LIKELIKE Online is built with node.js, socket.io, [p5.js](https://p5js.org/), and the add-on [p5.play](https://molleindustria.github.io/p5.play/). It was formerly hosted on [glitch.com](https://glitch.com/) (RIP).  

LIKELIKE Online is a project by [Molleindustria](http://molleindustria.org/).  

Licensed under a GNU Lesser General Public License v2.1.

![](promo.gif)

## The .env file

.env is a text file in the root folder that contains private variables, in this case admin usernames and passwords and the port used by the project. It's not published on github and it's not automatically published on glitch so you may have to create it manually and/or copy paste the content in the glitch editor and/or in your code editor if you are running is as a local project.

An example of .env file for LIKELIKE online is:

```javascript
ADMINS=adminname1|pass1,adminname2|pass2  
PORT = 3000
```

The admin names are reserved. Logging in as "adminname|pass" (nickname and password separated by a "|") will grant the user admin priviledges such as banning IP or sending special messages.
