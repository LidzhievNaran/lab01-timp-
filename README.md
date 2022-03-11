# lab01-timp-
Скачиваем библиотеку boost - wget: https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz.
Разархивируем  файл: tar -xf boost_1_69_0.tar.gz
меняем местоположение cd boost_1_69_0
качаем  tree 
Подсчитываем количество файлов в директории, не включая вложенные директории: tree -L1 -12

Подсчитываем количество файлов в директории, включая вложенные директории: tree 61191
Подсчитайте количество заголовочных файлов: tree -P *.hpp - 14912
Подсчитайте количество  файлов с расширением `.cpp':tree -P *.cpp - 13774
остальные файлы - 32433
Найдите полный пусть до файла any.hpp внутри библиотеки boost: realpath.any.hpp
Выведите в консоль все файлы, где упоминается последовательность boost::asio: grep -rl 'boost::asio'
Скомпилируйте Boost: ./bootstrap.sh
./b2
Перемещение библиотеки в директорию
mv ./boost/ ~/boost-libs && cd ~/boost-libs/
Подсчитайте сколько занимает дискового пространства каждый файл в этой директории.
ls -sh
Найдите топ10 самых "тяжёлых"
du -sh | sort -rh | head -10
https://drive.google.com/drive/u/0/folders/1kkveq0KCeUmXCZPIQV6Ckz1oqbgGQ7Fw
