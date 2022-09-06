1. Escribe un comando para ver las últimas dos líneas del archivo `lorem-ipsum.txt`, ubicado en el directorio `bash/`:
```
tail -n2 bash/lorem-ipsum.txt
```

2. Escribe un comando para mostrar la cantidad de palabras que contiene cada línea del archivo `lorem-ipsum.txt`, ubicado en el directorio `bash/`:
```
wc -w bash/lorem-ipsum.tx
```

1. Escribe un comando para ver el contenido del archivo `lorem-ipsum.txt`, ubicado en el directorio `bash`, sin los caracteres ***punto*** `.` y ***coma*** `,`:
```
awk '{gsub(/\.|,/, ""); print}' bash/lorem-ipsum.txt
```

4. Escribe un comando para listar todos los directorios dentro de este repositorio (no recursivo):
```shell
ls -ld */
```

5. Esribe un comando para ordenar los directorios listados, por tamaño:
```shell
ls -S -ld */
```
