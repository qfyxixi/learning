## git command ##

### commit ###

- **normal commit** 

   
    ```$git add .(filename)```      
    ```$git commit -m 'message'```      
    ```$git push origin branchname```

- **special commit**

    *hint:*    
    *Updates were rejected because the tip of your current branch is behind*       
    **There are three method to slove it**
    
    1)force push

    ```$git push -u origin branchname -f```  
   
    2)merge local branch
   
    ```$ git pull origin branchname```  
    ```$ git push -u origin branchname```
   
    3)save current branch

    ```$ git branch branchname_new```      
    ```$ git push -u origin branchname_new```  


    



