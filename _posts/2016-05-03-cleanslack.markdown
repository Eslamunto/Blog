---
layout:     post
comments:	true
title:      "Solving a Slack Problem"
subtitle:   "My very first open source contribution"
date:       2016-05-03 16:00:00
author:     "Eslam Maged"
header-img:	"img/post-bg-04.jpg"
description:	"First but not last open source contribution"
---


<p>Final exams period is the period of time when I realize how beautiful the ceiling in our apartment is. I just keep staring at it doing nothing; because come on! Who studies for the final exams any way? Here is when the concept of doing something interesting came into  mind!</p>

<p>Have you ever heard about <a href="https://slack.com/" target="_blank">Slack</a>?</p>

<p>Slack is the AWESOME messaging service developed by a great team to help other amazing teams communicate easily. I am a big fan of the product and I have previously developed our sexy slack bot, <a href="http://eslamaged.com/blog/2016/02/02/lucy/" target="_blank">Lucy</a>.</p>

<p>At the lovely startup I am currently working for, we depend heavily on Slack for day to day communication, for making polls, organizing or announcing events and of course sharing huge media files. But we had a problem... since we were using slack on a free-tier; we consume our free 5GB of media every 2-3 months and since Slack does not provide a "delete-all" button. Some days this was my morning text;</p> <img src="/img/clearslack/slackmsg.png" /> 

<p>Our team members had to go through their files one by one in order to free some storage. Of course that was a lot of time wasted!</p>


<p>The first thing that would come to the mind of a developer is to check the Slack developer API for a file deletion method and of course they had it :-) A python script was written that I used to run through my terminal. However, to help other workmates delete their files as well, I had to ask them for their tokens to be submitted in a Google form and then I had to go through the form results, one by one, and replace tokens in the code in order to delete the files for a specific user. After that long process, I had to re-ask them to generate new tokens for security reasons.</p>


<p>Two weeks ago, our smart <a href="https://twitter.com/MohamedBassem" target="_blank"> Bassem</a> proposed running the script from the browser. If our team members could have such a tool, that would save me from the long process and also their tokens would not leave their very own browsers. That's not only safe, but it also saves me a lot of time! Based on his suggestion, AngularJS was chosen as a frontend framework for executing the script and handling the calls to the slack API. The project is hosted on <a href="https://pages.github.com/" target="_blank">GitHub pages</a> and the code is open sourced. Feel free to request adding a feature or contribute to the code.
</p>

<p>We also believe that you might find this project helpful. Feel free to empty your slack storage whenever needed without having to go through your files one by one ;-)</p>


<p>Here is the link to the project <a href="http://clearslack.com/#/" target="_blank">http://clearslack.com</a></p>

<p> Last but not least, @Bassem, thanks for the idea, the motivation and for reviewing this post.</p>

<p><a href="https://twitter.com/Amal_Shaker">@Amal</a>, thank you for fixing my grammatical mistakes.</p>

<div id="disqus_thread"></div>
<script>
    /**
     *  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
     *  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables
     */
    /*
    var disqus_config = function () {
        this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
        this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
    };
    */
    (function() {  // DON'T EDIT BELOW THIS LINE
        var d = document, s = d.createElement('script');
        
        s.src = 'https://eslamaged.disqus.com/embed.js';
        
        s.setAttribute('data-timestamp', +new Date());
        (d.head || d.body).appendChild(s);
    })();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript" rel="nofollow">comments powered by Disqus.</a></noscript>
