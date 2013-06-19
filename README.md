commit-msg-hook
===============

*A repo to test the git commit-msg hook.*


I wanted to test the git commit-msg hook to see if I could fail a commit if the commit message was 
formatted incorrectly. In my test a correctly formatted commit message should have the word 
Issue, a dash, a number, and then some text.

   Example:

      Issue-123 Added some cool new feature.


#####To test the hook:

1. Copy the commit-msg file and put it in the .git/hooks directory
2. Make a modification to the someText.txt file
3. Try to commit without an Issue-####.  
4. The commit should be rejected because of an incorrect commit message format
5. Try to commit with the correct format and it should work as it normally does