## Create blog on gitHub with jekyll ##
### jekyll environment-local config for MacOS or Linux      
[Click here](http://pizida.com/technology/2016/03/03/use-jekyll-create-blog-on-github/)

###jekyll environment-local config for windows ###
- install ruby  
  1)[download rubyinstall for windows](http://rubyinstaller.org/)  
  2)click next till complete the installing.(select:Add Ruby executables to your PATH)  
  3)verify install result:  
      **cmd:**```ruby v```
- create blog station  
  1) **cmd:**```jekyll new jekyllTest01 ```  
     *If you meet the question as following:
      It looks like you don't have bundler or one of its dependencies installed.*  
   
     slove it:  
      **cmd:**```gem install bundler```  
- Start Built-in Server  
   **cmd:**```cd jekyllTest01```  
   **cmd:**```jekyll serve```
  
- use jekyll to write blog  
  1)file:YEAR-MONTH-DAY-title.MARKUP  
  2)head:  

     --- 
			---
            layout: post  
			title:  "Jekyll/Github create Personal blog"  
			date:   2016/12/29 20:03:42  
			categories: original  
            ---
	  ---  
  3)save in _posts dir    

- refresh th pages  
**cmd:**```jekyll build```  

###Create blog on the github 
1）create new Repossitory for blog on the gitHub:gitTest01  
2) select Publish page demo：  
        *https://qfyxixi.github.io/gitTest01/*  

###Deploy local blog to the remote repository   
1) ```mkdir test01```  
2) ```cd gitTest01```  
3) ```git init```  
4) ```git checkout --orphan gh-pages```  
5)copy /c/jekyllTest01/* to this /C/gitTest01/  
6)```git add .```  
7)```git commit -m "first post"```  
8)```git remote add origin https://github.com/username/gitTest01.git```  
9)```git push origin gh-pages```  

###Pull remote repository to local 

1)set the passcode  
  ```SSH Key：$ ssh-keygen -t rsa -C "XXX@XX.com"```  
2)create id_rsa:according to the hint  
3)add the id_rsa.pub to the git ssh-key  
4)download to local  ```git clone git@github.com:XXX/gitTest01.git```


  




   

    




