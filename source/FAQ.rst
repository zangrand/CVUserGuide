..    include:: <isonum.txt>

Frequently Asked Questions
==========================


-  I get this error when accessing via SSH my virtual machine:

   ::

       @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@                         
       @    WARNING: REMOTE HOST IDENTIFICATION HAS CHANGED!     @                         
       @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@                         
       IT IS POSSIBLE THAT SOMEONE IS DOING SOMETHING NASTY!                               
       Someone could be eavesdropping on you right now (man-in-the-middle attack)!         
       It is also possible that the RSA host key has just been changed.                    
       The fingerprint for the RSA key sent by the remote host is                          
       c8:1b:1d:37:61:ee:9f:e4:db:5b:31:91:35:7b:d2:59.                                    
       Please contact your system administrator.                                           
       Add correct host key in /home/user/.ssh/known_hosts to get rid of this message.     
       Offending key in /home/user/.ssh/known_hosts:3                                      
       RSA host key for 10.64.51.7 has changed and you have requested strict checking.     
       Host key verification failed.                                                       


   SOLUTION: the IP of your VM has probably been reused. You need to
   update the relevant entry on your */home/user/.ssh/known\_hosts* file.
   Please run:

   ::

       ssh-keygen -R 10.64.51.7                                                                                                    

   and try again.



-----------------------------------------------------


