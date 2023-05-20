# צעדים ראשונים

כעת נראה איך להריץ תוכנית "Hello World" מסורתית בפייתון. כך נלמד איך לכתוב, לשמור ולהריץ תוכניות פייתון.

ישנן שתי דרכים להשתמש בפייתון בשביל להריץ את הקוד שלך - שימוש במפרש (interpreter) אינטראקטיבי או שימוש בקבצי קוד מקור. כעת נראה כיצד להשתמש בשתי הדרכים. 

## שימוש במפרש האינטראקטיבי
פתח.י את הטרמינל (כפי שנלמד בפרק [ההתקנה](./installation.md#installation)) ופתח.י את האינטרפרטר בכתיבת הפקודה `python3` ולחיצה על הכפתור `[enter]`.

כאשר פייתון נפתח, את.ה אמור לראות `>>>` ליד הסמן שניתן לכתוב. זה יסמן לנו שאנחנו נמצאים בתוך _האינטרפרטר האינטראקטיבי של פייתון_

בתוך האינטרפרטר, כתב.י:

```python
print("Hello World")
```
ולאחר מכן לחצ.י על הכפתור `[enter]`. המילים "Hello World" אמורות להופיע על המסך.

הנה דוגמה של מה שאת.ה אמור.ה לראות, כאשר משתמשים במחשב מק. הפרטים של גרסת הפייתון ישתנו ממחשב למחשב, אבל החל מפתיחת התוכנה (כלומר, החל מהפעם הראשונה שמופיע `>>>`) מה שרואים צריך להיות זהה בכל מחשב וכל מערכת הפעלה.

<!-- The output should match pythonVersion variable in book.json -->
```python
$ python3
Python 3.6.0 (default, Jan 12 2017, 11:26:36)
[GCC 4.2.1 Compatible Apple LLVM 8.0.0 (clang-800.0.38)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> print("Hello World")
Hello World
```
שימ.י לב שפייתון מחזיר תשובה מיידית לשורה שכתבת! מה שהכנסת היא _ביטוי_ (statement) בודד. אנחנו משתמשים ב`print` (באופן לא מפתיע) על מנת להדפיס כל ערך שנספק לו. במקרה שלנו, סיפקנו את הטקסט `Hello World` והוא אכן מודפס למסך.

### איך לצאת מאינטרפרטר

אם את.ה משתמש במערכות ההפעלה לינוקס או מק, את.ה יכול לצאת מהאינטרפרטר באמצעות לחיצה על `[ctrl+d]` או כתיבת הפקודה `exit()` (שימ.י לב: חשוב לרשום את הסוגריים, `()`) ולאחר מכן לחיצה על הכפתור `[enter]`.

אם את.ה משתמש במערכת ההפעלה ווינדוס, עדיין ניתן לכתוב את הפקודה `exit()` או לחלופין ללחוץ על `[ctrl+z]` ולאחר מכן על הכפתור `[enter]`. 


## בחירת עורך טקסט

זה יהיה מסורבל מאוד לכתוב את התוכנה שלנו מחדש בכל פעם שאנחנו רוצים לכתוב משהו, ולכן נרצה לשמור אותה בקבצים ולהריץ מתי שנרצה. לקבצים האלו נקרא _קבצי קוד מקור_ (source code files)

כדי ליצור קבצי קוד מקור בפייתון, אנחנו צריכים תוכנת עריכה שאיתה נכתוב ונשמור את הקוד. תוכנה טובה תעשה לנו חיים קלים בכתיבת קבצי קוד המקור שלנו. אחת הדרישות הבסיסיות שלנו מתוכנת העריכה תהיה _צביעת תחביר השפה_ כך שכל החלקים השונים בתוכנית הפייתון שלך יהיו מסומנים בצבעים שונים כך שניתן _לראות_ את התוכנית בקלות. 

אם את.ה לא בטוח.ה באיזו תוכנה להשתמש, אפשרות מומלצת היא [פייצ'ארם](https://www.jetbrains.com/pycharm-edu/) שזמינה בווינדוס, מק ולינוקס. 

אם את.ה משתמש.ת בווינדוס, *אל תשתמש.י בnotepad* - זאת בחירה רעה בגלל שnotepad לא מדגישה את הסינטקס (תחביר) של פייתון ולא מאפשרת בקלות הזחה של הטקסט (הזזה שלו הצידה), שזו דרישה הכרחית כאשר נכתוב בפייתון. תוכנות עריכה טובות יעשו את שני הדברים האלו אוטומטית. 


## פייצ'ארם {#pycharm}

[פייצ'ארם](https://www.jetbrains.com/pycharm-edu/) היא תוכנת עריכת טקסט חינמית שנועדה לכתיבת קוד פייתון.

כאשר את.ה פותח.ת פייצ'ארם, לחצ.י על `Create New Project`:


![When you open PyCharm](./img/pycharm_open.png)

בחר.י `Pure Python`:

![PyCharm New Project](./img/pycharm_create_new_project.png)

החליפ.י את השם `untitled` לשם לבחירתך, למשל `hello_world`:

![PyCharm project details](./img/pycharm_create_new_project_pure_python.png)

לחצ.י על הכפתור `Create`.

Right-click on the `helloworld` in the sidebar and select `New` -> `Python File`:

![PyCharm -> New -> Python File](./img/pycharm_new_python_file.png)

You will be asked to type the name, type `hello`:

![PyCharm New File dialog box](./img/pycharm_new_file_input.png)

You can now see a file opened for you:

![PyCharm hello.py file](./img/pycharm_hello_open.png)

Delete the lines that are already present, and now type the following:

<!-- TODO: Update screenshots for Python 3 -->

```python
print("hello world")
```
Now right-click on what you typed (without selecting the text), and click on `Run 'hello'`.

![PyCharm Run 'hello'](./img/pycharm_run.png)

You should now see the output (what it prints) of your program:

![PyCharm output](./img/pycharm_output.png)

Phew! That was quite a few steps to get started, but henceforth, every time we ask you to create a new file, remember to just right-click on `helloworld` on the left -> `New` -> `Python File` and continue the same steps to type and run as shown above.

You can find more information about PyCharm in the [PyCharm Quickstart](https://www.jetbrains.com/pycharm-educational/quickstart/) page.

## Vim

1. Install [Vim](http://www.vim.org)
    * Mac OS X users should install `macvim` package via [HomeBrew](http://brew.sh/)
    * Windows users should download the "self-installing executable" from [Vim website](http://www.vim.org/download.php)
    * GNU/Linux users should get Vim from their distribution's software repositories, e.g. Debian and Ubuntu users can install the `vim` package.
2. Install [jedi-vim](https://github.com/davidhalter/jedi-vim) plugin for autocompletion.
3. Install corresponding `jedi` python package : `pip install -U jedi`

## Emacs

1. Install [Emacs 24+](http://www.gnu.org/software/emacs/).
    * Mac OS X users should get Emacs from http://emacsformacosx.com
    * Windows users should get Emacs from http://ftp.gnu.org/gnu/emacs/windows/
    * GNU/Linux users should get Emacs from their distribution's software repositories, e.g. Debian and Ubuntu users can install the `emacs24` package.
2. Install [ELPY](https://github.com/jorgenschaefer/elpy/wiki)

## Using A Source File

Now let's get back to programming. There is a tradition that whenever you learn a new programming language, the first program that you write and run is the 'Hello World' program - all it does is just say 'Hello World' when you run it. As Simon Cozens[^1] says, it is the "traditional incantation to the programming gods to help you learn the language better."

Start your choice of editor, enter the following program and save it as `hello.py`.

If you are using PyCharm, we have already [discussed how to run from a source file](#pycharm).

For other editors, open a new file `hello.py` and type this:

```python
print("hello world")
```

Where should you save the file? To any folder for which you know the location of the folder. If you
don't understand what that means, create a new folder and use that location to save and run all
your Python programs:

- `/tmp/py` on Mac OS X
- `/tmp/py` on GNU/Linux
- `C:\py` on Windows

To create the above folder (for the operating system you are using), use the `mkdir` command in the terminal, for example, `mkdir /tmp/py`.

IMPORTANT: Always ensure that you give it the file extension of `.py`, for example, `foo.py`.

To run your Python program:

1. Open a terminal window (see the previous [Installation](./installation.md#installation) chapter on how to do that)
2. **C**hange **d**irectory to where you saved the file, for example, `cd /tmp/py`
3. Run the program by entering the command `python hello.py`. The output is as shown below.

```
$ python hello.py
hello world
```

![Screenshot of running program in terminal](./img/terminal_screenshot.png)

If you got the output as shown above, congratulations! - you have successfully run your first Python program. You have successfully crossed the hardest part of learning programming, which is, getting started with your first program!

In case you got an error, please type the above program _exactly_ as shown above and run the program again. Note that Python is case-sensitive i.e. `print` is not the same as `Print` - note the lowercase `p` in the former and the uppercase `P` in the latter. Also, ensure there are no spaces or tabs before the first character in each line - we will see [why this is important](./basics.md#indentation) later.

**How It Works**

A Python program is composed of _statements_. In our first program, we have only one statement. In this statement, we call the `print` _statement_ to which we supply the text "hello world".

## Getting Help

If you need quick information about any function or statement in Python, then you can use the built-in `help` functionality. This is very useful especially when using the interpreter prompt. For example, run `help('len')` - this displays the help for the `len` function which is used to count number of items.

TIP: Press `q` to exit the help.

Similarly, you can obtain information about almost anything in Python. Use `help()` to learn more about using `help` itself!

In case you need to get help for operators like `return`, then you need to put those inside quotes such as `help('return')` so that Python doesn't get confused on what we're trying to do.

## Summary

You should now be able to write, save and run Python programs at ease.

Now that you are a Python user, let's learn some more Python concepts.

---

[^1]: the author of the amazing 'Beginning Perl' book
