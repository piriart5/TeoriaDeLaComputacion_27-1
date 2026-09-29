# 1er Lista de Problemas y Ejercicios 
**Escuela Superior de Cómputo**\
Teoría de la Computación $|$ 4CV4\
Sánchez Iriarte Juan Pablo $|$ 2025630142

## Problemas de Estructuras Ordenadas

Sea $\Sigma = \left\\{0, 1\right\\}$. En los problemas 1-4, encuentre una
cadena *w* que pertenezca al conjunto *A* con las características
indicadas, cuando sea posible.

1.  $A = \Sigma^*$. Encuentre *w* tal que $|w|$ = 5.\
    ***w* = 01001**

2.  $A = \Sigma^+$. Encuentre *w* tal que $|w|$ = 0.\
    **NO HAY *w*** tal que $|w|$ = 0, ya que la definición de **Clausura
    Positiva** nos dice que
    **$\Sigma^+ = \Sigma^* - \left\{\lambda\right\}$**; por lo tanto,
    *A* no contiene la *cadena vacía ($\lambda$)*.

3.  $A = \Sigma^*$. Encuentre *w* tal que $|w|$ = 0.\
    ***w* = $\lambda$**

4.  $A = \Sigma^5$. Encuentre *w* tal que el primer carácter de *w* sea
    0.\
    ***w* = 00100**

Sea $\Sigma = \{a,b\}$,
$L_1 = \{w \in \Sigma^* : w \text{ comienza con } a\}$ y
$L_2 = \{w \in \Sigma^* : w \text{ termina en } b\}$. Dadas las cadenas
$\omega$ = *abbbaa*, $\pi$ = *aaabb* y $\tau$ = *baaba*, realice lo
siguiente en los ejercicios 5-13:

5.  Determine $|\pi|$.\
    **$\pi = \textit{aaabb}, \quad \therefore \quad |\pi| = 5$**

6.  Determine $\omega\pi$.\
    **$\omega = \textit{abbbaa}, \quad \pi = \textit{aaabb}, \quad \therefore \quad \omega\pi = \textit{abbbaaaaabb}$**

7.  Determine $\pi\omega$.\
    **$\pi = \textit{aaabb}, \quad \omega = \textit{abbbaa}, \quad \therefore \quad \pi\omega = \textit{aaabbabbbaa}$**

8.  Verifique si $(\omega\pi)\tau = \omega(\pi\tau)$\
    Lado izquierdo:
    $\omega\pi = \textit{abbbaaaaabb} \rightarrow (\omega\pi)\tau = \textit{abbbaaaaabbbaaba}$\
    Lado derecho:
    $\pi\tau = \textit{aaabbbaaba} \quad \rightarrow \omega(\pi\tau) = \textit{abbbaaaaabbbaaba}$\
    Por lo tanto, **SI cumple**

9.  Proporcione una palabra en $\Sigma^7$.\
    **$w_9$ = *bababab***

10. Proporcione una palabra en $L_1 \cap \Sigma^5$.\
    **$w_A$ = *ababb***

11. Proporcione una palabra en $L_2 \cap \Sigma^4$.\
    **$w_B$ = *abab***

12. Proporcione una palabra en $L_1 \cap L_2$.\
    **$w_C$ = *ab***

13. Determine $L_1 \cap \Sigma^0$.\
    **NO SE PUEDE**, ya que $\Sigma^0 = \lambda$, la cual es una cadena
    vacía y no contiene a la letra *a*, es decir, $\lambda \notin L_1$.

Sea $\Sigma = \left\\{a, b, c, d\right\\}$ y $\omega$ = *abbca*, $\pi$ =
*abb*, $\tau$ = *ca*. Consideremos los siguientes lenguajes:\
$L_1 = \left\\{\rho\in\Sigma^* : |\rho|\leq5\right\\}$\
$L_2 = \left\\{a^n b^m : n < m\right\\}$\
$L_3 = \left\\{\rho\in\Sigma^* : \rho  \text{ tiene más letras } b \text{ que letras } a\right\\}$\
Indique si las siguientes afirmaciones (14-46) son verdaderas o falsas

14. $|\omega|$ = 3 $\rightarrow$ **FALSO**

15. $|\omega|$ = 5 $\rightarrow$ **VERDADERO**

16. $\omega=\tau\pi$ $\rightarrow$ **FALSO**, ($\omega\neq\text{caabb}$)

17. $\omega=\pi\tau$ $\rightarrow$ **VERDADERO**

18. $\omega(\pi\tau)=(\omega\pi)\tau$ $\rightarrow$ **VERDADERO**,
    demostrado en p.8

19. $\omega(\tau\pi)=(\omega\pi)\tau$ $\rightarrow$ **FALSO**,
    *abbcacaabb* $\neq$ *abbcaabbca*

20. $\lambda\in\Sigma^+$ $\rightarrow$ **FALSO**,
    $\Sigma^+$ no incluye $\lambda$

21. $\lambda\in\Sigma^*$ $\rightarrow$ **VERDADERO**

22. $\omega\in\Sigma^5$ $\rightarrow$ **VERDADERO**

23. $\omega\in\Sigma^3$ $\rightarrow$ **FALSO**

24. $\pi\tau\in\Sigma^5$ $\rightarrow$ **VERDADERO**, $\pi\tau=\textit{abbca}$

25. $\pi\lambda\in\Sigma^3$ $\rightarrow$ **VERDADERO**,
    $|\lambda|=0\quad\therefore\quad|\omega|+0=|\omega|$

26. $a^8\omega\in\Sigma^8$ $\rightarrow$ **FALSO**, $|a^8\omega|=13$

27. $a^3\omega\in\Sigma^8$ $\rightarrow$**VERDADERO**, $|a^3\omega|=8$

28. $a^3c^3\in\Sigma^9$ $\rightarrow$ **FALSO**, $|a^3c^3|=6$

29. $|a^2c^3|=|c^6|$ $\rightarrow$ **FALSO**,
    $|a^2b^3|=5$ y $|c^6|=6$

30. $|a^4b^3c|$=$|a^3b^2c^3|$ $\rightarrow$ **VERDADERO**,
    $|a^4b^3c|=8$ y $|a^3b^2c^3|=8$

