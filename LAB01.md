# Лабораторная работа №1
Изучение утилит для разработки проектов
## Практическая часть

- Скачайте библиотеку _boost_ с помощью утилиты **wget**. Адрес для скачивания `https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz`.
     
     Утилита wget - используется для скачаивания файла, который лежит по ссылке
 
     ![ew](https://github.com/sippyuy/timp/blob/ee9dfd72656865ffe2649d766a50a068351b342b/screens/lab1screens/screen/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2023-04-25_23-28-25.png)
- Разархивируйте скаченный файл в директорию ~/boost_1_69_0
      
     Утилита tar - используется для работы с архивными файлами(распаковка/архивация в частности), флаг -xf означает распаковку и вывод в файл, флаг -С c парматром ~ означает распаковку в домашнюю директорию

     ![](https://github.com/sippyuy/timp/blob/93372d9264fb901fbdf9b2d643cc8d806674bbad/screens/lab1screens/screen/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2023-04-25_22-57-17.png)
- Подсчитайте количество файлов в директории ~/boost_1_69_0 не включая вложенные директории.

     Утилита find - выводит найденные в директории файлы как последовательность строк — полных путей к ним, флаг -maxdepth 1 означет глубину поиска(без вложенных директорий), флаг -type f означает поиск файлов. Результат действия утилиты find передаём утилите wc, которая выводит кол-во строк, слов и байт. Утилита cd - используем для перемещения в нужную директорию.

     ![](https://github.com/sippyuy/timp/blob/b7846e9dd1345b414c3e7c10ceb4da66220e6da2/screens/lab1screens/screen/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2023-04-25_22-59-40.png)
- Подсчитайте количество файлов в директории ~/boost_1_69_0 включая вложенные директории.
     
     То же самое, что и в предыдущем пункте, но без флага -maxdepth, то есть ищем во всех директориях.

     ![](https://github.com/sippyuy/timp/blob/5f18d6698906f0725a0792e1e4163bf2b5026bf9/screens/lab1screens/screen/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2023-04-25_23-00-35.png)
- Подсчитайте количество заголовочных файлов, файлов с расширением .cpp, сколько остальных файлов (не заголовочных и не .cpp).
     
     Флаг -name с паттерном, ищем строку с указанным условием, ! означает отрицание.

     ![](https://github.com/sippyuy/timp/blob/af8c77aec2eadda7f00b79ac89450edb2da7f840/screens/lab1screens/screen/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2023-04-25_23-01-54.png) ![](https://github.com/sippyuy/timp/blob/af8c77aec2eadda7f00b79ac89450edb2da7f840/screens/lab1screens/screen/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2023-04-25_23-02-02.png)
- Найдите полный пусть до файла any.hpp внутри библиотеки boost.
     
     find с флагом -name выводит полные пути до файла.

     ![](https://github.com/sippyuy/timp/blob/c77c0c901e4f88b99d399cdcdd6115f019a86479/screens/lab1screens/screen/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2023-04-25_23-02-33.png)
- Выведите в консоль все файлы, где упоминается последовательность boost::asio.
     
     Утилита grep - проходит по всем строкам каждого файла и выводит все строки, содержащие данный фрагмент, флаг -l выводим вместо строки имя файла, флаг -r проходим по всем файлам, включая вложенные директории.

     ![](https://github.com/sippyuy/timp/blob/352ccb580c7db004d4f0ae2da1f235321ac13c47/screens/lab1screens/screen/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2023-04-25_23-03-48.png)
- Скомпилирутйе boost. Можно воспользоваться инструкцией или ссылкой.
     
     Используем команды ./bootstrap.sh и ./b2 install согласно инструкции, ждём окончания.

     ![](https://github.com/sippyuy/timp/blob/9b4340d2d926dd1f69488767e16842afa33cc6cd/screens/lab1screens/screen/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2023-04-25_23-04-25.png)
     
     
     ![](https://github.com/sippyuy/timp/blob/9b4340d2d926dd1f69488767e16842afa33cc6cd/screens/lab1screens/screen/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2023-04-25_23-08-44.png)
     
     
     ![](https://github.com/sippyuy/timp/blob/9b4340d2d926dd1f69488767e16842afa33cc6cd/screens/lab1screens/screen/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2023-04-25_23-07-48.png)
- Перенесите все скомпилированные на предыдущем шаге статические библиотеки в директорию ~/boost-libs.
     
     Mkdir - создать директорию. Утилита cp копирует файлы в указанную директорию, причём мы подаём ей на вход результат действия утилиты find.

     ![](https://github.com/sippyuy/timp/blob/40f2888811bfc90ea7c77ed097de7986c4d4cab9/screens/lab1screens/screen/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2023-04-25_23-09-38.png)
- Подсчитайте сколько занимает дискового пространства каждый файл в этой директории.
     
     Флаг -exec {} + для каждого найденного файла выполняется команда. du - выводит вес каждого файла. Флаг -h преобразует вес в удобочитаемый формат.

     ![](https://github.com/sippyuy/timp/blob/b4057b761c81ebabd4ab9a91b90e3250f2b4e0b4/screens/lab1screens/screen/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2023-04-25_23-10-46.png)
- Найдите топ10 самых "тяжёлых".
     
     Утилита sort - сортирует строки флаг -r означает сортировку по убыванию, флаг -n сортировка по числам, утилита head позволяет оставить первые строки, указанные в параметре флага -n

     ![](https://github.com/sippyuy/timp/blob/0cd6f75c9791baaee03b3c2241c6f274ac54d07a/screens/lab1screens/screen/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2023-04-25_23-11-20.png)
