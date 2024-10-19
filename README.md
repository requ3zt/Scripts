# BRUTE FORCE EXPLOIT FOR XMLRPC.PHP


A scirpt in Bash which we will use the 'curl' tool to send XML-RPC requests to the xmlrpc.php file of the WordPress website. Through the wp.getUsersBlogs method, we will send an XML structure containing the username and password to be tested.

If the credentials are incorrect, the server will respond with an error message indicating that the credentials are invalid. However, if the credentials are valid, the server's response will be different and will not include the error message.

In this way, we can use the server's response to determine when we have found valid credentials and thus gain access to the compromised WordPress site.

The wp.getUsersBlogs method is not the only existing method, not the only vulnerability in xmlrpc.php. There are other methods such as wp.getUsers, wp.getAuthors, or wp.getComments, among others, that can also be used by attackers to perform brute force attacks and compromise the security of the WordPress site.

IMPORTANT!!!

*Before you use this script it's necesary to know the user for the login! If you want to extract the usernames of the WordPress page I recomend to use the tool **wpscan***
