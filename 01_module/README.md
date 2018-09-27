# Модули ядра

## Тесты

```bash
1) Компиляция: make
2) Очистка: make clean
3) file md1.ko (просмотр инфы о модуле)
4) insmod md2.ko (тест порядка загрузки)
   insmod: error inserting 'md2.ko': -1 Unknown symbol in module
5) insmod md1.ko
6) insmod md2.ko
7) dmesg | tail -n30 | grep md
8) rmmod md1
   rmmod: ERROR: Module md1 is in use by: md2
9) lsmod | grep md
10) insmod md3.ko (завершается при запуске)
11) lsmod | grep md; dmesg | tail -n30 | grep md
12) rmmod md2
13) rmmod md1
14) lsmod | grep md
15) dmesg | grep +
```
