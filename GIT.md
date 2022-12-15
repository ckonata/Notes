Es un sistema de control de version distribuido.
La informacion se almacena con un sistema de _key:value_, donde se utiliza la _key_ para acceder al _value_.

##### _Key_
Es el hash de los datos a almacenar. Es un **SHA1**: una funcion hash criptografica, que genera un hash de 40 digitos (numero hexadecimal) => A un mismo input, la funcion generara el mismo hash para ese input. Esto significa que a partir del _value_ llego a la _key_, pero tambien a partir del _value_ puedo llegar a esa misma _key_.

Para obtener el hash de un contendio:
`eco 'Hello' | git hash-object --stdin`

##### _Value_
Son los datos a almacenar, **comprimidos** en un blob + metadata, que contiene:
* Identificador del blob
* Tamaño del contenido
* Delimitador `\0` <sub>string terminator en lenguaje C</sub>
* Contenido

![[Pasted image 20221214230258.png]]




hint: Waiting for your editor to close the file... /c/Users/AGT/AppData/Local/Programs/Microsoft VS Code/bin/code: line 28: /Code.exe: No such file or directory error: There was a problem with the editor 'code --wait'. Please supply the message using either -m or -F option.

git config --global core.editor /usr/bin/vim

git config --global core.editor "'C:\Users\AGT\AppData\Local\Programs\Microsoft VS Code\Code.exe' -n -w"

----------------------------------------------------

```
# Please enter the commit message for your changes. Lines starting
# with '#' will be ignored, and an empty message aborts the commit.
# On branch master
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#       deleted:    httpdocs/newsite/manifest/cache/0a432970ba6491fe65dad60b012e5c95_louloumay2011en-1-4dea3186b7f7b.jpg
#       deleted:    httpdocs/newsite/manifest/cache/0a61b5d7a9e97da78fe602e1ad41edb6_5-4dec7c3d57c80.jpg
#       deleted:    httpdocs/newsite/manifest/cache/0afb6a7716a85d0de46cdd03bb30f75f_fifa_panorama_full_page-01_thu-4dea3d1a0e0f5.jpg
#       deleted:    httpdocs/newsite/manifest/cache/0b3bc9be76a5d3e1e36af4b8dcf98658_free2-4df0e2e08761f.jpg
#       deleted:    httpdocs/newsite/manifest/cache/0b6342913b8e599fac76da452af98ec5_si-feb-2009-1-4dea3d1abcb61.jpg
#       deleted:    httpdocs/newsite/manifest/cache/0b9ddc587340f7744e03c4b2dafacf7f_lou-lou-winter-2009-cover-4dea3d1a9b1a0.jpg
#       deleted:    httpdocs/newsite/manifest/cache/0bf64ff8fc22720b3da20d0730fa6a04_chatelaine-dec-2009-4dea3d18daa30.jpg
# 
```

When you run `git commit` with no arguments, it will open your default editor to allow you to type a commit message. Saving the file and quitting the editor will make the commit.It looks like your default editor is Vi or Vim. The reason "weird stuff" happens when you type is that Vi doesn't start in insert mode - you have to hit i on your keyboard first! If you don't want that, you can change it to something simpler, for example:`git config --global core.editor nano` Then you'll load the Nano editor (assuming it's installed!) when you commit, which is much more intuitive for users who've not used a modal editor such as Vi.That text you see on your screen is just to remind you what you're about to commit. The lines are preceded by `#` which means they're comments, i.e. Git ignores those lines when you save your commit message. You don't need to type a message per file - just enter some text at the top of the editor's buffer.To bypass the editor, you can provide a commit message as an argument, e.g.`git commit -m "Added foo to the bar"`

in standart Vi editor in this situation you should

1.  press Esc
2.  type ":wq" (without quotes)
3.  Press Enter

![98b3b4ab9d27ba3b108ace1e58a25824.png](file:///C:/Users/cziemba/.config/joplin-desktop/resources/db0d72a372b04dcbbf3d6a3c973c2860.png)

![cc9d91bc75e1327fcfba83ae7183e460.png](file:///C:/Users/cziemba/.config/joplin-desktop/resources/914ee566c4fa4f48b0a5301c120c6b1e.png)

![53eae6503e0f7dfc900689d8aabaa7d0.png](file:///C:/Users/cziemba/.config/joplin-desktop/resources/4b9d8681321943bea806577c8b838999.png)

![d8da72a078e8f30f203f1d7034241711.png](file:///C:/Users/cziemba/.config/joplin-desktop/resources/531871ef514642199c8ae1a744cb1abd.png)