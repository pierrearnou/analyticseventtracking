analyticseventtracking
======================
// Add Google Analytics basic code
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

  ga('create', 'UA-44845359-1', 'wildfireapp.com');
  ga('send', 'pageview');

ga('create', 'UA-44845359-1', 'wildfireapp.com');
ga('send', 'pageview');

// Track tour Learn More click
$(document).on('click', '.track-link', function () {
  console.log('Tracked a Tour link: ' + $(this).attr('href'));
  ga('send', 'event', 'Tour Links', 'click', $(this).attr('href'));
});