31. *ab* $\in L_1$ $\rightarrow$ **VERDADERO**

32. *ab* $\in L_2$ $\rightarrow$ **FALSO**, $n \nless m$

33. *ab* $\in L_3$ $\rightarrow$ **FALSO**, misma
    cantidad de *a* que de *b*

34. *aba$b^2$* $\in L_1$ $\rightarrow$ **VERDADERO**

35. *aba$b^2$* $\in L_2$ $\rightarrow$ **VERDADERO**,
    *n*=2, *m*=3 $\therefore n < m$

36. *aba$b^2$* $\in L_3$ $\rightarrow$ **VERDADERO**

37. *abcad* $\in L_1$ $\rightarrow$ **VERDADERO**

38. *abcad* $\in L_2$ $\rightarrow$ **FALSO**,
    *n*=2, *m*=1 $\therefore n \nless m$

39. *abcad* $\in L_3$ $\rightarrow$ **FALSO**

40. $L_1 \subseteq L_2$ $\rightarrow$ **FALSO**, no tienen relación.

41. $L_1 \subseteq L_3$ $\rightarrow$ **FALSO**, no tienen relación.

42. $L_2 \subseteq L_3$ $\rightarrow$ **VERDADERO**

43. $L_3 \subseteq L_2$ $\rightarrow$ **FALSO**, $L_3$ no exige que
    tenga la forma $a^nb^m$

44. Si $\alpha\in\Sigma^*$, entonces $\alpha\lambda=\lambda\alpha$.
    $\rightarrow$ **VERDADERO**

45. Si $\alpha\in\Sigma^3$ y $\beta\in\Sigma^4$,
    $\therefore|\alpha\beta|=12$.
    $\rightarrow$ **FALSO**, $|\alpha\beta|= |\alpha|+|\beta|=3+4$

46. Si $\alpha\in\Sigma^3$ y $\beta\in\Sigma^4$,
    $\therefore|\alpha\beta|=7$.
    $\rightarrow$ **VERDADERO**

En caso de que sea posible, encuentre cinco palabras de cada uno de los
lenguajes que se definen en los problemas 47-56, usando el alfabeto
$\Sigma = \left\\{0,1,2,3,4,5,6\right\\}$.

47. $L_1=\left\\{01^n : n\in\mathbb{N}\right\\}$\
    **01, 01$^2$, 01$^3$, 01$^4$, 01$^5$**

48. $L_2=\left\\{0^n1^n2^n:n\in\mathbb{N}\right\\}$\
    **012, 0$^2$1$^2$2$^2$, 0$^3$1$^3$2$^3$,
    0$^4$1$^4$2$^4$, 0$^5$1$^5$2$^5$**

49. $L_3=\left\\{\omega\in\Sigma^*:|\omega|=6\right\\}$\
    **012345, 102345, 120345, 123045, 123405**

50. $L_4=\left\\{\omega\in\Sigma^*:\text{ la suma de los dígitos de }\omega\text{ es seis}\right\\}$\
    **06, 51, 42, 33, 222**

51. Determine $L_1 \cap L_2$\
    Una palabra de $L_1$ únicamente tiene un '0' y varios '1'. Mientras
    que una palabra de $L_2$ tiene la misma cantidad de '0', de '1' y
    **además contiene '2'**; $\therefore L_1 \cap L_2 = \varnothing$.

52. Determine $L_1 \cap L_3$\
    Debe tener la forma $01^n$ y longitud de 6, entonces *n = 5*;
    $\quad\therefore L_1 \cap L_3 = \left\\{ 011111   \right\\}$

53. Determine $L_1 \cap L_4$\
    Debe tener la forma $01^n$ y la suma de sus dígitos debe ser 6,
    entonces *n = 6*;
    $\therefore L_1 \cap L_4 = \left\\{ 0111111   \right\\}$

54. Determine $L_2 \cap L_3$\
    Debe tener la forma $0^n1^n2^n$ y longitud de 6, es decir, *3n = 6*,
    entonces *n = 2*;
    $\therefore L_2 \cap L_3 = \left\\{ 001122 \right\\}$

55. Determine $L_2 \cap L_4$\
    La suma de sus dígitos es: *0n + 1n + 2n = 3n* y *3n=6*, entonces *n
    = 2*;\
    $\therefore L_2 \cap L_4 = \left\\{ 001122 \right\\}$

56. Determine $L_3 \cap L_4$\
    Debe tener una longitud de 6 y la suma de dígitos igual a 6;\
    $\therefore \left\\{ 000006, 000051, 000042, 000033, 000222 \right\\} \in L_3 \cap L_4$

## Propiedades de la Clausura de Kleene y Positiva

Sea *A* un lenguaje sobre $\Sigma$, es decir, *A*$\subseteq\Sigma^*$.
Demuestre las siguientes propiedades (57-65) de la clausura de Kleene
($A^*$) y la clausura positiva ($A^+$):

57. $A^+ = A^* \cdotp A = A \cdot A^*$\
    $A^* \cdot A = ( \bigcup\limits_{n \geq 0} A^n \cdot A) = \bigcup\limits_{n \geq 0}(A^n \cdot A) = \bigcup\limits_{n \geq 0} A^{n+1} = \bigcup\limits_{m \geq 1} = A^+$\
    $A \cdot A^* = (A \cdot \bigcup\limits_{n \geq 0} A^n) = \bigcup\limits_{n \geq 0} (A \cdot A^n) = \bigcup\limits_{n \geq 0} A^{1+n} = \bigcup\limits_{m \geq 1} = A^+$\
    $\therefore A^+ = A^* \cdotp A = A \cdot A^*$

58. $A^* \cdot A^* = A^*$\
    Por definición, sabemos que:
    $B^* = \bigcup\limits_{n \geq 0} B^n \\ \text{Entonces: } A^*\cdot A^* = (\bigcup\limits_{i \geq 0} A^i) \cdot (\bigcup\limits_{j \geq 0} A^j) = \bigcup\limits_{i,j \geq 0} (A^i \cdot A^j) = \bigcup\limits_{i,j \geq 0} A^{i+j} = \bigcup\limits_{m \geq 0} A^m = A^* \\\therefore A^* \cdot A^* = A^*$

