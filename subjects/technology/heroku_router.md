- DNS
    Dns resolves domain to heruko target
- Heroku
    Add domain on heruko
- Heroku router (2.0)
    Load balancer to route traffic to dyno
    Router 2.0 uses HTTP2.0, HTTP/2 traffic from the client terminates at the Heroku router, and Heroku forwards HTTP/1.1 from the router to your application (dyno)

https://www.heroku.com/blog/tips-tricks-router-2dot0-migration/


3 Different ways to Inspect Router Version
- Inspect HTTP headers
				curl --head https://risingteam-kit.herokuapp.com
				https://www.heroku.com/blog/tips-tricks-router-2dot0-migration/#http-headers
				If the application is behind an external proxy, or CDN, headers might be stripped, 
				hence need to check 	xxx.herokuapp.com
- Check Application Logs
				heroku logs -a risingteam-kit --source heroku    
				and look for heroku[router]
				https://www.heroku.com/blog/tips-tricks-router-2dot0-migration/#logs
- Heruko Command
    heroku features:info http-routing-2-dot-0 -a <app name>


Migration could happen automatically.
Voluntary Migration/Validation (alternative is this, more controlled)
heroku features:enable http-routing-2-dot-0 -a <app name>
heroku ps:restart


Several Disable Options 
- Disable Router 2.0 
	heroku features:disable http-routing-2-dot-0 -a <app name>
	above basic tier has this capability.
- Disable Http2 (from browser to router)
	heroku labs:enable http-disable-http2 -a <app name>
- Disable keepalive
	heroku labs:enable http-disable-keepalive-to-dyno -a <app name>


https://devcenter.heroku.com/articles/http-routing#router-2-0-logs