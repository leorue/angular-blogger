<h1>angular-blogger</h1>

<h4>An AngularJS blog template interfacing with the Blogger API</h4>


<h3>Setup Blogger Account</h3>
<br/>
First you need a Google Account assuming most people have them from various Google Apps, then visit <a href="http://www.blogger.com">Blogger.com</a> and agree to the terms and having a blogger account.
<br/>
<br />
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/blog-1.png" align="left" width="800" ><br/>



<h3>Create a New Blog</h3>
<br/>
Next create a blog and name it something logical.
<br/>
<br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/blog.png" align="left" width="800" ><br/>


<h3>Create a Few Blog Posts</h3>
<br/>
Then create a few posts I like to chack on the HTML and add an img-resonsive class to any images so they show up responsive on the blog.
<br/>
<br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/blog-2.png" align="left" width="800" ><br/>



<h3>Create a new Google Developer Project</h3>
<br/>
Then visit the <a href="https://developers.google.com/">Google Developer Console</a> and agree to terms. Then create a new project and name it to identify with your blog.
<br/>
<br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/dev-1.png" align="left" width="800" ><br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/dev.png" align="left" width="800" ><br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/dev-2.png" align="left" width="800" ><br/>



<h3>Enable Blgger API</h3>
<br/>
Then go to the API & auth tab and search for the Blogger API v3 and change the status to "On".
<br/>
<br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/blog-3.png" align="left" width="800" ><br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/dev-3.png" align="left" width="800" ><br/>


<h3>Get Google API Key</h3>
<br/>
Then select the credentials tab and create a new Public API accesss key with browser permissions. If you have a specific domain you want to restrict the key to then you can type the domain. I would not do this until you go production for testing purposes. Save the key to inject in the code in a later step.
<br/>
<br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/key.png" align="left" width="800" ><br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/key-1.png" align="left" width="800" ><br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/key-2.png" align="left" width="800" ><br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/key-3.png" align="left" width="800" ><br/>


<h3>Get Blogger ID</h3>
<br/>
Next go back to your blogger account and select the blog you would like to debut on your site. In the URL on the admin screen you will see blogID=<some-number-set>. Save the blog ID to inject into the code in a later step.
<br/>
<br/>
<img src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/blog-1.png" align="left" width="800" ><br/>


<h3>Set Blog ID and API Key</h3>
<br/>
Get the Angular-Blogger, AngularJS project running with a server. Go to the app.js file in the JS folder. Inject the blogID and API Key retrived earlier in the Blog factory in the following URL: https://www.googleapis.com/blogger/v3/blogs/<blogID>/posts?&key=<API-Key>
<br/>
<br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/app.png" align="left" width="800" ><br/>


<h3>Setup Disqus</h3>
<br/>
Next visit <a href="https://www.disqus.com/">Disqus</a> and create an account if you don't already have one. Then click the <a href="https://disqus.com/admin/create/">for webistes</a> tab and create a new blog instance.
<br/>
<br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/comment.png" align="left" width="800" ><br/>


<h3>Add Disqus Short Name</h3>
<br/>
Upon Completion select the universal website code and under number 1 find the "var disqus_shortname = "<your-shortname>" grab the shortname from the code fragment and save it to inject into the post.html file in the pages folder. Save this in the variable disqus-shortname="<your-shortname>".
<br/>
<br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/comment-1.png" align="left" width="800" ><br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/comment-2.png" align="left" width="800" ><br/>


<h3>Add Disqus DNS Link</h3>
<br/>
Next in the app.js file change the postURL in the postsController to reflect where you are serving your blog out of.
<br/>
<br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/app-1.png" align="left" width="800" ><br/>


<h3>Edit Title</h3>
<br/>
Finally in the app.js file edit the title and description of the blog in the mainController to something which reflect the theme of your blogs content. 
<br/>
<br/>
<img class="img-responsive" src="https://raw.githubusercontent.com/leorue/angular-blogger/master/images/docs/app-2.png" align="left" width="800" ><br/>