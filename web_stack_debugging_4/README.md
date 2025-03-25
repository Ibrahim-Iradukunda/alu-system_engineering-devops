Task 0 - Sky is the Limit, Let’s Bring That Limit Higher:
Benchmark with ApacheBench: Use ab to test the server with 2000 requests, 100 concurrent. Initially, there are many failed requests (943).

Identify the Issue: Investigate the cause (e.g., insufficient resources, Nginx misconfiguration, PHP-FPM issues).

Fix the Issue: Adjust Nginx or PHP-FPM settings (e.g., increase worker processes, adjust buffer sizes).

Automate with Puppet: Write a Puppet manifest (0-the_sky_is_the_limit_not.pp) to automate the configuration changes.

Test Again: Re-run the ApacheBench test to confirm no failed requests and improved performance.

The task should end with zero failed requests and better performance under load.




