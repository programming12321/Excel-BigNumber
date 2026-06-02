# Excel-BigNumber

## Descripción

Excel-BigNumber es una biblioteca de números gigantes creada completamente con:

```
Excel 365
LAMBDA
Administrador de nombres
Fórmulas nativas de Excel
```

Permite realizar cálculos mucho más allá de los límites numéricos normales de Excel utilizando un formato BigNumber personalizado.

Formato:

```
mantisaeexponente
```

Ejemplos:

```
1e100
2.5e1000
7e500000
1e1.234567e38
```

---

## Formato BigNumber

Cada BigNumber se almacena como:

```
mantisaeexponente
```

Ejemplos:

```
5e3
1.23e6
9e100
-5e100
```

Significado:

```
5e3      = 5 × 10³
1.23e6   = 1.23 × 10⁶
9e100    = 9 × 10¹⁰⁰
```

---

## Funciones Aritméticas

### BigAdd

Suma dos BigNumbers.

```
=BigAdd("1e100";"2e100")
```

Resultado:

```
3e100
```

---

### BigSub

Resta dos BigNumbers.

```
=BigSub("5e100";"2e100")
```

Resultado:

```
3e100
```

---

### BigMul

Multiplica dos BigNumbers.

```
=BigMul("2e10";"3e5")
```

Resultado:

```
6e15
```

---

### BigDiv

Divide dos BigNumbers.

```
=BigDiv("6e15";"3e5")
```

Resultado:

```
2e10
```

---

### BigPower

Potenciación básica.

```
=BigPower("2e10";"3e1")
```

Resultado:

```
8e30
```

---

### BigAbs

Devuelve el valor absoluto.

```
=BigAbs("-5e100")
```

Resultado:

```
5e100
```

---

### BigNeg

Cambia el signo de un BigNumber.

```
=BigNeg("5e100")
```

Resultado:

```
-5e100
```

---

## Funciones de Comparación

### BigGT

Mayor que.

```
=BigGT("5e100";"2e100")
```

Resultado:

```
1
```

---

### BigGTE

Mayor o igual que.

```
=BigGTE("5e100";"5e100")
```

Resultado:

```
1
```

---

### BigLT

Menor que.

```
=BigLT("2e100";"5e100")
```

Resultado:

```
1
```

---

### BigLTE

Menor o igual que.

```
=BigLTE("5e100";"5e100")
```

Resultado:

```
1
```

---

### BigEQ

Igual a.

```
=BigEQ("5e100";"5e100")
```

Resultado:

```
1
```

---

### BigNEQ

Distinto de.

```
=BigNEQ("5e100";"4e100")
```

Resultado:

```
1
```

---

## Funciones Lógicas

### BigIF

```
=BigIF(
BigGT("5e100";"2e100");
"SI";
"NO"
)
```

Resultado:

```
SI
```

---

## Funciones Utilitarias

### BigLOG10

Devuelve el logaritmo en base 10.

```
=BigLOG10("2e3010")
```

Resultado:

```
3010.30103
```

---

### BigFormatExp

Formatea exponentes gigantes.

Entrada:

```
123456789012345678901234567890123456789
```

Salida:

```
1.234567e38
```

---

## Ejemplos

```
=BigAdd("1e100";"2e100")

=BigMul("2e10";"3e5")

=BigDiv("6e15";"3e5")

=BigPower("2e10";"3e1")

=BigGT("1e100";"9e99")

=BigEQ("5e100";"5e100")

=BigAbs("-7e200")

=BigNeg("7e200")

=BigLOG10("2e3010")
```

---

## Requisitos

```
Microsoft Excel 365
```

Características requeridas:

```
LAMBDA
Administrador de nombres
Fórmulas de matrices dinámicas
```

---

## Instalación

1. Abra archivo ```BigNumber.xlsx```

2. Vaya a:

   ```
   Fórmulas → Administrador de nombres
   ```

3. Cree todas las funciones BigNumber.

4. Guarde el libro.

5. Comience a utilizar las fórmulas BigNumber.

---

## Licencia

Licencia MIT

Copyright (c) 2026

Se concede permiso, de forma gratuita, a cualquier persona que obtenga una copia de este software y de los archivos de documentación asociados para utilizar el Software sin restricciones.

---

## Autor

programming12321

Proyecto:

```
Excel-BigNumber
```
