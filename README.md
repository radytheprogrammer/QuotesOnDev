# QuotesOnDev


Sample API call using RESTapi from the client computer

$(function() {

    //this is your event listener
    
    $('.randomQuote').on('click', function(e) 
    
      $.ajax({
      
        method: 'get',
        url:
          red_vars.rest_url + 'wp/v2/posts?filter[orderby]=rand&filter[posts_per_page]=10'

      }).done(function(data) {
        console.log(data);
      });
    });
  });

})(jQuery);

# C.R.U.D
Create, read, update and delete
method: 'get' translates to read data from the user's browser and evaluate that to query the databse for a new post

#document.ready function syntax. Used if you want to write jQuery code to handle an event listening
(function($) {

} ) (jQuery);


#Learnings
- Ajax is an asynchronous call to the API that returns a data object
- nonces are a security feature and are the new way of validationg an API request by a user
- WordPress can be used as a CMS where a developer can make API requests to get the posts and display them on the homepage

##Functions used so far:
- WP_Query()
- get_post_thumbnail()


### Technologies used:
- WordPress
- Yarn, Gulp, node.js
