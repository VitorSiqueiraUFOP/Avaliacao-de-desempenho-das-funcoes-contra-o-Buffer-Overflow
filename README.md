# Avaliação de desempenho das funções contra o Buffer Overflow

One Paragraph of project description goes here

## Equipamento utilizado

What things you need to install the software and how to install them

## Compilação

O código avaliado foi compilado pelo compilador GCC versão: 6.3.0 nas definições de fábrica usando o comando:

```
gcc main.c 'pkg-config --cflags --libs glib-2.0' -o main -lm
```

Onde ```pkg-config --cflags --libs glib-2.0``` representa a biblioteca glib.h e ```-lm``` significa a biblioteca math.h. 

## Execução

O software foi executado no modo administrador, e antes de cada iteração o buffer e o cache foram limpos através do comando: 

```
free \&\& sync \&\& echo 3 > /proc/sys/vm/drop\_caches \&\& free
```

## Testes executados