59. $(A^*)^n = A^*$, $\forall n\geq1$\
    Caso base: $n=1$ $(A^*)^1 = A^*$\
    Hipótesis de inducción: Supóngase que para algún $n \geq 1$ se
    cumple: $(A^*)^n=A^*$.\
    Demostremos: $(A^*)^{n+1} = A^*$;
    $(A^*)^{n+1} = (A^*)^n \cdot A^* = A^* \cdot A^*$, ya demostramos
    que
    $A^* \cdot A^* = A^*, \quad\therefore \text{ por inducción matemática: } (A^*)^n = A^*, \forall n \geq 1.$

60. $(A^*)^* = A^*$\
    Por definición: $B^* = \bigcup\limits_{i\geq0} B^i$, en este caso,
    $B=A^*$.\
    Entonces
    $(A^*)^* = \bigcup\limits_{i \geq 0} (A^*)^i = A^0 \cup \bigcup\limits_{i \geq 1} (A^*)^i = \left\{\lambda\right\} \cup \bigcup\limits_{i \geq 1} (A^*)^i$;\
    vimos que $(B^*)^n = B^*$, $\forall n \geq 1$,
    $\rightarrow \left\{\lambda\right\} \cup \bigcup\limits_{i \geq 1} A^* = \left\{\lambda\right\} \cup A^* = A^* \quad \therefore (A^*)^* = A^*$.

61. $A^+ \cdot A^+ \subseteq A^+$\
    Por definición, sabemos que: $B^+ = \bigcup\limits_{n\geq1} B^n$\
    Entonces:
    $A^+ \cdot A^+ = \bigcup\limits_{i\geq1} A^i \cdot \bigcup\limits_{j\geq1} A^j = \bigcup\limits_{i,j\geq1} A^{i+j} = \bigcup\limits_{k\geq1} A^{k} = A^+ \quad \therefore A^+ \cdot A^+ \subseteq A^*$.

62. $(A^*)^+ = A^*$\
    Por definición de Clausura Positiva:
    $(A^*)^+ = \bigcup\limits_{n \geq 1} (A^*)^n$, además, hemos
    demostrado que: $(A^*)^n = A^*, \forall n \geq 1$,
    $\quad\therefore (A^*)^+ = A^*$.

63. $(A^+)^* = A^*$\
    Por definición de Clausura de Kleene:
    $(A^+)^* = \bigcup\limits_{n \geq 0} (A^+)^n = (A^+)^0 \cup \bigcup\limits_{n \geq 1} (A^+)^n = \left\{\lambda\right\} \cup \bigcup\limits_{n \geq 1} (A^+)^n$,
    además, demostramos que:
    $A^+ \cdot A^+ \subseteq A^+ \quad (\forall n \geq 1)$.\
    Entonces: $(A^+)^* \subseteq \left\{\lambda\right\} \cup A^+ =A^*$
    $\quad\therefore (A^+)^* = A^*$.

64. $(A^+)^+ = A^+$\
    Por definición: $(A^+)^+ = \bigcup\limits_{n\geq1} (A^+)^n$, además,
    vimos que: $A^+ \cdot A^+ \subseteq A^+ \quad (\forall n \geq 1)$.\
    Entonces $(A^+)^n \subseteq A^+ \quad (\forall n \geq 1)$;
    $\quad\therefore (A^+)^+ \subseteq A^+$,\
    para la otra inclusión:
    $(A^+)^1 \subseteq A^+ \rightarrow A^+ \subseteq (A^+)^+ \quad\quad \therefore (A^+)^+ = A^+$.

65. Si *A* y *B* son lenguajes sobre $\Sigma^*$, entonces
    $(A \cup B)^* = (A^*B^*)^*$

    Si $x \in A$, entonces: $x = x \varepsilon$, con $x \in A^*$ y
    $\varepsilon \in B^*. \quad \therefore x \in A^*B^*$

    Del mismo modo, si $x \in B$, entonces: $x = \varepsilon x$, con
    $\varepsilon \in A^*$ y $x \in B^*. \quad \therefore x \in A^*B^*$

    Por lo tanto, $A \cup B \subseteq A^*B^*$, aplicando Clausura de
    Kleene: $(A \cup B)^* \subseteq (A^*B^*)^*$

    Como $A \subseteq A \cup B$, entonces: $A^* \subseteq (A \cup B)^*$.

    Igualmente: $B \subseteq A \cup B$, implica:
    $B^* \subseteq (A \cup B)^*$.

    Por lo tanto, si $x \in A^*$ y $y \in B^*$, como $(A \cup B)^*$ es
    concatenado: $xy \in (A \cup B)^*$, así:
    $A^*B^* \subseteq (A \cup B)^*$.

    Aplicando estrella: $(A^*B^*)^* \subseteq ((A \cup B)^*)^*$ y como
    vimos:
    $(B^*)^* = B^* \\ \therefore (A^*B^*)^* \subseteq (A \cup B)^*$

    Por lo tanto: $(A \cup B)^* = (A^*B^*)^*$

## Reflexión o Inverso de un Lenguaje

Dado *A* un lenguaje sobre $\Sigma$, se define $A^R$ de la siguiente
forma:

$A^R = \left\\{u^R : u \in A\right\\}$

donde:\
$u^R$ es la cadena inversa de *u*.\
$A^R$ se denomina la reflexión o el inverso de A.

**Propiedades:** Sean *A* y *B* lenguajes sobre $\Sigma$ (es decir,
$A, B \subseteq\Sigma^*$)

66. $(A \cdot B)^R = B^R \cdot A^R$

67. $(A \cup B)^R = A^R \cup B^R$

68. $(A \cap B)^R = A^R \cap B^R$

69. $(A^R)^R = A$

70. $(A^*)^R = (A^R)^*$

71. $(A^+)^R = (A^R)^+$

**Ejercicio:** Demuestre la propiedad 66 y 70.

