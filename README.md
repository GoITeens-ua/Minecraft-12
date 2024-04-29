# Механізми. Події

#### Опис

{% hint style="success" %}
Сьогодні ми продовжимо працювати в лабіринті й навчимося створювати систему фейєрверків і притискних панелей, а також битимемося з Мінотавром!👾
{% endhint %}

## Згадаймо🤔

1. Що таке нить Аріадни?&#x20;
2. Де з'явився перший фейєрверк?
3. Як створити фейєрверк?

## Сьогодні ми:

1. Побудуємо систему запуску фейєрверків
2. Створимо систему з притискних панелей, пилу редстоуну, липкого поршню та блок смарагду
3. Навчимося виводити на екран різні символи та текст при натисканні натискної панелі (з висування)

### Події

На початку заняття відпрацюємо створення елементів, які можуть сигналізувати про прохід агенту чи гравця в певній точці.

### Фейєрверки

Побудуйте систему запуску фейєрверків з **дубовими притискними пластинами**, **пилом редстоуну** та **розподілювачами**.

<table><thead><tr><th width="242"></th><th></th></tr></thead><tbody><tr><td>Код:</td><td><img src=".gitbook/assets/88.png" alt=""></td></tr><tr><td>Результат:</td><td><img src=".gitbook/assets/89.png" alt=""></td></tr></tbody></table>

До розподілювачів завантажимо фейєрверки.

![](<.gitbook/assets/image (26).png>)![](<.gitbook/assets/image (21).png>)

Сформуємо код, який запрограмує Агента так, щоб він почав бігати і натискати пластини.

<table><thead><tr><th width="196"></th><th></th></tr></thead><tbody><tr><td>Код:</td><td><img src=".gitbook/assets/90.png" alt=""></td></tr><tr><td>Результат:</td><td><img src=".gitbook/assets/Screen Recording (02.02.2023 16-26-37).gif" alt=""></td></tr></tbody></table>

{% hint style="warning" %}
При виконанні коду - треба дочекатися, щоб Агент всі кроки “вибігав” - тоді він знову опиниться в потрібній точці.
{% endhint %}

#### [Липкий поршень](https://makecode.com/\_gtCLmE2Lx9f3)

Створіть систему з притискних панелей, пилу редстоуну, липкого поршню та блок смарагду.

<table><thead><tr><th width="233"></th><th></th></tr></thead><tbody><tr><td>Код:</td><td><img src=".gitbook/assets/91.png" alt=""><br><img src=".gitbook/assets/92.png" alt=""></td></tr><tr><td>Результат:</td><td><img src="https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/piston01.png" alt="" data-size="original"></td></tr></tbody></table>

Перевірте роботу створеної системи.

<div align="left">

<img src="https://github.com/mikh-maksi/minecraft_cards2/raw/main/lesson04/img/piston02.gif" alt="">

</div>

Визначте координати поруч із блоком смарагду **(0;-60;-12)**.&#x20;

<figure><img src=".gitbook/assets/93.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**Зверніть увагу!** У вас координати (**0;-60;-12**) будуть іншими, їх значення необхідно брати із вказівника координат в точці, куде липкий поршень пересуває блок смарагду **у вашому світі.**
{% endhint %}

Сформуйте код, який контролює наявність блоку смарагду у визначених координатах (**0;-60;-12**).\


<figure><img src=".gitbook/assets/94.png" alt=""><figcaption></figcaption></figure>

Перевірте роботу відповідного елементу.

<figure><img src=".gitbook/assets/Screen Recording (07.02.2023 13-55-37).gif" alt=""><figcaption></figcaption></figure>

### Події

<table><thead><tr><th> </th><th width="383.66666666666663"> </th></tr></thead><tbody><tr><td><strong>Завдання</strong></td><td><p></p><ol><li>Виведіть на екран символи «<strong>:-)</strong>» при натисканні натискної панелі (із висування).</li><li>Виведіть на екран символи «<strong>!</strong>» при натисканні натискної панелі.</li><li>Виведіть поточний ігровий час при натисканні натискної панелі.</li></ol></td></tr><tr><td><strong>Код</strong></td><td><p><img src=".gitbook/assets/93.png" alt="" data-size="original"></p><p><img src=".gitbook/assets/94.png" alt="" data-size="original"></p></td></tr><tr><td><strong>Результат</strong></td><td><p></p><p><img src=".gitbook/assets/Screen Recording (07.02.2023 13-55-37).gif" alt="" data-size="original"></p></td></tr></tbody></table>

