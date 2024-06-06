## How to properly use this

(Assuming you're on linux)

- This is an incredibly niche file and I dont think anyone's going to use it, but here we go

1. Download micro text editor (or any of your choice)
2. Find that text editor with this command (replace micro with yours if you have a different text editor)

```
which micro
```

(should return something like /usr/bin/micro)

3. Rename that text editor file. I renamed mine mic. This can be done by the following commands (you may have to be super user,
so try these with sudo if they dont work)

```
cd /usr/bin
mv micro mic

```

4. Download the file from the github
5. Go to wherever you downloaded that file on your computer and run the command

```
chmod +x micro
```

6. Now you need to move that file to somewhere the computer can see it so run 

```
echo $PATH
```
this will show you where you can put the file on your computer to have it be seen and ran just by
typing micro on your computer

7. Move this file to one of those locations (command should be something like) (again, put sudo before command if needed)

```
mv micro /usr/local/bin
```
8. Almost done, but there are some annoying responses you get from input remapper
if you want to get rid of these you need to edit and remove lines that print the garbage that you
get shown in your terminal


/usr/bin/input-remapper-control


/usr/lib/python3/dist-packages/inputremapper/daemon.py


9. go to the terminal and type

```
micro
```

10. This should now toggle on and off your keybindings when in the text editor