66. $(A \cdot B)^R = B^R \cdot A^R$

    Por definición de Inverso de un Lenguaje:
    $A^R = \left\\{u^R | u \in B\right\\}$.\
    Sea $\omega \in (A \cdot B)^R$. Por definición de inversa de un
    lenguaje, existe $z \in A \cdot B$ y como $z \in A \cdot B$,
    $\therefore$ existen $x \in A$ y $y \in B$, tales que: $z = xy$.
    Entonces: $\omega = (xy)^R$.

    Ahora, por la definición de inversa, invertir una cadena significa
    escribir sus simbolos en orden contrario.\
    Si $x = a_1 \cdot\cdot\cdot a_n$, $y = b_1 \cdot\cdot\cdot b_m$,
    $x^R = a_n \cdot\cdot\cdot a_1$ y $y^R = b_m \cdot\cdot\cdot b_1$\
    entonces: $xy = a_1 \cdot\cdot\cdot a_n b_1 \cdot\cdot\cdot b_m$,
    por lo tanto:
    $(xy)^R = b_m \cdot\cdot\cdot b_1 a_n \cdot\cdot\cdot a_1 = y^Rx^R$\
    Así que: $\omega = y^Rx^R$.

    Como $y \in B$ y $x \in A$, entonces: $y^R \in B^R$ y $x^R \in A^R$,
    por lo tanto: $\omega \in B^RA^R$.

    Así, como: $\omega \in (A \cdot B)^R$ y $\omega \in B^RA^R$,
    $\quad\therefore(A \cdot B)^R = B^R \cdot A^R$

67. $(A^*)^R = (A^R)^*$

    Por definición de Clausura de Kleene:
    $A^* = \bigcup\limits_{n \geq 0} A^n$, entonces:
    $(A^*)^R = (\bigcup\limits_{n \geq 0} A^n)^R$. La inversa de una
    unión se puede distribuir:
    $(A^*)^R = \bigcup\limits_{n \geq 0} (A^n)^R$.

    Ahora, para cada *n*, invertir una cadena formada por *n* elementos
    de *A*, produce una cadena formada por *n*-elementos de $A^R$. Por
    lo tanto: $(A^n)^R = (A^R)^n$.

    Entonces: $(A^*)^R = \bigcup\limits_{n \geq 0} (A^R)^n$, de nuevo,
    por definición de Clausura de Kleene:
    $\bigcup\limits_{n \geq 0} (A^R)^n = (A^R)^*$,\
    Por lo tanto: $(A^*)^R = (A^R)^*$.

## Longitud de Cadenas

La longitud de una cadena $u\in\Sigma^*$ se denota $|u|$ y se define
como el número de símbolos de *u* (contando los símbolos repetidos). Es
decir, $$|u| = \begin{cases}
        0, & \text{si } u = \lambda,\\
        n, & \text{si } u = a_1a_2 \cdot\cdot\cdot a_n 
    \end{cases}$$ 

**Ejercicio:** Si $\omega\in\Sigma^*$,
$n,m\in\mathbb{N}$, demuestre que
$|\omega^{n+m}| = |\omega^n|+|\omega^m|$\
Por definición de potencia: $\omega^{n+m} = \omega^n\omega^m$. Entonces:
$|\omega^{n+m}| = |\omega^n\omega^m|$.\
Verémos en los últimos ejercicios de esta lista que:
$|xy| = |x| + |y|$,\
aplicándolo aquí: $|\omega^n\omega^m| = |\omega^n|+|\omega^m|$. Por lo
tanto: $|\omega^{n+m}| = |\omega^n| + |\omega^m|$

## *n-cadenas* o *n-palabras*

El siguiente teorema expresa el número de n-cadenas en función del
número de elementos del alfabeto.

72. Demuestre el siguiente teorema haciendo uso del Principio de
    Inducción Matemática.\
    **Teorema:** Sea $\Sigma$ un alfabeto. $\forall n \geq 1$ se cumple
    que:

    $|\Sigma^n| = |\Sigma|^n$

    Caso base ($n = 1$):\
    $\Sigma^1 = \Sigma$, entonces $|\Sigma^1| = |\Sigma|$. Y como:
    $|\Sigma| = |\Sigma|^1$, obtenemos: $|\Sigma| = |\Sigma|^1$.

    Hipótesis inductiva: Supongamos que para algún $n \geq 1$, se
    cumple: $|\Sigma^n| = |\Sigma|^n$.

    Paso inductivo ($n = n+1$):\
    Por definición de potencia de un lenguaje:
    $\Sigma^{n+1} = \Sigma^n\cdot\Sigma$, aplicando longitud de cadena:
    $|\Sigma^{n+1}| = |\Sigma^n| \cdot |\Sigma|$, aplicando la
    hipótesis:
    $|\Sigma^{n+1}| = |\Sigma|^n \cdot |\Sigma| = |\Sigma|^{n+1}$.
    Entonces: $|\Sigma^{n+1}| = |\Sigma|^{n+1}$

    Por lo tanto, por el principio de inducción matemática:
    $|\Sigma^n| = |\Sigma|^n, \quad\forall n\geq1$.

## Prefijos y Sufijos de una Cadena

Sean $\Sigma=\left\\{a,b,c,d\right\\}$ y $u = bcbaadb$.

73. Enumere todos los prefijos de *u*.

    1.  $\lambda$

    2.  *b*

    3.  *bc*

    4.  *bcb*

    5.  *bcba*

    6.  *bcbaa*

    7.  *bcbaad*

    8.  *bcbaadb*

74. Enumere todos los sufijos de *u*.

    1.  $\lambda$

    2.  *b*

    3.  *db*

    4.  *adb*

    5.  *aadb*

    6.  *baadb*

    7.  *cbaadb*

    8.  *bcbaadb*

## Potencias de un Lenguaje 

Dado un lenguaje *A* sobre $\Sigma (A \subseteq \Sigma^*)$ y un número
natural $n\in\mathbb{N}$, se define $A^n$ de la siguiente forma:\
$A^0=\left\\{\lambda\right\\}$,

$A^n= \underbrace{A \cdot A \cdot\cdot\cdot A}_{n \text{ veces}} = \left\\{u_1u_2 \cdot\cdot\cdot u_n : u_i \in A, \forall 1 \leq i \leq n\right\\}$\
De esta forma $A^2$ es el conjunto de las concatenaciones dobles de
cadenas de $A$, $A^3$ está formado por las concatenaciones triples y, en
general, $A^n$ es el conjunto de todas las concatenaciones de n cadenas
de $A$, de todas las formas posibles.

