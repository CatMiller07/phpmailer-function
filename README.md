phpmailer-function
==================

Custom function to send emails using phpmailer

How to use ?
Add class.phpmailer.php and class.smtp.php in the directory. In the code of sendmail.php, make sure you have added your smtp details.
for instance you can use your Google account as well. Just add your email ID and passoword in the code.
<code>
<?php
      include("sendmail.php");
      $to       =   "some email";
      $subject  =   "Hello";
      $message  =   "hello <i>how are you.</i>";
      $name     =   "Shahid Shaikh";
      $mailsend =   sendmail($to,$subject,$message,$name);
      if($mailsend==1){
        echo '<h2>email sent.</h2>';
      }
      else{
        echo '<h2>There are some issue.</h2>';
      }
?>
</code>
