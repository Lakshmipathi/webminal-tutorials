title: Урок2 - Создание файлов, просмотр содержимого и состояния

### Урок2 - Создание файлов, просмотр содержимого и состояния

На первом уроке Вы научились создавать каталоги.

Давайте научимся как создать новый файл,

    touch file1.txt

нажмите Ввод и читайте дальше :)

----

title: touch

команда touch создает новый файл или 
меняет временную метку существующего.
Теперь попробуем снова,

	touch  file1.txt

на этот раз будет изменено время создания/последнего доступа и изменения на текущее.

	touch file2.txt

создаст пустой новый файл, если он еще не был создан.
Для просмотра содержимого каталога Вы также можете использовать

        dir
title: dir


`dir` служит для перечисления содержимого каталога.
Да, Вы верно догадались, команда `dir` аналогична `ls -C -b` (Знаю, Вы не догадались :P)


that is, by default files are listed in columns, sorted vertically,
and special characters are represented by backslash escape sequences.
To clear a screen,the command is

	clear

title: clear

Viola! terminal screen is cleared!!!
Lets print some message on the terminal,

	echo "hello" 
title: echo

Cool! the message is displayed on the screen.
Lets redirect the message to a new file instead 
of screen.

	echo "hello" > hello.txt 

To append  data you must use &gt;&gt; not just &gt;

	echo "linux" >> hello.txt 
	echo "world" >> hello.txt

Done.To view the file content ,do 

	cat hello.txt 

title: cat

so now you have viewed the file content.`cat` is 
used to display the entire file content.<br/>


To view only first two lines from the file

	head -2 hello.txt



title: head

see,it showed us first two lines from files.
By default,`head` will display the first 10 lines when you run,

	head hello.txt 

Now how to view last two lines?.Its simple,use `tail`

	tail -2 hello.txt


title: tail

cool. Thus `head` will be used to display
lines from begining and `tail` will be 
used to display last few lines. As with `head` 

	tail hello.txt

by default will display last 10 lines from the line.

Lets check some stats of the files and directories
we have create so far.

	stat hello.txt

title: stat

carefully examine few important fields the output. The first line
shows the `filename`.second line says its a `regular file` with
size as `18`.Third  line shows `Inode` number and no.of `links`
to that inode.

Fourth one,says `owner(Uid),group(Gid)` who has read-write permission
but other have read permission.Final three lines show `access,modified 
and change` time.They mean:

	access - when the file was last accessed/read.
	modified - when the contents was last 
		 modified written.
	change - denotes changes to files metadata
		like changing user permission.


Now lets do a `stat` on directory.

	stat dir1

Compare the previous `stat` "hello.txt" output with "dir1",before you move.
especially find out "dir1" type.That marks the end of lesson2!.Well done.

Now  move to lesson3.

