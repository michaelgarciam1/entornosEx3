# Memoria Práctica 3

## Vemos los commits hechos hasta el momento
![image](https://user-images.githubusercontent.com/114613053/204564698-3ea3dd68-33b0-4399-adb1-c8b6fb411f12.png)  

## Queremos etiquetar el primer y tercer commit  
Para ello debemos usar el comando  
~~~
git  tag  -a  nombre_etiqueta  -m  "Mensaje"   commit_a_etiquetar
~~~  


Los comandos que uso en mi caso son para poner v1 al primer commit y v2 al ultimo:  
~~~
git tag -a v1 -m "Version 1" 114b
git tag -a v2 -m "Version 2" dd7f
~~~  

Tal que queda así:  
![image](https://user-images.githubusercontent.com/114613053/204565729-eab5907a-c654-4ee8-94cb-5a69f3b8eff4.png)  

## Moviendo el head a v1 y v2
Usamos el comando git checkout para v1 y v2.  
Ahora para v1  
~~~
git checkout v1
~~~
![image](https://user-images.githubusercontent.com/114613053/204566522-273d6766-6c2b-4b0f-9441-5e923dbc3c6a.png)  

Ahora para v2  
~~~
git checkout v1
~~~
![image](https://user-images.githubusercontent.com/114613053/204566794-2805a6d3-adc2-4702-b4a1-0384e2e3e04d.png)


## Ver los cambios del commit anterior
Para ello se usa el comando siguiente:
~~~
git show
~~~  
![image](https://user-images.githubusercontent.com/114613053/204567641-a0160d75-6016-4669-b9e4-58fddf24feb5.png)  

Ahora queremos ver los cambios del segundo respecto al primero:  
~~~
git show e3e5
~~~
![image](https://user-images.githubusercontent.com/114613053/204567955-4790c9f2-69d4-4d88-8e2b-ec749e6f196e.png)  

Los cambios del primmer commit  
~~~
git show v1
~~~  
![image](https://user-images.githubusercontent.com/114613053/204568173-eac8ebc9-b5b2-4fd1-bcc5-d5de4c77045d.png)


## Ver cambios respecto a varios commit
Usando el siguiente comando:  
~~~
git  diff  commit1..commit2
~~~  
En mi caso uso:  
~~~
git diff v1..v2
~~~  
![image](https://user-images.githubusercontent.com/114613053/204569099-2357a91c-8279-4bc6-acc3-dea7eac33731.png)


## Diferencias entre el show y el diff
Vemos que hace el git show:
~~~
git show v1..v2
~~~
![image](https://user-images.githubusercontent.com/114613053/204569398-268cef2a-bde8-4ec3-b48e-0798d144d550.png)  

Se puede ver que la gran diferencia es que con el git show se muestran todos los cambios de todos los commit que hay entre medias