75. De una definición recursiva de $A^n$

    Sea *A* un lenguaje sobre $\Sigma$. Definimos recursivamente $A^n$
    como:

    Caso base: $A^0 = \left\\{\varepsilon\right\\}$

    Paso recursivo: $A^{n+1} = A^n \cdot A$

## Ejercicios

76. Sea $\Sigma=\left\\{0,1\right\\}$. Exhiba $\Sigma^n$ para *n* = 2, 3,
    4.\
    $\Sigma^2 = \left\\{00, 01, 10, 11\right\\}$\
    $\Sigma^3 = \left\\{000, 001, 010, 011, 100, 101, 110, 111\right\\}$\
    $\Sigma^4 = \left\\{0000, 0001, 0010, 0011, 0100, 0101, 0110, 0111, 1000, 1001, 1010, 1011, 1100, 1101, 1110, 1111\right\\}$

77. Demuestra que $|uv| = |u| + |v|$ para cualesquiera dos cadenas *u* y
    *v*.

    Por Inducción Matemática:

    Caso base ($v = \varepsilon$):\
    Por un lado: $|u\varepsilon| = |u|$.Del otro lado:
    $|u| + |\varepsilon| = |u| + 0 = |u|$.\
    Por lo tanto: $|u\varepsilon| = |u| + |\varepsilon|$

    Hipótesis Inductiva: $|uv| = |u| + |v|$.

    Paso inductivo:\
    Sea $v\alpha$ una cadena, donde $\alpha \in \Sigma$. Demostremos
    que: $|u(v\alpha)| = |u| + |v\alpha|$.\
    Por asociatividad: $u(v\alpha) = (uv)\alpha$, entonces:
    $|u(v\alpha)| = |(uv)\alpha|$\
    Aplicando la hipótesis:
    $|(uv)\alpha| = |uv| + |\alpha| = (|u| + |v|) + 1$, de nuevo por
    asociatividad: $(|u| + |v|) + 1 = |u| + (|v| + 1)$. Y como:
    $|v\alpha| = |v| + 1$, obtenemos: $|u(v\alpha)| = |u| + |v\alpha|$.

    Por lo tanto, se cumple que: $|uv| = |u| + |v|$.

78. Utiliza inducción para demostrar que $|u^n|=n|u|$ para cualquier
    cadena *u* y cualquier número natural *n*.

    Por Inducción Matemática:

    Caso base ($n = 0$):\
    Sabemos que: $u^0 = \varepsilon$. Entonces:
    $|u^0| = |\varepsilon| = 0$, así mismo: $0|u| = 0$.\
    $\therefore |u^0| = 0|u|$.

    Hipótesis Inductiva: Supongamos que para algún $n \geq 0$ se cumple:
    $|u^n| = n|u|$.

    Paso Inductivo: Demostrando que $|u^{n+1}| = (n+1)|u|$.\
    Por definición de potencia: $u^{n+1} = u^n \cdot u$, entonces:
    $|u^{n+1}| = |u^n| \cdot |u|$, aplicando la hipótesis:
    $|u^n| \cdot |u| = n|u| + |u|$, agrupando:
    $n|u| + |u| = (n + 1)|u|$.\
    Obtenemos: $|u^{n+1}| = (n+1)|u|$.

    Por lo tanto, se cumple que: $|u^n| = n|u|$.

79. El reverso de una cadena se define recursivamente como:

    $a^R = a$,\
    $(wa)^R=aw^R$

    para todo $a\in\Sigma$ y $w\in\Sigma^*$. Utilizando esta definición,
    demuestra que:

    $(uv)^R=v^Ru^R$

    para todo $u,v\in\Sigma^*$.

    Por Inducción Matemática:

    Caso base ($v = \varepsilon$):\
    Como $u \cdot \varepsilon = u$, entonces:
    $(u \cdot \varepsilon)^R = u^R$.\
    Además, como: $\varepsilon^R = \varepsilon$, entonces
    $\varepsilon^R \cdot u^R = \varepsilon \cdot u^R = u^R$
    $\therefore (u\cdot\varepsilon)^R = \varepsilon^R \cdot u^R$.

    Hipótesis Inductiva: Supóngase que se cumple
    $(u \cdot v)^R = v^R \cdot u^R$

    Paso Inductivo: Demostrando que $(uv\alpha)^R = (v\alpha)^R u^R$\
    Sea $(\alpha\in\Sigma)$ y $v\alpha$ una cadena. Por la definición
    del inverso de una cadena: $(uv\alpha)^R = \alpha(uv)^R$.\
    Aplicando la hipótesis: $\alpha(uv)^R = \alpha(v^R u^R)$, por
    asociatividad: $\alpha(v^R u^R) = (\alpha v^R) u^R$\
    Como: $(v\alpha)^R = \alpha v^R$, entonces:
    $(\alpha v^R) u^R = (v\alpha)^R u^R$.\
    Obtenemos: $(uv\alpha)^R = (v\alpha)^R u^R$.

    Por lo tanto, se cumple que: $(uv)^R=v^Ru^R$.

80. Dado el alfabeto $\Sigma=\left\\{a,b\right\\}$, determina $\Sigma^*$.

    $\Sigma^*$ representa el conjunto de todas las cadenas finitas que
    se pueden formar con *a* y *b*, incluyendo la cadena vacía
    $\varepsilon$.

    $\therefore \Sigma^* = \left\\{\varepsilon, a, b, aa, ab, ba, bb, aaa, aab, aba, abb, baa, bab, bba, bbb, aaaa, aaab, aaba, aabb ...\right\\}$

    Podemos expresarlo mediante la definición de Clausura de Kleene,
    como:

    $\Sigma^* = \bigcup\limits_{n \geq 0} \Sigma^n$

    a)  Da un ejemplo de un lenguaje finito sobre $\Sigma$\
        $L_1 = \left\\{\omega \in \Sigma^* : |\omega| \leq 3\right\\}$

    b)  Dado el lenguaje $L=\left\\{a^nb^n : n\geq0\right\\}$, determina
        si las cademas *aabb*, *aaaabbbb* y *abb* pertenece a *L*.

       1. $aabb = a^2b^2$, donde $n = 2$;
          $\therefore aabb \in L$.

       2. $aaaabbbb = a^4b^4$, donde $n = 4$;
          $\therefore aaaabbbb \in L$.

       3. $abb = a^1b^2$, como $1 \neq 2$;
          $\therefore abb \notin L$.

