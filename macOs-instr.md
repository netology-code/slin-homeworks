## Установка VirtualBox на операционные системы, отличные от Windows

Вы можете установить VirtualBox на такие операционные системы как macOS, дистрибутивы Linux и некоторые другие. Установочные файлы и инструкции можно найти на [официальном сайте VirtualBox](https://www.virtualbox.org/wiki/Downloads) компании Oracle.

### Установка на macOS

- **Процессоры Intel**

Если ваш компьютер на базе процессора Intel, воспользуйтесь соответствующей ссылкой для «macOS/Intel hosts» с [официального сайта VirtualBox](https://www.virtualbox.org/wiki/Downloads).

- **Apple ARM-процессоры M1/M2**

На момент написания этой инструкции VirtualBox для процессоров Apple M1/M2 находится в Developer Preview (предварительная версия для разработчиков). По отзывам многих данная версия по факту не работает. Это может измениться с выходом более новых версий.

Если на момент установки VirtualBox не работает на вашем компьютере, вы можете воспользоваться альтернативами такими как:
•	[UTM](https://mac.getutm.app/)(бесплатная)
•	[Parallels](https://www.parallels.com/products/desktop/) (платная)
•	[VMware Fusion 13](https://www.vmware.com/products/fusion/fusion-evaluation.html) (есть бесплатная версия, требует регистрации)

Пример установки UTM используя пакетный менеджер Homebrew:

`brew install --cask utm`

Примечание:
Для наилучшей (приемлемой) производительности необходимо использовать ARM образы для ваших виртуальных машин.

### Установка на Linux

Для установки VirtualBox на ваш дистрибутив Linux воспользуйтесь [инструкцией с официального сайта Virtual Box](https://www.virtualbox.org/wiki/Linux_Downloads).
