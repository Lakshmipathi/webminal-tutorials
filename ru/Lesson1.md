title: Lesson1 - Basic commands to navigate directories 

### Урок 1 - Основные команды навигации по файловой системе

Просто наберите 

    $ pwd


нажмите Ввод и прочтите результат выполнения комманды :)
title: pwd

Видите нечто похожее на */home/yourname* ? Здорово, Вы определили текущий каталог.
Поздравляем! Вы вступили в экслюзивный клуб пользователей командной строки linux :)

Как Вы уже поняли, команда

     pwd


покажет текущий каталог. Ага, Ваш дом - каталог.

Теперь попробуем создать новый каталог. Введите следующую команду

    mkdir -v dir1

и нажмите Ввод.
title: mkdir

Появилось сообщение?

*`mkdir: created directory dir1`*

Круто, теперь Вы создали новый каталог. Предположим Вы хотите создать более одного каталога

Wow,now you created a new  directory. Lets say you want to create more than 
one directory instead of invoking mkdir multiple(three) times-like.

	mkdir -v dir2
	mkdir -v dir2/dir3
	mkdir -v dir2/dir3/dir4
you can simply use 

	mkdir -vp dir2/dir3/dir4

"-p" option will create parent directories for "dir4" as needed.
In this case,it creates dir2,dir3 automatically.Now we have created 
4 directories.How to view them?

To view type 'ls' and press enter

	ls

title: ls

listed `dir1 dir2` as directory content right? Thats exactly what we wanted

	`dumb tutor: yes,the guy with blue-t-shirt,
		   Yeah, you ,why you look so confused?`
	`blue-t-shirt:I created 4 directories,
                   where is the missing dir3,dir4?`

Good question.They are created inside dir2 they won't be listed with 
simple command like `ls`.you need to use "complex" command to view them. Try this:

	ls -R 

really "complex" isn't it  :P ,btw -R stands for recursive.

Okay,we have created a new directories and listed them.Now lets 
move into a new directory.

	cd dir2





title: cd

cool,you have changed to dir2 Now confirm this
location by using previously learned `wm_pwd`(aka pwd)
command.To move into next directory dir3

	cd dir3
will place you under "dir3" directory.

>`Tips and tricks:` Typing 

        cd ..

will move to parent directory.i.e dir2.
Now type,

	cd -
will move you to previous working directory 
i.e dir3 Cool ,isn't it? and a simple

	cd 
will move to the your home directory.

That's it.You have successfully completed lesson1
Now to start next lesson.