81. Dado el alfabeto $\Sigma=\left\\{a, b\right\\}$, determina $\Sigma^*$.

    En el ejercicio anterior, vimos que:

    $\Sigma^* = \left\\{\varepsilon, a, b, aa, ab, ba, bb, aaa, aab, aba, abb, baa, bab, bba, bbb, aaaa, aaab, aaba, aabb ...\right\\}$

    Además de que podemos expresarlo mediante la definición de Clausura
    de Kleene, como:

    $\Sigma^* = \bigcup\limits_{n \geq 0} \Sigma^n$

    a)  $L^2$\
        Dado que $L = \left\\{a, b\right\\}$, y $L^2 = L \cdot L$,
        entonces: $\therefore L^2 = \left\\{aa, ab, ba, bb\right\\}$

    b)  $L^R$\
        Por definición: $L^R = \left\\{\omega^R | \omega \in L\right\\}$,
        dado que: $L = \left\\{a, b\right\\}$ y
        $L^R = \left\\{a, b\right\\}$,
        $\therefore L^R = L = \left\\{a, b\right\\}$

82. Sea $L = \left\\{ab, aa, baa\right\\}$. ¿Cuáles de las siguientes
    cadenas pertenecen a $L^*$?

    a)  *abaabaaabaa*\
        $abaabaaabaa = ab \cdot aa \cdot baa \cdot ab \cdot aa$, donde
        todos los bloques pertenecen a L: $ab, aa, baa, ab, aa \in L$,
        $\therefore abaabaaabaa \in L^*$.

    b)  *aaaabaaaa*\
        $aaaabaaaa = aa \cdot aa \cdot baa \cdot aa$, donde todos los
        bloques pertenecen a L: $aa, aa, baa, aa \in L$,
        $\therefore aaaabaaaa \in L^*$.

    c)  *baaaaabaaaab*\
        $baaaaabaaaab = baa \cdot aa \cdot ab \cdot aa \cdot aa \cdot b$,
        donde $b \notin L$, $\therefore baaaaabaaaab \notin L$.

    d)  *baaaaabaa*\
        $baaaaabaa = baa \cdot aa \cdot ab \cdot aa$, donde todos los
        bloques pertenecen a L: $baa, aa, ab, aa \in L$,
        $\therefore baaaaabaa \in L$.

83. Dado el lenguaje $L = \left\\{ a^nb^{n+1} : n\geq0 \right\\}$, ¿es
    cierto que $L^*=L$ para este lenguaje en particular?

    Recordando que
    $L^* = \left\\{\text{concatenaciones de cero o más elementos de L}\right\\}$\
    Primero vemos que
    $L = \left\\{b, abb, aabbb, aaabbbb, aaaabbbbb, aaaaabbbbbb, ...\right\\}$\
    Ahora tomando el primer ejemplo de concatenación: $b \cdot b = bb$,
    sin embargo $bb \notin L$, $\therefore L^* \neq L$.

84. Dadas las cadenas $u = a^2ba^3b^2$ y $v=bab^2$, calcula:

    a)  *uv*\
        $u \cdot v = a^2ba^3b^2bab^2 = aabaaabbbabb$

    b)  *vu*\
        $v \cdot u = bab^2a^2ba^3b^2 = babbaabaaabb$

    c)  $v^2$\
        $v^2 = v \cdot v = bab^2bab^2 = babbbabb$

    d)  $u^2$\
        $u^2 = u \cdot u = a^2ba^3b^2a^2ba^3b^2 = aabaaabbaabaaabb$

    e)  $|u|$\
        $|u| = |a^2ba^3b^2| = |a^2|+|b|+|a^3|+|b^2| = 2+1+3+2 = 8$

    f)  $|v|$\
        $|v| = |bab^2| = |b|+|a|+|b^2| = 1+1+2 = 4$

    g)  $|uv|$\
        $|u \cdot v| = |u| + |v| = 8 + 4 = 12$

    h)  $|vu|$\
        $|v \cdot u| = |v| + |u| = 4 + 8 = 12$

    i)  $|v^2|$\
        $|v^2| = |v \cdot v| = |v| + |v| = 4 + 4 = 8$

    j) $|u^2|$\
        $|u^2| = |u \cdot u| = |u| + |u| = 8 + 8 = 16$

85. Demuestra que para cualquier par de cadenas *u* y *v*, se cumple
    que:

    a)  $|uv| = |u| + |v|$\
        Caso base ($v = \varepsilon$):\
        Como $u\cdot\varepsilon = u$, tenemos:
        $|u\cdot\varepsilon| = |u|$. Y como $|\varepsilon| = 0$:
        $|u| + |\varepsilon| = |u| + 0 = |u|$. Por lo tanto:
        $|u\cdot\varepsilon| = |u| + |\varepsilon|$.

       Hipótesis Inductiva: Supongamos que se cumple:
       $|u \cdot v| = |u| + |v|$.

       Paso Inductivo: Demostrando que:
       $|u(v\alpha)| = |u| + |v\alpha|$, con $\alpha \in \Sigma$.\
       Como $u(v\alpha) = (uv)\alpha$, tenemos:
       $|u(v\alpha)| = |(uv)\alpha|$. Aplicando la hipótesis de
       inducción:
       $|(uv)\alpha| = |u \cdot v| + |\alpha| = (|u| + |v|) + 1$, por
       asociatividad: $(|u| + |v|) + 1 = |u| + (|v| + 1)$. Y como:
       $|v \cdot \alpha| = |v| + |\alpha| = |v| + 1$. Obtenemos:
       $|u| + (|v| + 1) = |u| + |v\cdot\alpha|$.
       $\quad\therefore |u(v\alpha)| = |u| + |v\alpha|$.

       Por lo tanto, se cumple que: $|uv| = |u| + |v|$

    b)  $|uv| = |vu|$

       Utilizando la demostración anterior: $|uv| = |u| + |v|$.\
       Así mismo: $|vu| = |v| + |u|$. Como la suma de números es
       conmutativa, podemos decir que: $|u| + |v| = |v| + |u|$, por lo
       tanto: $|uv| = |vu|$.

