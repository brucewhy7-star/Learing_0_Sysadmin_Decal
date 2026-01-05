`pwd`-current woring directory

I use `man ls` (notice that it is not `man [ls]`, hahahahaha) to find that `ls -a` or `ls --all` will show entries start with `.`
And using `cat .secret` I get `hunter2`

I `cd nonsense` and see those files. I guess there are ways to see the informations hidden in those file at once. So I use `man ls` again, and I think `ls -h -l` or `ls -Z` (or `ls --context`), `ls -D` to be candidates. But all of them failed.
So I type `man xargs`. But my English is not so good. And I missed. While I go to ChatGPT, then I figure out what does `xargs` do or mean. Then I try `ls | xargs cat`, and I just get `standford > berkeley` which is funny.....("A malicious user" haha)

For remove the `nonsense`, I go to type `cd ..` to go back to `b01`, and I try `rm nonsense` which did not work. So I `man rm` and find `rm -r` will remove directory and their content recursively. So I just type `rm -r nonsense`

For `bag_data.txt`, I knew I shall use `less` command combined with some search function. But, it's too painful to read the full manuscript of `less`, so again, I reach to ChatGPT. And what do is:
1. `less big_data.txt`
2. inside the `less` mode, type `/http`
3. press uparrow twice
And I just find `THE SOLUTION IS MORE COFFEE`. OK, and I even know how to quit `less`, by pressing `q`

For `a_script`, we need execute permission since we are going to execute it. How to do it? I have no idea. Seriously. But the answer is `chmod +x a_script`. Here, `chmod +x` just do the work. By the way, `r` and `w` stand for read and write.
Oh, and the outcome is `Hello World!`

Finally, I need to write a file, I guess I will need some editor. And I just use Vim:
1. `vim hello_world`
2. press `i` to enter the insert mode
3. type my name
4. press ESC to get out of insert mode
5. press `:`+`w` to save the file
6. press `:`+`q` to quit

