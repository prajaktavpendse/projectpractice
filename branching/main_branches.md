# The main branches 

![Git main branches](https://github.com/prajaktavpendse/projectpractice/blob/master/Images/main_branches.PNG)



The central repo holds two main branches with an infinite lifetime:     
                                                                          
*1. master*                                                              
*2. develop*                                                                
                                                                          
The **master branch** at origin should be familiar to every Git user.Parallel to the master branch, another branch exists called **develop**.    
                                                                          
We consider **origin/master** to be the main branch where the source code of HEAD always reflects a production-ready state.   
                                                                          
We consider **origin/develop** to be the main branch where the source code of HEAD always reflects a state with the latest delivered development changes for the next release.                       
                                                                          
When develop branch reaches a stable point and is ready to be released,all of the changes should be merged back into master somehow and then tagged with a release number.