86. Dado el alfabeto $A=\left\\{a, b, c\right\\}$, encuentra $L^*$ para:\
    Recordando que
    $L^* = \left\\{\text{concatenaciones de cero o más elementos de L}\right\\}$.

    a)  $L=\left\\{b^2\right\\}$\
        $L = \left\\{b^2\right\\} = \left\\{bb\right\\}$. Los elementos de L
        son únicamente la cadena $bb$. Al concatenarla consigo misma,
        obtenemos:\
        $L^* = \left\\{\varepsilon, bb, bbbb, bbbbbb, bbbbbbbb, ...\right\\}$,por
        lo tanto: $L^* = \left\\{b^{2n} : n \geq 0\right\\}$.

    b)  $L=\left\\{a, b\right\\}$\
        Los elementos de L son las cadenas a y b. Al concatenarlas,
        obtenermos todas las cadenas sobre $\left\\{a, b\right\\}$,
        incluyendo $\varepsilon$, obteniendo:\
        $L^* = \left\\{\varepsilon, a, b, aa, ab, ba, bb, aaa, aab, aba, abb, baa, bab, bba, bbb, ...\right\\}$.
        Podemos expresarlo como: $L^* = \left\\{a, b\right\\}^*$.

    c)  $L=\left\\{a,b,c^3\right\\}$\
        Podemos concatenar cualquier cantidad de *a*, *b* y bloques de
        tres *c's*;\
        incluyendo la cadena vacía ($\varepsilon$).

       Podemos decir:
       $L^* = \left\\{\omega \in \left\\{a,b,c\right\\}^*:\text{la cantidad de } c \text{ en 
       } \omega \text{ es múltiplo de } 3 \right\\}$
       
       O también:
       $L^* = \left\\{a,b,ccc\right\\}^*$

87. Para el lenguaje $L=\left\\{ab, c\right\\}$ sobre el alfabeto
    $A=\left\\{a, b, c\right\\}$, calcula:

    a)  $L^3$\
        $L^3 = \left\\{ababab, ababc, abcab, abcc, cabab, cabc, ccab, ccc\right\\}$.

    b)  $L^{-2}$\
        En lenguajes formales, **las potencias negativas de un lenguaje
        no están definidas**. Por lo tanto:\
        $L^{-2} \text{ no está definido}$.

    c)  $L^0$\
        La potencia cero de cualquier lenguaje es el lenguaje que
        contiene únicamente la cadena vacía.\
        $L^0 = \left\\{\lambda\right\\}$.

88. Dados los lenguajes $L_1 = \left\\{a, ab, a^2\right\\}$ y
    $L_2 = \left\\{b^2, aba\right\\}$ sobre el alfabeto
    $A = \left\\{a, b\right\\}$, determina:

    a)  $L_1L_2$\
        $L_1L_2 = \left\\{ab^2, a^2ba, ab^3, ababa, a^2b^2, a^3ba\right\\} = \left\\{abb, aaba, abbb, ababa, aabb, aaaba\right\\}$

    b)  $L_2L_2$\
        $L_2L_2 = \left\\{b^4, b^2aba, abab^2, aba^2ba\right\\} = \left\\{bbbb, bbaba, ababb, abaaba\right\\}$

89. Dados $u = a^2b$ y $v = b^3ab$, encuentra:

    a)  *uvu*\
        $uvu = a^2b \cdot b^3ab \cdot a^2b = aabbbbabaab$

    b)  $\lambda u$, $u \lambda$, $u \lambda v$\
        Hemos mencionado en varias ocaciones que:
        $\omega \cdot \lambda = \omega$. Por lo tanto:\
        $u \cdot \lambda = u = a^2b = aab$\
        $v \cdot \lambda = v = b^3ab = bbbab$\
        $u \cdot \lambda \cdot v = u \cdot v = a^2b \cdot b^3ab = aabbbbab$

90. Dado el alfabeto $A = \left\\{a, b, c\right\\}$, determina si $L_1$,
    $L_2$, $L_3$ y $L_4$ son lenguajes sobre *A*, donde:

    a)  $L_1 = \left\\{a, aa, ab, ac, abc, cab\right\\}$\
        Todas las cadenas están formadas por símbolos $a, b, c$, que
        pertenecen a *A*.\
        Por lo tanto: $L_1 \text{ SI es un lenguaje sobre } A$.

    b)  $L_2 = \left\\{aba, aabaa\right\\}$\
        Todas las cadenas están formadas por símbolos $a, b$, que
        pertenecen a *A*.\
        Por lo tanto: $L_2 \text{ SI es un lenguaje sobre } A$.

    c)  $L_3 = \left\\{\quad\right\\}$\
        El conjunto vacío no contiene ningúna cadena que pudiera
        utilizar símbolos fuera de *A*, además:
        $\varnothing \subseteq A^*$.\
        Por lo tanto: $L_3 \text{ SI es un lenguaje sobre } A$.

    d)  $L_4 = \left\\{a^icb^i : i\geq1\right\\}$\
        Las cadenas se pueden formar por símbolos $a, b, c$, que
        pertenecen a *A*.\
        Por lo tanto: $L_4 \text{ SI es un lenguaje sobre } A$.

91. a)  Dados $L_1 = \left\\{a^ib^j : i>j\geq1\right\\}$ y
        $L_2 = \left\\{a^ib^j : 1\leq i<j\right\\}$, encuentra
        $L_1 \cup L_2$.\
        La unión contiene las cadenas que pertenecen a $L_1$ o a $L_2$.
        Ahora, en $L_1: i>j$ y en $L_2: i<j$, sin embargo ambos son
        $\geq 1$.\
        Por lo tanto:
        $L_1 \cup L_2 = \left\\{a^ib^j : i,j \geq 1, i \neq j\right\\}$.

    b)  Dados $L_3 = \left\\{a^ib^ic^j : i,j\geq 1\right\\}$ y
        $L_4 = \left\\{a^ib^jc^j : i,j\geq 1\right\\}$, encuentra
        $L_3 \cap L_4$.\
        La intersección contiene las cadenas que pertenecen
        simultáneamente en $L_3$ y $L_4$. Ahora, en
        $L_3: |\omega|_a = |\omega|_b$ y en
        $L_4: |\omega|_b| = |\omega|_c$, por lo tanto, debe cumplirse:
        $|\omega|_a = |\omega|_b| = \omega|_c$.\
        Por lo tanto:
        $L_3 \cap L_4 = \left\\{a^ib^ic^i : i \geq 1\right\\}$.

