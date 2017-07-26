## Python Exception Chains (or Trees)  
Originally published: 2012-09-04 15:57:51  
Last updated: 2013-02-04 15:15:22  
Author: Alfe   
  
I have here an approach for chaining exceptions in case a lower layer (*library*) raises an exception which is caught in an upper layer (*application*) and later given as *cause* when a different exception is raised.  Passing this *cause* exception is meant to offer access to the stack trace of the inner exception for debugging.