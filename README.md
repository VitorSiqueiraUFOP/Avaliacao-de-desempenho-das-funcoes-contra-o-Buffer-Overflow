# Avaliação de desempenho das funções contra o Buffer Overflow

O presente software é um trabalho acadêmico que tem objetivo de comparar o desempenho das soluções seguras do Buffer Overflow com as não-seguras para medir uma eventual sobrecarga. As funções selecionadas manipulam as string que apesar de ser uma amostra pequena,  tem fins didáticos, visto que há outras funções para testar. 

## Funções inseguras

``` ```
``` ```
``` ```

## Funções seguras nativa da linguagem C

``` ```
``` ```
``` ```

## Funções seguras da biblioteca glib.h

```gsize g_strlcpy (gchar *dest, const gchar *src, gsize dest_size);```
```gsize g_strlcat (gchar *dest, const gchar *src, gsize dest_size);```
```gint g_snprintf (gchar *string, gulong n, gchar const *format, ...);```

## Equipamento utilizado

O equipamento utilizado para representar os dispositivos de IoT foi Raspberry Pi, um computador desenvolvido pela Raspberry Pi Foundation, que é uma organização de caridade britânica. O propósito do é estimular a educação da Ciência Computação através da acessibilidade de aquisição, com valor estabelecido de $35,00, que apesar de apresentar uma configuração modesta, é uma ferramenta capaz de executar diversas tarefas apta para fins acadêmico. O modelo específico é o Raspberry 3 modelo B+, disponibilizado em 2018.

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

## Resultados

Foi executado 4 iterações do programa, os resultados obitidos estão no formato de prints extraídos do Raspberry Pi disponível no diretório "Prints-Resultado-Raspberry-Pi".