92. Dados $L_1$ como el lenguaje del inglés y $L_2$ como el lenguaje del
    francés, ¿qué significan:

    a)  $L_1 \cup L_2$?\
        La unión contiene las cadenas que pertenecen a uno u otro
        lenguaje, entonces contiene **todas las palabras que están en
        inglés o en francés**.

    b)  $L_1 \cap L_2$?\
        La intersección contiene las cadenas que pertenecen
        simultáneamente a ambos lenguajes, entonces contiene **todas las
        palabras que están tanto en inglés como en francés**, por
        ejemplo: weekend, T-shirt, cool.

93. Sea $A=\left\\{a, b\right\\}$ y $B=\left\\{b, c, d\right\\}$\
    Definimos los siguientes lenguajes:

    $L_1 = \left\\{a^ib^j \quad|\quad i\geq1, j\geq1\right\\}$

    $L_2 = \left\\{b^ic^j \quad|\quad i\geq j\geq1\right\\}$

    $L_3 = \left\\{a^ib^jc^id^j \quad|\quad i\geq1, j\geq1\right\\}$

    $L_4 = \left\\{(ad)^ia^jd^j \quad|\quad i\geq2, j\geq1\right\\}$

    Determine si las siguientes afirmaciones son verdaderas o falsas:

    Primero calculamos los alfabetos combinados:

    $A \cup B = \left\\{a, b, c, d\right\\}$\
    $A \cap B = \left\\{b\right\\}$\
    $A - B = \left\\{a\right\\}$\
    $B - A = \left\\{c, d\right\\}$\
    $A \oplus B = (A - B) \cup (B - A) = \left\\{a, c, d\right\\}$


    a)  $L_1$ es un lenguaje sobre *A*.\
        $L_1$ utiliza únicamente *a* y *b*. Como:
        $\left\\{a,b\right\\} = A$, $\quad\therefore$ **VERDADERO**

    b)  $L_1$ es un lenguaje sobre *B*.\
        $L_1$ contiene cadenas con *a*, pero $a \notin B$,
        $\quad\therefore$ **FALSO**

    c)  $L_2$ es un lenguaje sobre $A \cup B$.\
        $L_2$ utiliza unicamente *b* y *c*. Como: $b, c \in A \cup B$,
        $\quad\therefore$ **VERDADERO**

    d)  $L_2$ es un lenguaje sobre $A \cap B$.\
        $L_2$ contiene cadenas con *c*, pero $c \notin A \cap B$,
        $\quad\therefore$ **FALSO**

    e)  $L_3$ es un lenguaje sobre $A \cup B$.\
        $L_3$ utiliza $a, b, c, d$, y como:
        $A \cup B = \left\\{a,b,c,d\right\\}$, $\quad\therefore$
        **VERDADERO**

    f)  $L_3$ es un lenguaje sobre $A \cap B$.\
        $L_3$ contiene cadenas con $a, c, d$, pero
        $a, c, d \notin A \cap B$, $\quad\therefore$ **FALSO**

    g)  $L_4$ es un lenguaje sobre $A \oplus B$.\
        $L_4$ utiliza únicamente *a* y *d*. Como: $a, d \in A \oplus B$,
        $\quad\therefore$ **VERDADERO**

    h)  $L_1$ es un lenguaje sobre $A - B$.\
        $L_1$ contiene *a* y *b*, pero $b \notin A - B$,
        $\quad\therefore$ **FALSO**

    i)  $L_1$ es un lenguaje sobre $B - A$.\
        $L_1$ contiene *a* y *b*, pero $B - A = \left\\{c, d\right\\}$ y
        $a, b \notin B - A$, $\quad\therefore$ **FALSO**

    j) $L_1 \cup L_2$ es un lenguaje sobre $A$.\
        $L_1$ utiliza $a, b$, y $L_2$ utiliza $b, c$. Sin embargo,
        $c \notin A^*$, $\quad\therefore$ **FALSO**

    k) $L_1 \cup L_2$ es un lenguaje sobre $A \cup B$.\
        $L_1$ utiliza $a, b$, y $L_2$ utiliza $b, c$. Además,
        $A \cup B = \left\\{a, b, c, d\right\\}$,\
        $\therefore$ **VERDADERO**

    l) $L_1 \cup L_2$ es un lenguaje sobre $A \cap B$.\
        $L_1$ utilizes $a, b$, y $L_2$ utiliza $b, c$. Sin embargo,
        $a, c \notin A \cap B$, $\quad\therefore$ **FALSO**

    m) $L_1 \cap L_2$ es un lenguaje sobre $B$.\
        $L_1 = \left\\{a^ib^j\right\\}$ y $L_2 = \left\\{b^ic^j\right\\}$.
        Para una intersección, una cadena debe pertenecer a ambos
        lenguajes. Sin embargo, $L_1$ contiene *a's* antes de las *b's*,
        mientras que $L_2$ contiene *b's* antes de las *c's*. Por lo
        tanto, no hay una cadena que pueda satisfacer ambas formas con
        $i,j \geq 1$. Por eso: $L_1 \cap L_2 = \varnothing$.

       Como: $\varnothing \subseteq B^*$, $\quad\therefore$
        **VERDADERO**

    n) $L_1 \cap L_2$ es un lenguaje sobre $A \cup B$.\
        Ya vimos que $L_1 \cap L_2 = \varnothing$, y como
        $\varnothing \subseteq (A \cup B)^*$, $\quad\therefore$
        **VERDADERO**

    o) $L_1 \cap L_2$ es un lenguaje sobre $A \cap B$.\
        Ya vimos que $L_1 \cap L_2 = \varnothing$, y como
        $\varnothing \subseteq (A \cap B)^*$, $\quad\therefore$
        **VERDADERO**
