Перші кроки:
git version - яка версія стоїть?

Одноразово сконфігурувати Git:
git config --global user.name "Rec0440"
git config --global user.email "bogdankyr@gmail.com"

Створення репозиторію:
cd ...
cd c:/         - change directory
cd c:/gitload/ - перехід у потрібну директорію
mkdir name - створення директорії name (для подальшої роботи перейти у неї)
git init - створення пустого репозиторію в активній папці
Взагалі, git init можна виконати в будь-якій директорії, після чого вона міститиме локальний git-репозитарій

створити файл (програма, текст, інше)

git workflow:
1. git clone https://github.com/Rec0440/HelloWorld.git - копіюємо собі на ПК проект з Git
2. git status - виводимо поточний статус проекту/файлів
3. git add filename - додаємо файл під версійний контроль або індексуємо зміни у вже відслідкованому файлі
4. git commit -m "insert what you doing"
5. git push - заливаємо зміни на Git

Як внести зміни:
1. git add -A - завантажити всі редаговані файли
2. git commit -m "insert what you doing" - внести помітку "Що зроблено"
3. git status - перевірити зміни перед завантаженням на Git
4. git push - заливаємо зміни на Git

Як стягнути зміни/зроблену іншими роботу:
1. git pull - зкачуємо зміни з Git
2. git fetch - стягнути зміни

Ігнорування файлів.
пример файла .gitignore:
# no .a files
*.a
# but do track lib.a, even though you're ignoring .a files above
!lib.a
# only ignore the root TODO file, not subdir/TODO
/TODO
# ignore all files in the build/ directory
build/
# ignore doc/notes.txt, but not doc/server/arch.txt
doc/*.txt
# ignore all .txt files in the doc/ directory
doc/**/*.txt

TIP GitHub поддерживает довольно полный список примеров .gitignore файлов для
множества проектов и языков https://github.com/github/gitignore это может стать
отправной точкой для .gitignore в вашем проекте.



Перелік команд і їх атрибутів:

git status - 
	git status -s      - вивід в спрощеному вигляді
	git status --short - вивід в спрощеному вигляді
		вивід:  ?? - нові, невідсліддковувані файли,
			A - файли, що додані у відслідковувані
			M - відредаговані файли