### Одна дія

Ви можете побачити в попередньому завданні, що виведення на екран тексту повторюється декілька разів. Для того, щоб дія повторювалася лише один раз, необхідно використовувати змінну, якій значення задаємо при команді «start». Встановимо код, який задає змінній flag **значення 0** та виведемо на екран повідомлення «**(+) Flag activated.**»

![](.gitbook/assets/97.png)

Додамо умову спрацьовування (знаходження блоку смарагду в точці (-30;4;-99)) та за умови, що змінна flag має значення 0

<figure><img src=".gitbook/assets/95.png" alt=""><figcaption></figcaption></figure>

Змінимо значення змінної **flag на 1**. В результі дія, що зазначена в цій умові (в нашому випадку це вивід на екран символів «**:-)**») відбудеться лише 1 раз.

<figure><img src=".gitbook/assets/96.png" alt=""><figcaption></figcaption></figure>

Змінимо текст повідомлення на «**(-) Flag deactivated.**»

<figure><img src=".gitbook/assets/1123456789.gif" alt=""><figcaption></figcaption></figure>

Для створеної системи з притискної панелі, пилу редстоуну, липкого поршню та блоку смарагду запрограмуйте наступні дії (_**зверніть увагу**, що в вашому випадку координати можуть відрізнятися, і вам необхідно визначати координати місця, у яке переміщується блок смарагду самостійно_):

<table data-header-hidden><thead><tr><th> </th><th width="413.66666666666663"> </th></tr></thead><tbody><tr><td><strong>Завдання</strong></td><td><ol><li>Запрограмуйте так, щоб при команді <strong>start</strong> на екран було виведено текст <strong>(+)Flag activated</strong>, а при натисканні панелі — один раз було виведено <strong>(-)Flag deactivated</strong></li><li>Запрограмуйте так, щоб при команді <strong>start</strong> на екран було виведено текст <strong>Action started!</strong>, а при натисканні панелі — один раз було виведено <strong>Action stoped!</strong></li></ol></td></tr><tr><td><strong>Код</strong></td><td><img src=".gitbook/assets/97.png" alt=""><br><img src=".gitbook/assets/98.png" alt=""></td></tr><tr><td><strong>Результат</strong></td><td><img src=".gitbook/assets/1123456789.gif" alt="" data-size="original"></td></tr></tbody></table>



## Фіксація розбиття блоків

За команди чату **start2** задамо змінній **flag2** значення **1** та виведемо на екран повідомлення «**start**». А також перенесемо гравця в точку **(-40;-60;-90)** та розмістимо блок алмазу в точці **(-45;-60;-90)**\
![](.gitbook/assets/99.png)

Задамо код, який виводить повідомлення «**finish**», якщо блок алмазу знищити. Задамо код, який виводить повідомлення «**finish**», якщо блок алмазу знищити.

<figure><img src=".gitbook/assets/100 (2).png" alt=""><figcaption></figcaption></figure>

Подивимось на на результат

<figure><img src=".gitbook/assets/Screen Recording (07.02.2023 15-45-49).gif" alt=""><figcaption></figcaption></figure>

## Фіксація розбиття 2-х блоків

Створимо два блоку: смарагду та алмазу та задамо змінним **flag3** та **flag4** значення 1, а також виведемо на екран текст «**Initialisation**»

![](.gitbook/assets/101.png)

При знищенні алмазного блоку напишемо на екрані **Start,** при знищенні смарагдового — напишемо на екрані **Finish**

<figure><img src=".gitbook/assets/102.png" alt=""><figcaption></figcaption></figure>

Подивимось на результат

![](<.gitbook/assets/Screen Recording (07.02.2023 15-56-21).gif>)

### Механізм появи монстрів

Знову будуємо той самий механізм і відмічаємо координати

<figure><img src=".gitbook/assets/109.png" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
Щоб швидше зрозуміти координати які вам потрібні - не ставайте на пластину і тоді беріть координати Агента
{% endhint %}

Далі пишемо такий код:

<figure><img src=".gitbook/assets/110.png" alt=""><figcaption></figcaption></figure>

Результат:

<figure><img src=".gitbook/assets/Screen Recording (07.02.2023 17-22-13).gif" alt=""><figcaption></figcaption></figure>



\


![Підсумки заняття](<.gitbook/assets/Group 2393.png>)

