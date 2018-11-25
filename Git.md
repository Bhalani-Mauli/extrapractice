### 1. Git is version control tool

### 2. if we have more developers working on same project so we have different code coming from different people from same project.

### 3. how we use it ?
- Step by Step
    - git is super easy
    - git has simple commands that can be self Explainantory
    - **add , commit , pull , push , status , clone , log , checkout , merge ,rebase , stash ,etc.**
    reference : https://git-scm.com/docs

    - So every developer can create their own branch and they will merge it to master branch .
    - So ---is time so as we go left to right time is passing.
    - lets see what it try's to tell us.
    ##### Explainantion
    - We have Git .We have default master branch.
    - we have 2 developers.
    - they created different branch and working on it.
    - after some time they merged their new code with master branch.
    - Our Aim here is to Every developer should work on anything in branch so we can have clean and good and working code in master.
    - It will look good at master so anyone can check and look at it and they will find it more readable

```js
                                                 ______working Developer -2______
                                                /                                \
    Master---------------------------------------------------------------------------->Time.
             \____working developer-1_____/
```

- so here we have default Master branch and these are branches that developer 1 and 2 are working 
- So they can work seperately and then merge their branch to master.


### Now what happens if one merge and other is still working.(Merge-Conflict issue)
```js
                      ______working Developer -2______
                     /                                \                             
    Master---------------------------------------------------------------------->Time.
             \____working developer-1_____/
```
- Step by Step
    - So One created a branch from a master so at that time he has the same code as master.
    - Now 2nd created a branch after some time and he is working on his branch.He also has the
    same code as master has at that time.
    - Now 1 is done with his development and merged his new code with master.
    - 2 is still working on his task and after finishing up his task he cannot merge his branch
    with master because master has some new changes that is done by developer 1.
    - so in order to merge 2's branch he need to take the update from master by git pull origin master
    and then he might have some conflict with the code that he has and the code that master has.
    ex.
        ```js
        let a=10;
        a=a+2;
        console.log(a);
        ```
        so if developer 1 changed with to `a=12`
        and developer 2 change it to `20`
        then it will show 2nd developer as conflict and he can decide which to keep.
    after solving all conflicts like the example developer 2 can merge his code to master.

### 4. How we can improve ?
- 10000 Times : Practice makes a man perfect.


