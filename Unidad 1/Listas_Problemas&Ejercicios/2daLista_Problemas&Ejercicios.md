# 2da Lista de Problemas y Ejercicios 
**Escuela Superior de Cómputo**\
Teoría de la Computación $|$ 4CV4\
Sánchez Iriarte Juan Pablo $|$ 2025630142

## Autómatas Finitos

En los problemas 94 - 123, debe hallar un Autómata Finito Determinista
(AFD) que distinga las palabras del lenguaje que se describe con el
alfabeto que se indica. Debe representar la respuesta usando el diagrama
de transiciones y la tabla de transiciones. Los alfabetos utilizados
son:

$\Sigma_1 = \left\\{0,1,2\right\\}$,
$\quad\Sigma_2 = \left\\{a,b,c,0,1\right\\}$, 
$\quad\Sigma_3 = \left\\{a,b\right\\}$

- **97.** Las palabras de $\Sigma_1$ cuya longitud es un multiplo de 3.

    <figure data-latex-placement="H">
    <div class="minipage">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_97.png" style="height:4cm" />
    </div>
      
    <div class="minipage">
    <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">Entrada (0, 1 o 2)</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0 *$</td>
            <td style="text-align: center;">$q_1$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_0$</td>
        </tr>
      </tbody>
    </table>
    </div>
    </figure>

- **99.** Las palabras de $\Sigma_1$ que terminan con la cadena *001001*.

    <figure data-latex-placement="h">
    <div class="minipage">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_99.png" style="height:4cm" />
    </div>
    <div class="minipage">
    <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$\rightarrow q_0$</th>
            <th style="text-align: center;">$q_1$</th>
            <th style="text-align: center;">$q_2$</th>
            <th style="text-align: center;">$q_3$</th>
            <th style="text-align: center;">$q_4$</th>
            <th style="text-align: center;">$q_5$</th>
            <th style="text-align: center;">$q_6 *$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$0$</td>
            <td style="text-align: center;">$q_1$</td>
            <th style="text-align: center;">$q_2$</th>
            <th style="text-align: center;">$q_2$</th>
            <th style="text-align: center;">$q_4$</th>
            <th style="text-align: center;">$q_5$</th>
            <th style="text-align: center;">$q_2$</th>
            <th style="text-align: center;">$q_1$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$1$</td>
            <td style="text-align: center;">$q_0$</td>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_3$</th>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_6$</th>
            <th style="text-align: center;">$q_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$2$</td>
            <td style="text-align: center;">$q_0$</td>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_0$</th>
        </tr>
      </tbody>
    </table>
    </div>
    </figure>

- **102.** Las palabras de $\Sigma_3$ que contienen la cadema *abbbab*.

    <figure data-latex-placement="h">
    <div class="minipage">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_102.png" style="height:4cm" />
    </div>
    <div class="minipage">
    <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$\rightarrow q_0$</th>
            <th style="text-align: center;">$q_1$</th>
            <th style="text-align: center;">$q_2$</th>
            <th style="text-align: center;">$q_3$</th>
            <th style="text-align: center;">$q_4$</th>
            <th style="text-align: center;">$q_5$</th>
            <th style="text-align: center;">$q_6 *$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$a$</td>
            <td style="text-align: center;">$q_1$</td>
            <th style="text-align: center;">$q_1$</th>
            <th style="text-align: center;">$q_1$</th>
            <th style="text-align: center;">$q_1$</th>
            <th style="text-align: center;">$q_5$</th>
            <th style="text-align: center;">$q_1$</th>
            <th style="text-align: center;">$q_6$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$b$</td>
            <td style="text-align: center;">$q_0$</td>
            <th style="text-align: center;">$q_2$</th>
            <th style="text-align: center;">$q_3$</th>
            <th style="text-align: center;">$q_4$</th>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_6$</th>
            <th style="text-align: center;">$q_6$</th>
        </tr>
      </tbody>
    </table>
    </div>
    </figure>

- **103.** Las palabras de $\Sigma_3$ que contienen la cadema *aabbba*.

     <figure data-latex-placement="h">
     <div class="minipage">
     <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_103.png" style="height:4cm" />
     </div>
     <div class="minipage">
     <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$\rightarrow q_0$</th>
            <th style="text-align: center;">$q_1$</th>
            <th style="text-align: center;">$q_2$</th>
            <th style="text-align: center;">$q_3$</th>
            <th style="text-align: center;">$q_4$</th>
            <th style="text-align: center;">$q_5$</th>
            <th style="text-align: center;">$q_6 *$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$0$</td>
            <td style="text-align: center;">$q_1$</td>
            <th style="text-align: center;">$q_2$</th>
            <th style="text-align: center;">$q_2$</th>
            <th style="text-align: center;">$q_1$</th>
            <th style="text-align: center;">$q_1$</th>
            <th style="text-align: center;">$q_6$</th>
            <th style="text-align: center;">$q_6$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$1$</td>
            <td style="text-align: center;">$q_0$</td>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_3$</th>
            <th style="text-align: center;">$q_4$</th>
            <th style="text-align: center;">$q_5$</th>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_6$</th>
        </tr>
      </tbody>
    </table>
     </div>
     </figure>

- **106.** Las palabas de $\Sigma_1$ que incluyen la subcadena *1101001*.

     <figure data-latex-placement="h">
     <div class="minipage">
     <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_106.png" style="height:4cm" />
     </div>
     <div class="minipage">
     <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$\rightarrow q_0$</th>
            <th style="text-align: center;">$q_1$</th>
            <th style="text-align: center;">$q_2$</th>
            <th style="text-align: center;">$q_3$</th>
            <th style="text-align: center;">$q_4$</th>
            <th style="text-align: center;">$q_5$</th>
            <th style="text-align: center;">$q_6$</th>
            <th style="text-align: center;">$q_7 *$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$0$</td>
            <td style="text-align: center;">$q_0$</td>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_3$</th>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_5$</th>
            <th style="text-align: center;">$q_6$</th>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_7$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$1$</td>
            <td style="text-align: center;">$q_1$</td>
            <th style="text-align: center;">$q_2$</th>
            <th style="text-align: center;">$q_2$</th>
            <th style="text-align: center;">$q_4$</th>
            <th style="text-align: center;">$q_2$</th>
            <th style="text-align: center;">$q_1$</th>
            <th style="text-align: center;">$q_7$</th>
            <th style="text-align: center;">$q_7$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$2$</td>
            <td style="text-align: center;">$q_0$</td>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_0$</th>
            <th style="text-align: center;">$q_7$</th>
        </tr>
      </tbody>
     </table>
     </div>
     </figure>

- **107.** Las palabras de $\Sigma_1$ que incluyen al menos una vez la
     subcadena *0101* y al menos una vez la subcadena *021*.

     Veamos que el AFD debe recordar ambas cosas simultáneamente,
     usaremos:\
     $q \rightarrow$ para buscar *0101*:
     $q_0 \rightarrow q_1 \rightarrow q_2 \rightarrow q_3 \rightarrow q_4$,
     donde $q_0$ es el estado inicial y $q_4$ el estado final.\
     $p \rightarrow$ para buscar *021*:
     $p_0 \rightarrow p_1 \rightarrow p_2 \rightarrow p_3$, donde $p_0$
     es el estado inicial y $p_3$ el estado final.

     Combinaremos todos los estados finales: 5 estados *q* x 4 estados
     *p* = **20 estados**.

     <figure data-latex-placement="h">
     <div class="minipage">
     <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_107.png" style="height:4cm" />
     </div>
     <div class="minipage">
     <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
            <th style="text-align: center;">$2$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0p_0$</td>
            <td style="text-align: center;">$q_1p_1$</td>
            <th style="text-align: center;">$q_0p_0$</th>
            <th style="text-align: center;">$q_0p_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_0p_1$</td>
            <td style="text-align: center;">$q_1p_1$</td>
            <th style="text-align: center;">$q_0p_0$</th>
            <th style="text-align: center;">$q_0p_2$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_0p_2$</td>
            <td style="text-align: center;">$q_1p_1$</td>
            <th style="text-align: center;">$q_0p_3$</th>
            <th style="text-align: center;">$q_0p_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_0p_3$</td>
            <td style="text-align: center;">$q_1p_3$</td>
            <th style="text-align: center;">$q_0p_3$</th>
            <th style="text-align: center;">$q_0p_3$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1p_0$</td>
            <td style="text-align: center;">$q_1p_1$</td>
            <th style="text-align: center;">$q_2p_0$</th>
            <th style="text-align: center;">$q_0p_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1p_1$</td>
            <td style="text-align: center;">$q_1p_1$</td>
            <th style="text-align: center;">$q_2p_0$</th>
            <th style="text-align: center;">$q_0p_2$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1p_2$</td>
            <td style="text-align: center;">$q_1p_1$</td>
            <th style="text-align: center;">$q_2p_3$</th>
            <th style="text-align: center;">$q_0p_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1p_3$</td>
            <td style="text-align: center;">$q_1p_3$</td>
            <th style="text-align: center;">$q_2p_3$</th>
            <th style="text-align: center;">$q_0p_3$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2p_0$</td>
            <td style="text-align: center;">$q_3p_1$</td>
            <th style="text-align: center;">$q_0p_0$</th>
            <th style="text-align: center;">$q_0p_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2p_1$</td>
            <td style="text-align: center;">$q_3p_1$</td>
            <th style="text-align: center;">$q_0p_0$</th>
            <th style="text-align: center;">$q_0p_2$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2p_2$</td>
            <td style="text-align: center;">$q_3p_1$</td>
            <th style="text-align: center;">$q_0p_3$</th>
            <th style="text-align: center;">$q_0p_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2p_3$</td>
            <td style="text-align: center;">$q_3p_3$</td>
            <th style="text-align: center;">$q_0p_3$</th>
            <th style="text-align: center;">$q_0p_3$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3p_0$</td>
            <td style="text-align: center;">$q_1p_1$</td>
            <th style="text-align: center;">$q_4p_0$</th>
            <th style="text-align: center;">$q_0p_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3p_1$</td>
            <td style="text-align: center;">$q_1p_1$</td>
            <th style="text-align: center;">$q_4p_0$</th>
            <th style="text-align: center;">$q_0p_2$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3p_2$</td>
            <td style="text-align: center;">$q_1p_1$</td>
            <th style="text-align: center;">$q_4p_3$</th>
            <th style="text-align: center;">$q_0p_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3p_3$</td>
            <td style="text-align: center;">$q_1p_3$</td>
            <th style="text-align: center;">$q_4p_3$</th>
            <th style="text-align: center;">$q_0p_3$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_4p_0$</td>
            <td style="text-align: center;">$q_4p_1$</td>
            <th style="text-align: center;">$q_4p_0$</th>
            <th style="text-align: center;">$q_4p_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_4p_1$</td>
            <td style="text-align: center;">$q_4p_1$</td>
            <th style="text-align: center;">$q_4p_0$</th>
            <th style="text-align: center;">$q_4p_2$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_4p_2$</td>
            <td style="text-align: center;">$q_4p_1$</td>
            <th style="text-align: center;">$q_4p_3$</th>
            <th style="text-align: center;">$q_4p_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_4p_3 *$</td>
            <td style="text-align: center;">$q_4p_3$</td>
            <th style="text-align: center;">$q_4p_3$</th>
            <th style="text-align: center;">$q_4p_3$</th>
        </tr>
      </tbody>
     </table>
     </div>
     </figure>

- **109.** Las palabras de $\Sigma_2$ que incluyen al menos una vez la
     subcadena de *abbcb* y al menos una vez la subcadena *cbaabb*,
     asumiendo que sí se pueden traslapar.

     Veamos que el AFD debe recordar ambas cosas simultáneamente,
     usaremos:\
     $q \rightarrow$ para buscar *abbcb*:
     $q_0 \rightarrow q_1 \rightarrow q_2 \rightarrow q_3 \rightarrow q_4 \rightarrow q_5$,
     donde $q_0$ es el estado inicial y $q_5$ el estado final.\
     $r \rightarrow$ para buscar *cbaabb*:
     $r_0 \rightarrow r_1 \rightarrow r_2 \rightarrow r_3 \rightarrow r_4 \rightarrow r_5 \rightarrow r_6$,
     donde $r_0$ es el estado inicial y $r_6$ el estado final.

     Combinaremos todos los estados finales: 6 estados *q* x 7 estados
     *r* = **42 estados**.

     <figure data-latex-placement="H">
     <div class="minipage">
     <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_109.png" style="height:4cm" />
     </div>
     <div class="minipage">
     <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$a$</th>
            <th style="text-align: center;">$b$</th>
            <th style="text-align: center;">$c$</th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0r_0$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_0r_0$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_0r_0$</th>
            <th style="text-align: center;">$q_0r_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_0r_1$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_0r_2$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_0r_1$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_0r_2$</td>
            <td style="text-align: center;">$q_1r_3$</td>
            <th style="text-align: center;">$q_0r_0$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_0r_2$</th>
            <th style="text-align: center;">$q_0r_2$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_0r_3$</td>
            <td style="text-align: center;">$q_1r_4$</td>
            <th style="text-align: center;">$q_0r_0$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_0r_3$</th>
            <th style="text-align: center;">$q_0r_3$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_0r_4$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_0r_5$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_0r_4$</th>
            <th style="text-align: center;">$q_0r_4$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_0r_5$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_0r_6$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_0r_5$</th>
            <th style="text-align: center;">$q_0r_5$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_0r_6$</td>
            <td style="text-align: center;">$q_1r_6$</td>
            <th style="text-align: center;">$q_0r_6$</th>
            <th style="text-align: center;">$q_0r_6$</th>
            <th style="text-align: center;">$q_0r_6$</th>
            <th style="text-align: center;">$q_0r_6$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1r_0$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_2r_0$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_1r_0$</th>
            <th style="text-align: center;">$q_1r_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1r_1$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_2r_2$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_1r_1$</th>
            <th style="text-align: center;">$q_1r_1$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1r_2$</td>
            <td style="text-align: center;">$q_1r_3$</td>
            <th style="text-align: center;">$q_2r_0$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_1r_2$</th>
            <th style="text-align: center;">$q_1r_2$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1r_3$</td>
            <td style="text-align: center;">$q_1r_4$</td>
            <th style="text-align: center;">$q_2r_0$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_1r_3$</th>
            <th style="text-align: center;">$q_1r_3$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1r_4$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_2r_5$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_1r_4$</th>
            <th style="text-align: center;">$q_1r_4$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1r_5$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_2r_6$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_1r_5$</th>
            <th style="text-align: center;">$q_1r_5$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1r_6$</td>
            <td style="text-align: center;">$q_1r_6$</td>
            <th style="text-align: center;">$q_2r_6$</th>
            <th style="text-align: center;">$q_0r_6$</th>
            <th style="text-align: center;">$q_1r_6$</th>
            <th style="text-align: center;">$q_1r_6$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2r_0$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_3r_0$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_2r_0$</th>
            <th style="text-align: center;">$q_2r_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2r_1$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_3r_2$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_2r_1$</th>
            <th style="text-align: center;">$q_2r_1$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2r_2$</td>
            <td style="text-align: center;">$q_1r_3$</td>
            <th style="text-align: center;">$q_3r_0$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_2r_2$</th>
            <th style="text-align: center;">$q_2r_2$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2r_3$</td>
            <td style="text-align: center;">$q_1r_4$</td>
            <th style="text-align: center;">$q_3r_0$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_2r_3$</th>
            <th style="text-align: center;">$q_2r_3$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2r_4$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_3r_5$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_2r_4$</th>
            <th style="text-align: center;">$q_2r_4$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2r_5$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_3r_6$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_2r_5$</th>
            <th style="text-align: center;">$q_2r_5$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2r_6$</td>
            <td style="text-align: center;">$q_1r_6$</td>
            <th style="text-align: center;">$q_3r_6$</th>
            <th style="text-align: center;">$q_0r_6$</th>
            <th style="text-align: center;">$q_2r_6$</th>
            <th style="text-align: center;">$q_2r_6$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3r_0$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_0r_0$</th>
            <th style="text-align: center;">$q_4r_1$</th>
            <th style="text-align: center;">$q_3r_0$</th>
            <th style="text-align: center;">$q_3r_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3r_1$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_0r_2$</th>
            <th style="text-align: center;">$q_4r_1$</th>
            <th style="text-align: center;">$q_3r_1$</th>
            <th style="text-align: center;">$q_3r_1$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3r_2$</td>
            <td style="text-align: center;">$q_1r_3$</td>
            <th style="text-align: center;">$q_0r_0$</th>
            <th style="text-align: center;">$q_4r_1$</th>
            <th style="text-align: center;">$q_3r_2$</th>
            <th style="text-align: center;">$q_3r_2$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3r_3$</td>
            <td style="text-align: center;">$q_1r_4$</td>
            <th style="text-align: center;">$q_0r_0$</th>
            <th style="text-align: center;">$q_4r_1$</th>
            <th style="text-align: center;">$q_3r_3$</th>
            <th style="text-align: center;">$q_3r_3$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3r_4$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_0r_5$</th>
            <th style="text-align: center;">$q_4r_1$</th>
            <th style="text-align: center;">$q_3r_4$</th>
            <th style="text-align: center;">$q_3r_4$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3r_5$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_0r_6$</th>
            <th style="text-align: center;">$q_4r_1$</th>
            <th style="text-align: center;">$q_3r_5$</th>
            <th style="text-align: center;">$q_3r_5$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3r_6$</td>
            <td style="text-align: center;">$q_1r_6$</td>
            <th style="text-align: center;">$q_0r_6$</th>
            <th style="text-align: center;">$q_4r_6$</th>
            <th style="text-align: center;">$q_3r_6$</th>
            <th style="text-align: center;">$q_3r_6$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_4r_0$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_5r_0$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_4r_0$</th>
            <th style="text-align: center;">$q_4r_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_4r_1$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_5r_2$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_4r_1$</th>
            <th style="text-align: center;">$q_4r_1$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_4r_2$</td>
            <td style="text-align: center;">$q_1r_3$</td>
            <th style="text-align: center;">$q_5r_0$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_4r_2$</th>
            <th style="text-align: center;">$q_4r_2$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_4r_3$</td>
            <td style="text-align: center;">$q_1r_4$</td>
            <th style="text-align: center;">$q_5r_0$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_4r_3$</th>
            <th style="text-align: center;">$q_4r_3$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_4r_4$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_5r_5$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_4r_4$</th>
            <th style="text-align: center;">$q_4r_4$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_4r_5$</td>
            <td style="text-align: center;">$q_1r_0$</td>
            <th style="text-align: center;">$q_5r_6$</th>
            <th style="text-align: center;">$q_0r_1$</th>
            <th style="text-align: center;">$q_4r_5$</th>
            <th style="text-align: center;">$q_4r_5$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_4r_6$</td>
            <td style="text-align: center;">$q_1r_6$</td>
            <th style="text-align: center;">$q_5r_6$</th>
            <th style="text-align: center;">$q_0r_6$</th>
            <th style="text-align: center;">$q_4r_6$</th>
            <th style="text-align: center;">$q_4r_6$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_5r_0$</td>
            <td style="text-align: center;">$q_5r_0$</td>
            <th style="text-align: center;">$q_5r_0$</th>
            <th style="text-align: center;">$q_5r_1$</th>
            <th style="text-align: center;">$q_5r_0$</th>
            <th style="text-align: center;">$q_5r_0$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_5r_1$</td>
            <td style="text-align: center;">$q_5r_0$</td>
            <th style="text-align: center;">$q_5r_2$</th>
            <th style="text-align: center;">$q_5r_1$</th>
            <th style="text-align: center;">$q_5r_1$</th>
            <th style="text-align: center;">$q_5r_1$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_5r_2$</td>
            <td style="text-align: center;">$q_5r_3$</td>
            <th style="text-align: center;">$q_5r_0$</th>
            <th style="text-align: center;">$q_5r_1$</th>
            <th style="text-align: center;">$q_5r_2$</th>
            <th style="text-align: center;">$q_5r_2$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_5r_3$</td>
            <td style="text-align: center;">$q_5r_4$</td>
            <th style="text-align: center;">$q_5r_0$</th>
            <th style="text-align: center;">$q_5r_1$</th>
            <th style="text-align: center;">$q_5r_3$</th>
            <th style="text-align: center;">$q_5r_3$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_5r_4$</td>
            <td style="text-align: center;">$q_5r_0$</td>
            <th style="text-align: center;">$q_5r_5$</th>
            <th style="text-align: center;">$q_5r_1$</th>
            <th style="text-align: center;">$q_5r_4$</th>
            <th style="text-align: center;">$q_5r_4$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_5r_5$</td>
            <td style="text-align: center;">$q_5r_0$</td>
            <th style="text-align: center;">$q_5r_6$</th>
            <th style="text-align: center;">$q_5r_1$</th>
            <th style="text-align: center;">$q_5r_5$</th>
            <th style="text-align: center;">$q_5r_5$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_5r_6 *$</td>
            <td style="text-align: center;">$q_5r_6$</td>
            <th style="text-align: center;">$q_5r_6$</th>
            <th style="text-align: center;">$q_5r_6$</th>
            <th style="text-align: center;">$q_5r_6$</th>
            <th style="text-align: center;">$q_5r_6$</th>
        </tr>
      </tbody>
     </table>
     </div>
     </figure>

- **111.** Las palabras de $\Sigma_1$ que contienen exactamente tres veces la
     subcadena *01002*.

     Para este ejercicio se utilizará para el nombre de los estados el formato: $q_{n_m}$,\
     dónde *n* es el contador de ocurrencias detectadas de la subcaden y *m* es el progreso del         patrón.

     <figure data-latex-placement="H">
     <div class="minipage">
     <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_111.png" style="height:4cm" />
     </div>
     <div class="minipage">
     <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
            <th style="text-align: center;">$2$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_{0_0}$</td>
            <td style="text-align: center;">$q_{0_1}$</td>
            <th style="text-align: center;">$q_{0_0}$</th>
            <th style="text-align: center;">$q_{0_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{0_1}$</td>
            <td style="text-align: center;">$q_{0_1}$</td>
            <th style="text-align: center;">$q_{0_2}$</th>
            <th style="text-align: center;">$q_{0_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{0_2}$</td>
            <td style="text-align: center;">$q_{0_3}$</td>
            <th style="text-align: center;">$q_{0_0}$</th>
            <th style="text-align: center;">$q_{0_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{0_3}$</td>
            <td style="text-align: center;">$q_{0_4}$</td>
            <th style="text-align: center;">$q_{0_2}$</th>
            <th style="text-align: center;">$q_{0_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{0_4}$</td>
            <td style="text-align: center;">$q_{0_1}$</td>
            <th style="text-align: center;">$q_{0_0}$</th>
            <th style="text-align: center;">$q_{1_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{1_0}$</td>
            <td style="text-align: center;">$q_{1_1}$</td>
            <th style="text-align: center;">$q_{1_0}$</th>
            <th style="text-align: center;">$q_{1_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{1_1}$</td>
            <td style="text-align: center;">$q_{1_1}$</td>
            <th style="text-align: center;">$q_{1_2}$</th>
            <th style="text-align: center;">$q_{1_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{1_2}$</td>
            <td style="text-align: center;">$q_{1_3}$</td>
            <th style="text-align: center;">$q_{1_0}$</th>
            <th style="text-align: center;">$q_{1_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{1_3}$</td>
            <td style="text-align: center;">$q_{1_4}$</td>
            <th style="text-align: center;">$q_{1_2}$</th>
            <th style="text-align: center;">$q_{1_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{1_4}$</td>
            <td style="text-align: center;">$q_{1_1}$</td>
            <th style="text-align: center;">$q_{1_0}$</th>
            <th style="text-align: center;">$q_{2_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{2_0}$</td>
            <td style="text-align: center;">$q_{2_1}$</td>
            <th style="text-align: center;">$q_{2_0}$</th>
            <th style="text-align: center;">$q_{2_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{2_1}$</td>
            <td style="text-align: center;">$q_{2_1}$</td>
            <th style="text-align: center;">$q_{2_2}$</th>
            <th style="text-align: center;">$q_{2_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{2_2}$</td>
            <td style="text-align: center;">$q_{2_3}$</td>
            <th style="text-align: center;">$q_{2_0}$</th>
            <th style="text-align: center;">$q_{2_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{2_3}$</td>
            <td style="text-align: center;">$q_{2_4}$</td>
            <th style="text-align: center;">$q_{2_2}$</th>
            <th style="text-align: center;">$q_{2_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{2_4}$</td>
            <td style="text-align: center;">$q_{2_1}$</td>
            <th style="text-align: center;">$q_{2_0}$</th>
            <th style="text-align: center;">$q_{3_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{3_0} *$</td>
            <td style="text-align: center;">$q_{3_1}$</td>
            <th style="text-align: center;">$q_{3_0}$</th>
            <th style="text-align: center;">$q_{3_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{3_1} *$</td>
            <td style="text-align: center;">$q_{3_1}$</td>
            <th style="text-align: center;">$q_{3_2}$</th>
            <th style="text-align: center;">$q_{3_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{3_2} *$</td>
            <td style="text-align: center;">$q_{3_3}$</td>
            <th style="text-align: center;">$q_{3_0}$</th>
            <th style="text-align: center;">$q_{3_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{3_3} *$</td>
            <td style="text-align: center;">$q_{3_4}$</td>
            <th style="text-align: center;">$q_{3_2}$</th>
            <th style="text-align: center;">$q_{3_0}$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{3_4} *$</td>
            <td style="text-align: center;">$q_{3_1}$</td>
            <th style="text-align: center;">$q_{3_0}$</th>
            <th style="text-align: center;">$q_4$</th>
        </tr>
        <tr>
            <td style="text-align: center;">$q_4$</td>
            <td style="text-align: center;">$q_4$</td>
            <th style="text-align: center;">$q_4$</th>
            <th style="text-align: center;">$q_4$</th>
        </tr>
      </tbody>
     </table>
     </div>
     </figure>

- **112.** Las palabras de $\Sigma_1$ que contienen dos veces la cadena *010*,
     asumiendo que no se pueden traslapar; es decir, que *01010* no está
     en el lenguaje, mientras que *010010* sí pertenece.

     <figure data-latex-placement="H">
     <div class="minipage">
     <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_112.png" style="height:4cm" />
     </div>
     <div class="minipage">
     <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
            <th style="text-align: center;">$2$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_{0_0}$</td>
            <td style="text-align: center;">$q_{0_1}$</td>
            <td style="text-align: center;">$q_{0_0}$</td>
            <td style="text-align: center;">$q_{0_0}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{0_1}$</td>
            <td style="text-align: center;">$q_{0_1}$</td>
            <td style="text-align: center;">$q_{0_2}$</td>
            <td style="text-align: center;">$q_{0_0}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{0_2}$</td>
            <td style="text-align: center;">$q_{1_0}$</td>
            <td style="text-align: center;">$q_{0_0}$</td>
            <td style="text-align: center;">$q_{0_0}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{1_0}$</td>
            <td style="text-align: center;">$q_{1_1}$</td>
            <td style="text-align: center;">$q_{1_0}$</td>
            <td style="text-align: center;">$q_{1_0}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{1_1}$</td>
            <td style="text-align: center;">$q_{1_1}$</td>
            <td style="text-align: center;">$q_{1_2}$</td>
            <td style="text-align: center;">$q_{1_0}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{1_2}$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_{1_0}$</td>
            <td style="text-align: center;">$q_{1_0}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2 *$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_2$</td>
        </tr>
      </tbody>
     </table>
     </div>
     </figure>

- **113.** Las palabras de $\Sigma_1$ que contienen dos veces la subcadena
     $010$, asumiendo que sí se pueden traslapar.

     <figure data-latex-placement="H">
     <div class="minipage">
     <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_113.png" style="height:4cm" />
     </div>
     <div class="minipage">
     <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
            <th style="text-align: center;">$2$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_{0_0}$</td>
            <td style="text-align: center;">$q_{0_1}$</td>
            <td style="text-align: center;">$q_{0_0}$</td>
            <td style="text-align: center;">$q_{0_0}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{0_1}$</td>
            <td style="text-align: center;">$q_{0_1}$</td>
            <td style="text-align: center;">$q_{0_2}$</td>
            <td style="text-align: center;">$q_{0_0}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{0_2}$</td>
            <td style="text-align: center;">$q_{1_1}$</td>
            <td style="text-align: center;">$q_{0_0}$</td>
            <td style="text-align: center;">$q_{0_0}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{1_0}$</td>
            <td style="text-align: center;">$q_{1_1}$</td>
            <td style="text-align: center;">$q_{1_0}$</td>
            <td style="text-align: center;">$q_{1_0}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{1_1}$</td>
            <td style="text-align: center;">$q_{1_1}$</td>
            <td style="text-align: center;">$q_{1_2}$</td>
            <td style="text-align: center;">$q_{1_0}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{1_2}$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_{1_0}$</td>
            <td style="text-align: center;">$q_{1_0}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2 *$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_2$</td>
        </tr>
      </tbody>
     </table>
     </div>
     </figure>

- **116.** $L = \left\\{\omega \in \Sigma_2 \quad:\quad \omega = a^nb^mc^{n+1}, m, n \in \mathbb{N}\right\\}$

     **Este lenguaje NO ES REGULAR**, por lo que no se puede construir
     un **Autómata Finito Determinista (AFD)**.

     La razón, *n* puede ser cualquier numero natural, y la máquina
     necesita *\"recordar\"* cuántos símbolos *a* leyó para asegurar que
     al final aparezcan *n + 1* simbolos *c*. Como un AFD tiene memoria
     finita (numero fijo de estados), no puede contar infinitas *a's*.

- **118.** $L = \left\\{\omega \in \Sigma_3 \quad:\quad \omega = axabya, x,y \in \Sigma_3^*\right\\}$

     <figure data-latex-placement="H">
     <div class="minipage">
     <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_118.png" style="height:4cm" />
     </div>
     <div class="minipage">
     <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$a$</th>
            <th style="text-align: center;">$b$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0$</td>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_m$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_1$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_3$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3$</td>
            <td style="text-align: center;">$q_4$</td>
            <td style="text-align: center;">$q_3$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_4 *$</td>
            <td style="text-align: center;">$q_4$</td>
            <td style="text-align: center;">$q_5$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_5$</td>
            <td style="text-align: center;">$q_4$</td>
            <td style="text-align: center;">$q_m$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
        </tr>
      </tbody>
     </table>
     </div>
     </figure>

- **120.** Las palabras de $\Sigma_1$ tales que el primer carácter y el último
     sean distintos.

     <figure data-latex-placement="H">
     <div class="minipage">
     <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_120.png" style="height:4cm" />
     </div>
     <div class="minipage">
     <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
            <th style="text-align: center;">$2$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0$</td>
            <td style="text-align: center;">$f_0c_0$</td>
            <td style="text-align: center;">$f_1c_1$</td>
            <td style="text-align: center;">$f_2c_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$f_0c_0$</td>
            <td style="text-align: center;">$f_0c_0$</td>
            <td style="text-align: center;">$f_0c_1$</td>
            <td style="text-align: center;">$f_0c_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$f_0c_1 *$</td>
            <td style="text-align: center;">$f_0c_0$</td>
            <td style="text-align: center;">$f_0c_1$</td>
            <td style="text-align: center;">$f_0c_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$f_0c_2 *$</td>
            <td style="text-align: center;">$f_0c_0$</td>
            <td style="text-align: center;">$f_0c_1$</td>
            <td style="text-align: center;">$f_0c_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$f_1c_0 *$</td>
            <td style="text-align: center;">$f_1c_0$</td>
            <td style="text-align: center;">$f_1c_1$</td>
            <td style="text-align: center;">$f_1c_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$f_1c_1$</td>
            <td style="text-align: center;">$f_1c_0$</td>
            <td style="text-align: center;">$f_1c_1$</td>
            <td style="text-align: center;">$f_1c_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$f_1c_2 *$</td>
            <td style="text-align: center;">$f_1c_0$</td>
            <td style="text-align: center;">$f_1c_1$</td>
            <td style="text-align: center;">$f_1c_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$f_2c_0 *$</td>
            <td style="text-align: center;">$f_2c_0$</td>
            <td style="text-align: center;">$f_2c_1$</td>
            <td style="text-align: center;">$f_2c_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$f_2c_1 *$</td>
            <td style="text-align: center;">$f_2c_0$</td>
            <td style="text-align: center;">$f_2c_1$</td>
            <td style="text-align: center;">$f_2c_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$f_2c_2$</td>
            <td style="text-align: center;">$f_2c_0$</td>
            <td style="text-align: center;">$f_2c_1$</td>
            <td style="text-align: center;">$f_2c_2$</td>
        </tr>
      </tbody>
     </table>
     </div>
     </figure>

- **121.** Las palabras de $\Sigma_1$ con longitud *3n* para algún
     $n \in \mathbb{N}$, tales que si se dividen en *n*-bloques de
     longitud *3*, cada uno de éstos tiene al menos un *0*. Por ejemplo,
     *000 011 110 101* es una palabra válida, mienstras que *001 101 111
     010* no lo es, pues el tercer bloque no tienen ningún *0*.

     <figure data-latex-placement="H">
     <div class="minipage">
     <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_121.png" style="height:4cm" />
     </div>
     <div class="minipage">
     <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
            <th style="text-align: center;">$2$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0 *$</td>
            <td style="text-align: center;">$c_{0_1}$</td>
            <td style="text-align: center;">$s_{0_1}$</td>
            <td style="text-align: center;">$s_{0_1}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$c_{0_1}$</td>
            <td style="text-align: center;">$c_{0_2}$</td>
            <td style="text-align: center;">$c_{0_2}$</td>
            <td style="text-align: center;">$c_{0_2}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$c_{0_2}$</td>
            <td style="text-align: center;">$q_0$</td>
            <td style="text-align: center;">$q_0$</td>
            <td style="text-align: center;">$q_0$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$s_{0_1}$</td>
            <td style="text-align: center;">$c_{0_2}$</td>
            <td style="text-align: center;">$s_{0_2}$</td>
            <td style="text-align: center;">$s_{0_2}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$s_{0_2}$</td>
            <td style="text-align: center;">$q_0$</td>
            <td style="text-align: center;">$T$</td>
            <td style="text-align: center;">$T$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$T$</td>
            <td style="text-align: center;">$T$</td>
            <td style="text-align: center;">$T$</td>
            <td style="text-align: center;">$T$</td>
        </tr>
      </tbody>
     </table>
     </div>
     </figure>

- **122.** Las palabras de $\Sigma_1$ tales que cualquier cadena de tres
     símbolos consecutivos debe tener un *0*. Nota que la cadena
     *001110* sí está en el lenguaje del problema anterior, pero no en
     este, mientras que *00101* está en el lenguaje de este problema y
     no en el del anterior.

     <figure data-latex-placement="H">
     <div class="minipage">
     <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_122.png" style="height:4cm" />
     </div>
     <div class="minipage">
     <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
            <th style="text-align: center;">$2$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0$</td>
            <td style="text-align: center;">$q_0$</td>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_1$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_0$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2 *$</td>
            <td style="text-align: center;">$q_0$</td>
            <td style="text-align: center;">$T$</td>
            <td style="text-align: center;">$T$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$T$</td>
            <td style="text-align: center;">$T$</td>
            <td style="text-align: center;">$T$</td>
            <td style="text-align: center;">$T$</td>
        </tr>
      </tbody>
     </table>
     </div>
     </figure>

- **123.** Las palabras de $\Sigma_3$ de la forma $\omega x \omega$ donde
     $\omega \in \Sigma_3^2$ y $x \in \Sigma_3^*$.

     <figure data-latex-placement="H">
     <div class="minipage">
     <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_123.png" style="height:4cm" />
     </div>
     <div class="minipage">
     <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$a$</th>
            <th style="text-align: center;">$b$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0$</td>
            <td style="text-align: center;">$q_a$</td>
            <td style="text-align: center;">$q_b$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_a$</td>
            <td style="text-align: center;">$q_{aa}$</td>
            <td style="text-align: center;">$q_{ab}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_b$</td>
            <td style="text-align: center;">$q_{ba}$</td>
            <td style="text-align: center;">$q_{bb}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{aa}$</td>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_{aa}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{ab}$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_{ab}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{ba}$</td>
            <td style="text-align: center;">$q_{ba}$</td>
            <td style="text-align: center;">$q_3$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{bb}$</td>
            <td style="text-align: center;">$q_{bb}$</td>
            <td style="text-align: center;">$q_4$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_{faa}$</td>
            <td style="text-align: center;">$q_{aa}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_{fab}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3$</td>
            <td style="text-align: center;">$q_{fba}$</td>
            <td style="text-align: center;">$q_3$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_4$</td>
            <td style="text-align: center;">$q_{bb}$</td>
            <td style="text-align: center;">$q_{fbb}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{faa} *$</td>
            <td style="text-align: center;">$q_{faa}$</td>
            <td style="text-align: center;">$q_{aa}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{fab} *$</td>
            <td style="text-align: center;">$q_{ab}$</td>
            <td style="text-align: center;">$q_{ab}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{fba} *$</td>
            <td style="text-align: center;">$q_{ba}$</td>
            <td style="text-align: center;">$q_{ba}$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_{fbb} *$</td>
            <td style="text-align: center;">$q_{bb}$</td>
            <td style="text-align: center;">$q_{fbb}$</td>
        </tr>
      </tbody>
     </table>
     </div>
     </figure>

- **124.** En el siguiente diagrama, se muestra un mecanismo con palancas. Se
     suelta una cadena de canicas ordenadas en las entradas 0 y 1,
     formado una palabra del alfabeto $\Sigma = \left\\{0,1\right\\}$. De
     esta forma, la palabra $0010$ significa que dos canicas caen por el
     conducto 0, luego se suelta una en 1, terminando con una cuarta
     en 0. En el juego se encuntran tres palancas. Si se encuentra en la
     posicion (diagonal izquierda), la canica se va al lado izquierdo,
     por el contrario, si la posición es (diagonal derecha), se va al
     lado derecho. Cada vez que una canica pasa por una palanca, esta
     cambia de posición. Una palabra será aceptada si la última cnica
     sale por A y será rechazada si la última canica sale por R

     <figure data-latex-placement="H">
     <img src="/Unidad%201/Recursos/Imagenes_Lista2/ej_124.png" style="height:4cm" />
     </figure>

     **a)**  ¿De cuántas formas pueden estar colocadas las tres palancas?

  El mecanismo cuenta con **tres palancas** en total, dado que
  cada palanca tiene dos **posiciones posibles**, las palancas se
  pueden encontrar en:\
  $2^3 = 8$ formas (o estados) posibles

     **b)**  Realice un dibujo de cada uno de los estados en los que pueden
         estar colocadas e identifique cuál es el resultado de soltar
         una canica en 0 o en 1 en cada uno de los estados, así como la
         posición en la que quedarán las palancas después de cada paso.

  Recordando las posibles posiciones de las palancas:\
  (diagonal izquierda) $\rightarrow$ la canica se desvía hacia la
  **izquierda**.\
  (diagonal derecha) $\rightarrow$ la canica de desvía hacia la
  **derecha**.\
  Por comodidad, representaremos (diagonal izquierda) como *L*
  (left/izquierda), y (diagonal derecha) como *R*
  (right/derecha). En la tabla, leeremos los estados de izquierda
  a derecha y en las entradas, leeremos el tipo de salida y
  cambio de estado.

  <figure data-latex-placement="H">
    <div class="minipage">
      <img src="/Unidad%201/Recursos/Imagenes_Lista2/estados_124.png" style="height:4cm" />
    </div>
    <div class="minipage">
    <table>
      <thead>
        <tr>
            <th style="text-align: center;">Estado</th>
            <th style="text-align: center;">$Entrada 0$</th>
            <th style="text-align: center;">$Entrada 1$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$LLL$</td>
            <td style="text-align: center;">$A \rightarrow RLL$</td>
            <td style="text-align: center;">$A \rightarrow LRR$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$LLR$</td>
            <td style="text-align: center;">$A \rightarrow RLR$</td>
            <td style="text-align: center;">$R \rightarrow LLL$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$LRL$</td>
            <td style="text-align: center;">$A \rightarrow RRL$</td>
            <td style="text-align: center;">$R \rightarrow LLR$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$LRR$</td>
            <td style="text-align: center;">$A \rightarrow RRR$</td>
            <td style="text-align: center;">$R \rightarrow LRL$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$RLL$</td>
            <td style="text-align: center;">$A \rightarrow LRL$</td>
            <td style="text-align: center;">$A \rightarrow RRR$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$RLR$</td>
            <td style="text-align: center;">$A \rightarrow LRR$</td>
            <td style="text-align: center;">$R \rightarrow RLL$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$RRL$</td>
            <td style="text-align: center;">$R \rightarrow LLL$</td>
            <td style="text-align: center;">$R \rightarrow RLR$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$RRR$</td>
            <td style="text-align: center;">$R \rightarrow LLR$</td>
            <td style="text-align: center;">$R \rightarrow RRL$</td>
        </tr>
      </tbody>
     </table>
    </div>
   </figure>

     **c)**  Encuentre la tabla de transiciones de un autómata finito
         determinista que describa si una palabra es aceptada o
         rechazada.

  <figure data-latex-placement="H">
    <div class="minipage">
       <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_124.png" style="height:4.5cm" />
     </div>
     <div class="minipage">
     <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0$</td>
            <td style="text-align: center;">$RLL_A$</td>
            <td style="text-align: center;">$RRR_A$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$LLL_A *$</td>
            <td style="text-align: center;">$RLL_A$</td>
            <td style="text-align: center;">$RRR_A$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$LLL_R$</td>
            <td style="text-align: center;">$RLL_A$</td>
            <td style="text-align: center;">$RRR_A$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$LLR_A *$</td>
            <td style="text-align: center;">$RLR_A$</td>
            <td style="text-align: center;">$LLL_R$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$LLR_R$</td>
            <td style="text-align: center;">$RLR_A$</td>
            <td style="text-align: center;">$LLL_R$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$LRL_A *$</td>
            <td style="text-align: center;">$RRL_A$</td>
            <td style="text-align: center;">$LLR_R$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$LRL_R$</td>
            <td style="text-align: center;">$RRL_A$</td>
            <td style="text-align: center;">$LLR_R$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$LRR_A *$</td>
            <td style="text-align: center;">$RRR_A$</td>
            <td style="text-align: center;">$LRL_R$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$LRR_R$</td>
            <td style="text-align: center;">$RRR_A$</td>
            <td style="text-align: center;">$LRL_R$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$RLL_A *$</td>
            <td style="text-align: center;">$LRL_A$</td>
            <td style="text-align: center;">$LRR_R$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$RLL_R$</td>
            <td style="text-align: center;">$LRL_A$</td>
            <td style="text-align: center;">$LRR_R$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$RLR_A *$</td>
            <td style="text-align: center;">$LRR_A$</td>
            <td style="text-align: center;">$RLL_R$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$RLR_R$</td>
            <td style="text-align: center;">$LRR_A$</td>
            <td style="text-align: center;">$RLL_R$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$RRL_A *$</td>
            <td style="text-align: center;">$LLR_A$</td>
            <td style="text-align: center;">$RLR_R$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$RRL_R$</td>
            <td style="text-align: center;">$LLR_A$</td>
            <td style="text-align: center;">$RLR_A$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$RRR_A *$</td>
            <td style="text-align: center;">$LLL_R$</td>
            <td style="text-align: center;">$RRL_R$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$RRR_R$</td>
            <td style="text-align: center;">$LLL_R$</td>
            <td style="text-align: center;">$RRL_R$</td>
        </tr>
      </tbody>
     </table>
     </div>
   </figure>

- **125.**  Sea $A = (Q, \Sigma, \delta, A_0, F)$ un autómata finito
    determinista. ¿Cuál es el lenguaje del autómata
    $A = (Q, \Sigma, \delta, A_0, Q \setminus F )$? (Recuerde que
    $A \setminus B = \left\\{x : x \in A \text{ y } x \notin B\right\\}$)

    Recordando, de la definición de un Autómata Finito Determinista,
    que:\
    $Q \rightarrow$ Conjunto finito, cuyos elementos son los estados de
    A.\
    $F \subseteq Q \rightarrow$ Estados finales de A.

    Así mismo,
    $Q \setminus F = \left\\{x : x \in Q \text{ y } x \notin F\right\\}$,
    el cuál leemos como: Cualquier *x* tal que *x* pertenece a los
    estados de A y no pertenece a los estados finales de A.

    Por lo tanto, el lenguaje del autómata:
    $A = (Q, \Sigma, \delta, A_0, Q \setminus F )$ es el **lenguaje
    complementario**; si $A = (Q, \Sigma, \delta, A_0, F)$, podemos
    denotar el nuevo lenguaje como $A'$, mantiene la misma estructura
    que el autómata $A$, pero **intercambia los estados de aceptación
    por los de rechazo**.

- **126.**  Sea $A = (Q, \Sigma, \delta, A_0, F)$ un autómata finito
    determinista. ¿Cuál es el lenguaje del autómata si $F = \emptyset$?

    Recordando, de la definición de un Autómata Finito Determinista,
    que:\
    $F \subseteq Q \rightarrow$ Estados finales de A.

    Si $F = \emptyset$ (conjunto vacío), entonces, podemos decir que
    **NO HAY estados finales**, por lo tanto, es un **lenguaje sin
    estados de aceptación**.

    Por lo tanto: $A = (Q, \Sigma, \delta, A_0, F=\emptyset)$ es el
    **lenguaje vacío**. Es decir, rechaza absolutamente todas las
    palabras posibles sobre el alfabeto $\Sigma$.

- **127.**  Sea $A = (Q, \Sigma, \delta, q_0, F)$ un autómata finito
    determinista. ¿Cuál es el lenguaje del autómata si $F = Q$?

    Recordando, de la definición de un Autómata Finito Determinista,
    que:\
    $Q \rightarrow$ Conjunto finito, cuyos elementos son los estados de
    A.\
    $F \subseteq Q \rightarrow$ Estados finales de A.

    Si $F = Q$, entonces, podemos decir que **TODOS los estados de A son
    estados finales**, por lo tanto, es un **lenguaje sin estados de
    rechazo**.

    Por lo tanto: $A = (Q, \Sigma, \delta, A_0, F=Q)$ es el **lenguaje
    universal**, expresado como $\Sigma^*$. Es decir, absolutamente
    todas las palabras posibles sobre el alfabeto $\Sigma$ son
    aceptadas.

- **128.**  Sea *L* el lenguaje del autómata dado por el siguiente diagrama:

    <figure data-latex-placement="H">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/ej_128.png" style="height:4cm" />
    </figure>

    Encuentre un autómata finito determinista que identifique el
    lenguaje $L_2$ cuyas palabras son las palabras *L* quitándoles el
    último símbolo. Es decir, si $001001 \in L$, entonces
    $00100 \in L_2$.

    <figure data-latex-placement="H">
    <div class="minipage">
      <p><img src="/Unidad%201/Recursos/Imagenes_Lista2/ej_128_afd.png" style="height:4cm" alt="image" />
      <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow A$</td>
            <td style="text-align: center;">$B$</td>
            <td style="text-align: center;">$C$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$B$</td>
            <td style="text-align: center;">$C$</td>
            <td style="text-align: center;">$D$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$C$</td>
            <td style="text-align: center;">$D$</td>
            <td style="text-align: center;">$E$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$D$</td>
            <td style="text-align: center;">$F$</td>
            <td style="text-align: center;">$E$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$E$</td>
            <td style="text-align: center;">$E$</td>
            <td style="text-align: center;">$F$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$F *$</td>
            <td style="text-align: center;">$D$</td>
            <td style="text-align: center;">$D$</td>
        </tr>
      </tbody>
     </table></p>
    </div>
    <div class="minipage">
      <p><img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_128.png" style="height:4cm" alt="image" />
      <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow A$</td>
            <td style="text-align: center;">$B$</td>
            <td style="text-align: center;">$C$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$B$</td>
            <td style="text-align: center;">$C$</td>
            <td style="text-align: center;">$D$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$C$</td>
            <td style="text-align: center;">$D$</td>
            <td style="text-align: center;">$E$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$D *$</td>
            <td style="text-align: center;">$F$</td>
            <td style="text-align: center;">$E$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$E *$</td>
            <td style="text-align: center;">$E$</td>
            <td style="text-align: center;">$F$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$F$</td>
            <td style="text-align: center;">$D$</td>
            <td style="text-align: center;">$D$</td>
        </tr>
      </tbody>
     </table></p>
    </div>
    </figure>

- **131.**  Dibuje el AFD dado por los siguientes elementos:

    $M = (\left\\{q_1, q_2\right\\}, \left\\{0,1\right\\}, \delta, q_1,\left\\{q_2\right\\})$

    La función de transición $\delta$ está definida como sigue:

    $\delta(q_1, 0) = q_1$ y $\delta(q_2, 0) = q_1$

    $\delta(q_1, 1) = q_2$ y $\delta(q_2, 1) = q_2$

    Determine un lenguaje $L(M)$ que el AFD reconoce.

    <figure data-latex-placement="H">
    <div class="minipage">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_131.png" style="height:4cm" />
    </div>
    <div class="minipage">
    <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_1$</td>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2 *$</td>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_2$</td>
        </tr>
      </tbody>
     </table>
    $\therefore L(M)$ = Cadenas que terminan en 1.</p>
    </div>
    </figure>

- **133.**  Obtener la tabla de estados y el diagrama de transiciones (esquema
    AFD) del autómata finito $M = (Q, \Sigma, \delta, q_0, F)$, donde:

    - $Q = \left\\{q_0, q_1, q_2, q_3\right\\}$

    - $\Sigma = \left\\{a, b\right\\}$

    - $q_0$ es el estado inicial y también el estado final (F =
      $\left\\{q_0\right\\}$)

    Las transiciones están definidas de la siguiente manera:

    $\delta(q_0, a) = q_2$\
    $\delta(q_1, a) = q_3$\
    $\delta(q_2, a) = q_0$\
    $\delta(q_3, a) = q_1$\
    $\delta(q_0, b) = q_1$\
    $\delta(q_1, b) = q_0$\
    $\delta(q_2, b) = q_3$\
    $\delta(q_3, b) = q_2$

    <figure data-latex-placement="H">
    <div class="minipage">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_133.png" style="height:4cm" />
    </div>
    <div class="minipage">
    <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$a$</th>
            <th style="text-align: center;">$b$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0 *$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_1$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_3$</td>
            <td style="text-align: center;">$q_0$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_0$</td>
            <td style="text-align: center;">$q_3$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3$</td>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_2$</td>
        </tr>
      </tbody>
     </table>
    </div>
    </figure>

- **135.**  Dado $\Sigma = \left\\{a,b\right\\}$, construir un AFD que reconozca
    el lenguaje:

    $L = \left\\{b^mab^n : m,n>0\right\\}$

    <figure data-latex-placement="H">
    <div class="minipage">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_135.png" style="height:4cm" />
    </div>
    <div class="minipage">
    <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$a$</th>
            <th style="text-align: center;">$b$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_1$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_1$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_3$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3 *$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_3$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
        </tr>
      </tbody>
     </table>
    </div>
    </figure>

- **137.**  Construir un AFD que reconozca el conjunto de todas las cadenas
    sobre $\Sigma = \left\\{a, b\right\\}$ que comiencen con el prefijo
    *'ab'*.

    <figure data-latex-placement="H">
    <div class="minipage">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_137.png" style="height:4cm" />
    </div>
    <div class="minipage">
    <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$a$</th>
            <th style="text-align: center;">$b$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0$</td>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_m$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2 *$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
        </tr>
      </tbody>
     </table>
    </div>
    </figure>

- **139.**  Construya un autómata finito (FA) que acepte todas las cadenas en
    $\left\\{0,1\right\\}^*$ que tengan un número par de ceros.

    <figure data-latex-placement="H">
    <div class="minipage">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_139.png" style="height:4cm" />
    </div>
    <div class="minipage">
    <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0 *$</td>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_0$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_0$</td>
            <td style="text-align: center;">$q_1$</td>
        </tr>
      </tbody>
     </table>
    </div>
    </figure>

- **141.** Determine un autómata finito (FA), *M*, que acepte el lenguaje *L*,
    donde:

    $L = \left\\{\omega \in \left\\{0,1\right\\}^* \quad:\quad \text{ cada } 0 \text{ en } \omega \text{ tiene un } 1 \text{ inmediatamente a su derecha}\right\\}$

    <figure data-latex-placement="H">
    <div class="minipage">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_141.png" style="height:4cm" />
    </div>
    <div class="minipage">
    <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0$</td>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_0$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2 *$</td>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
        </tr>
      </tbody>
     </table>
    </div>
    </figure>

- **143.** Determine los lenguajes producidos por los autómatas finitos (FA) mostrados en las Figuras (a) y (b).

    <figure data-latex-placement="H">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/ej_143.png" style="height:4cm" />
    </figure>

    <figure data-latex-placement="H">
    <div class="minipage">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_143_a.png" style="height:4cm" />
    <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$a$</th>
            <th style="text-align: center;">$b$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0 *$</td>
            <td style="text-align: center;">$q_0$</td>
            <td style="text-align: center;">$q_0$</td>
        </tr>
      </tbody>
     </table>
    </div>
    </figure>
    
    Ya habíamos visto en un ejercicio anterior que en un autómata cuyo
    estado final es el estado inicial, es el <strong>lenguaje
    universal</strong>, por lo tanto acepta TODAS las cadenas posibles sobre
    el alfabeto $$\Sigma = \left\\{a,b\right\\} $$.
        
    <figure data-latex-placement="H">
    <div class="minipage">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_143_b.png" style="height:4cm" />
    <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$a$</th>
            <th style="text-align: center;">$b$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0$</td>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$\emptyset$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1 *$</td>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">{ $q_0 , q_1$ }</td>
        </tr>
      </tbody>
     </table>
    </div>
    </figure>
    
    El autómata no es Determinista, dado que
    $q_1$ al recibir *b*, el autómata tiene la "libertad" de tomar dos
    caminos simultáneamente. El autómata acepta el conjunto de todas las
    cadenas sobre el alfabeto
    $$\Sigma = \left\\{a, b\right\\} $$

- **145.** Encuentre un AFD que lee un número binario de derecha a izquierda e
    identifica aquellos que son múltiplos de 5.

    Cuando se lee de **derecha a izquierda**, el número se forma sumando
    cada bit ($b$) multiplicado por su posición en potencias de 2. De la
    siguiente manera:

    $V = b_0\cdot2^0 + b_1\cdot2^1 + b_2\cdot2^2 + ...$

    Si observamos las potencias de 2 módulo 5, ocurre un ciclo
    repetitivo cada 4 posiciones:

    - $2^0 = 1$ *mod 5* $= 1$

    - $2^1 = 2$ *mod 5* $= 2$

    - $2^2 = 4$ *mod 5* $= 4$

    - $2^3 = 8$ *mod 5* $= 3$

    - $2^4 = 16$ *mod 5* $= 1$\
      el ciclo se repite\...

    Para procesar la cadena correctamente, el autómata necesita llevar
    el control de dos cosas simultáneamente:

    1.  El residuo actual del número modulo 5:
        $r \in \left\\{0,1,2,3,4\right\\}$

    2.  El peso (potencia) de la posición actual del bit:
        $p \in \left\\{1,2,3,4\right\\}$

    Cuando el autómata se encuentra en un estado con residuo *r* y peso
    de posición *p*, al leer un nuevo bit *b* (0 o 1):

    - **Si b = 0:** El valor no cambia. El residuo *r* se queda igual,
      pero el peso de la posición avanza al siguiente valor:
      $(p \cdot 2)$ *mod 5*.

    - **Si b = 1:** Se le suma el valor del peso actual al residuo:
      $r_{nuevo} = (r + p)$ *mod 5* y el peso de la posición también
      avanza: $(p \cdot 2)$ *mod 5*.

    Para el AFD, nombraremos a los estados: $r_np_m$. El estado inicial
    es $r_0p_1$ y los finales todos los estados cuyo resuido sea 0:
    $r_0p_1, r_0p_2, r_0p_3, r_0p_4$.

    <figure data-latex-placement="H">
    <div class="minipage">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_145.png" style="height:4cm" />
    </div>
    <div class="minipage">
    <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow r_0p_1 *$</td>
            <td style="text-align: center;">$r_0p_2$</td>
            <td style="text-align: center;">$r_1p_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_1p_1$</td>
            <td style="text-align: center;">$r_1p_2$</td>
            <td style="text-align: center;">$r_2p_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_2p_1$</td>
            <td style="text-align: center;">$r_2p_2$</td>
            <td style="text-align: center;">$r_3p_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_3p_1$</td>
            <td style="text-align: center;">$r_3p_2$</td>
            <td style="text-align: center;">$r_4p_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_4p_1$</td>
            <td style="text-align: center;">$r_4p_2$</td>
            <td style="text-align: center;">$r_0p_2$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_0p_2 *$</td>
            <td style="text-align: center;">$r_0p_4$</td>
            <td style="text-align: center;">$r_2p_4$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_1p_2$</td>
            <td style="text-align: center;">$r_1p_4$</td>
            <td style="text-align: center;">$r_3p_4$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_2p_2$</td>
            <td style="text-align: center;">$r_2p_4$</td>
            <td style="text-align: center;">$r_4p_4$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_3p_2$</td>
            <td style="text-align: center;">$r_3p_4$</td>
            <td style="text-align: center;">$r_4p_4$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_4p_2$</td>
            <td style="text-align: center;">$r_4p_4$</td>
            <td style="text-align: center;">$r_1p_4$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_0p_3 *$</td>
            <td style="text-align: center;">$r_0p_1$</td>
            <td style="text-align: center;">$r_3p_1$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_1p_3$</td>
            <td style="text-align: center;">$r_1p_1$</td>
            <td style="text-align: center;">$r_4p_1$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_2p_3$</td>
            <td style="text-align: center;">$r_2p_1$</td>
            <td style="text-align: center;">$r_0p_1$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_3p_3$</td>
            <td style="text-align: center;">$r_3p_1$</td>
            <td style="text-align: center;">$r_1p_1$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_4p_3$</td>
            <td style="text-align: center;">$r_4p_1$</td>
            <td style="text-align: center;">$r_2p_1$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_0p_4 *$</td>
            <td style="text-align: center;">$r_0p_3$</td>
            <td style="text-align: center;">$r_4p_3$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_1p_4$</td>
            <td style="text-align: center;">$r_1p_3$</td>
            <td style="text-align: center;">$r_0p_3$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_2p_4$</td>
            <td style="text-align: center;">$r_2p_3$</td>
            <td style="text-align: center;">$r_1p_3$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_3p_4$</td>
            <td style="text-align: center;">$r_3p_3$</td>
            <td style="text-align: center;">$r_2p_3$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$r_4p_4$</td>
            <td style="text-align: center;">$r_4p_3$</td>
            <td style="text-align: center;">$r_3p_3$</td>
        </tr>
      </tbody>
     </table>
    </div>
    </figure>

13. Diseñe un AFD que lee un número binario de izquierda a derecha y lo
    acepta si es un múltiplo de 6.

    Cuando leemos un número binario de **izquierda a derecha**, podemos
    guardar el residuo módulo 6. Si estamos en un estado que representa
    el resuido *r* y leemos un bit *b*: $r_{nuevo} = (2r + b)$ *mod 6*
    El estado inicial es $q_0$, y solamente $q_0$ es final, porque
    queremos numeros divisibles entre 6.

    <figure data-latex-placement="H">
    <div class="minipage">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_147.png" style="height:4cm" />
    </div>
    <div class="minipage">
    <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0 *$</td>
            <td style="text-align: center;">$q_0$</td>
            <td style="text-align: center;">$q_1$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_3$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_4$</td>
            <td style="text-align: center;">$q_5$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_3$</td>
            <td style="text-align: center;">$q_0$</td>
            <td style="text-align: center;">$q_1$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_4$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_3$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_5$</td>
            <td style="text-align: center;">$q_4$</td>
            <td style="text-align: center;">$q_5$</td>
        </tr>
      </tbody>
     </table>
    </div>
    </figure>

- **148.** Diseñar un autómata finito (FA) que modele el progreso de un alumno
    de la *ESCOM* a lo largo de una Unidad de Aprendizaje, en este caso,
    del curso de *Teoría de la Computación*. El autómata debe
    representar las distintas decisiones que se toman en cada
    evaluación, como si el alumno aprueba, aplaza o no se presenta a un
    examen, y controlar que no se presenten más de dos convocatorias en
    un año. El autómata concluirá cuando el alumno apruebe el curso.

    El alfabeto de entrada estará formado por los siguientes elementos:

    - P : El alumno se presenta al examen

    - N : El alumno no se presenta al examen

    - A : El alumno aprueba el examen

    - S : El alumno aplaza el examen.

    El alumno comenzará en un estado inicial y tomará decisiones sobre
    si presentarse en las distintas convocatorias de febrero, septiembre
    y diciembre, hasta que apruebe el curso. Se deben evitar más de dos
    convocatorias en un año y reiniciar el ciclo en caso de no aprobar
    en las dos primeras.

    <figure data-latex-placement="H">
    <div class="minipage">
    <img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_148.png" style="height:4cm" />
    </div>
    <div class="minipage">
    <table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$P$</th>
            <th style="text-align: center;">$N$</th>
            <th style="text-align: center;">$A$</th>
            <th style="text-align: center;">$S$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow q_0$</td>
            <td style="text-align: center;">$c_1$</td>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$c_1$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_f$</td>
            <td style="text-align: center;">$q_1$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_1$</td>
            <td style="text-align: center;">$c_2$</td>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$c_2$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_f$</td>
            <td style="text-align: center;">$q_0$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_2$</td>
            <td style="text-align: center;">$c_3$</td>
            <td style="text-align: center;">$q_0$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$c_3$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_f$</td>
            <td style="text-align: center;">$q_0$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_f *$</td>
            <td style="text-align: center;">$q_f$</td>
            <td style="text-align: center;">$q_f$</td>
            <td style="text-align: center;">$q_f$</td>
            <td style="text-align: center;">$q_f$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
            <td style="text-align: center;">$q_m$</td>
        </tr>
      </tbody>
     </table>
    </div>
    </figure>

En los problemas 149 y 150, considere el autómata
$A = (Q, \Sigma, \delta, A_0, F)$ definidos en cada tabla. Encuentre
$Q$, $\Sigma$, $A_0$ y $F$, haga el diagrama de transiciones del
autómata y halle los valores que se piden en cada inciso.

- **149.**

**a)** $\delta(B,0)$

**b)**  $\delta(C,1)$

**c)**  $\hat{\delta}(A,1101)$

**d)**  $\hat{\delta}(A,01001)$

<figure data-latex-placement="H">
<div class="minipage">
<table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow A$</td>
            <td style="text-align: center;">$B$</td>
            <td style="text-align: center;">$C$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$B$</td>
            <td style="text-align: center;">$A$</td>
            <td style="text-align: center;">$C$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$C *$</td>
            <td style="text-align: center;">$C$</td>
            <td style="text-align: center;">$A$</td>
        </tr>
      </tbody>
     </table>
</div>

- $Q = \left\\{A,B,C\right\\}$
- $\Sigma = \left\\{0,1\right\\}$
- $A_0 = A$
- $F = C$

<div class="minipage">
<img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_149.png" style="height:4cm" />
</div>
</figure>

**a)**  $\delta(B,0)$

De la tabla de transiciones proporcionada: $\delta(B,0) = A$

**b)**  $\delta(C,1) = A$

De la tabla de transiciones proporcionada: $\delta(C,1) = A$

**c)**  $\hat{\delta}(A,1101)$

Veamos que: $\hat{\delta}(A,\lambda) = A$,\
entonces: $\hat{\delta}(A, 1) = \delta(\hat{\delta}(A, \lambda), 1) = C$\
Así:

$\hat{\delta}(A, 11) = \delta(\hat{\delta}(A, 1), 1) = \delta(C, 1) = A$\
$\hat{\delta}(A, 110) = \delta(\hat{\delta}(A, 11), 0) = \delta(A, 0) = B$\
$\hat{\delta}(A, 1101) = \delta(\hat{\delta}(A, 110), 1) = \delta(B, 1) = C$

$\therefore \hat{\delta}(A, 1101) = C$

**d)**  $\hat{\delta}(A,01001)$

Veamos que: $\hat{\delta}(A,\lambda) = A$,\
entonces: $\hat{\delta}(A, 0) = \delta(\hat{\delta}(A, \lambda), 0) = B$\
Así:

$\hat{\delta}(A, 01) = \delta(\hat{\delta}(A, 0), 1) = \delta(B, 1) = C$\
$\hat{\delta}(A, 010) = \delta(\hat{\delta}(A, 01), 0) = \delta(C, 0) = C$\
$\hat{\delta}(A, 0100) = \delta(\hat{\delta}(A, 010), 0) = \delta(C, 0) = C$\
$\hat{\delta}(A, 01001) = \delta(\hat{\delta}(A, 0100), 1) = \delta(C, 1) = A$

$\therefore \hat{\delta}(A, 1101) = A$

- **150.**

**a)**  $\hat{\delta}(B,10a11)$

**b)**  $\hat{\delta}(B,aa1100)$

**c)**  $\hat{\delta}(A,a01a01)$

**d)**  $\hat{\delta}(C,a11a00)$

<figure data-latex-placement="H">
<div class="minipage">
<table>
      <thead>
        <tr>
            <th style="text-align: center;"></th>
            <th style="text-align: center;">$0$</th>
            <th style="text-align: center;">$1$</th>
            <th style="text-align: center;">$a$</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td style="text-align: center;">$\rightarrow A$</td>
            <td style="text-align: center;">$B$</td>
            <td style="text-align: center;">$C$</td>
            <td style="text-align: center;">$D$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$B *$</td>
            <td style="text-align: center;">$B$</td>
            <td style="text-align: center;">$C$</td>
            <td style="text-align: center;">$C$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$C *$</td>
            <td style="text-align: center;">$A$</td>
            <td style="text-align: center;">$A$</td>
            <td style="text-align: center;">$D$</td>
        </tr>
        <tr>
            <td style="text-align: center;">$D *$</td>
            <td style="text-align: center;">$B$</td>
            <td style="text-align: center;">$B$</td>
            <td style="text-align: center;">$B$</td>
        </tr>
      </tbody>
     </table>
</div>

- $Q = \left\\{A,B,C,D\right\\}$
- $\Sigma = \left\\{0,1,a\right\\}$
- $A_0 = A$
- $F = \left\\{B,C,D\right\\}$

<div class="minipage">
<img src="/Unidad%201/Recursos/Imagenes_Lista2/sol_149.png" style="height:4cm" />
</div>
</figure>

**a)**  $\hat{\delta}(B,10a11)$

Veamos que: $\hat{\delta}(B,\lambda) = B$,\
entonces: $\hat{\delta}(B, 1) = \delta(\hat{\delta}(B, \lambda), 1) = C$\
Así:

$\hat{\delta}(B, 10) = \delta(\hat{\delta}(B, 1), 0) = \delta(C, 0) = A$\
$\hat{\delta}(B, 10a) = \delta(\hat{\delta}(B, 10), a) = \delta(A, a) = D$\
$\hat{\delta}(B, 10a1) = \delta(\hat{\delta}(B, 10a), 1) = \delta(D, 1) = B$\
$\hat{\delta}(B, 10a11) = \delta(\hat{\delta}(B, 10a1), 1) = \delta(B, 1) = C$

$\therefore \hat{\delta}(B, 10a11) = C$

**b)**  $\hat{\delta}(B,aa1100)$

Veamos que: $\hat{\delta}(B,\lambda) = B$,\
entonces: $\hat{\delta}(B, a) = \delta(\hat{\delta}(B, \lambda), a) = C$\
Así:

$\hat{\delta}(B, aa) = \delta(\hat{\delta}(B, a), a) = \delta(C, a) = D$\
$\hat{\delta}(B, aa1) = \delta(\hat{\delta}(B, aa), 1) = \delta(D, 1) = B$\
$\hat{\delta}(B, aa11) = \delta(\hat{\delta}(B, aa1), 1) = \delta(B, 1) = C$\
$\hat{\delta}(B, aa110) = \delta(\hat{\delta}(B, aa11), 0) = \delta(C, 0) = A$\
$\hat{\delta}(B, aa1100) = \delta(\hat{\delta}(B, aa110), 0) = \delta(A, 0) = B$

$\therefore \hat{\delta}(B, aa1100) = B$

**c)**  $\hat{\delta}(A,a01a01)$

Veamos que: $\hat{\delta}(A,\lambda) = A$,\
entonces: $\hat{\delta}(A, a) = \delta(\hat{\delta}(A, \lambda), a) = D$\
Así:

$\hat{\delta}(A, a0) = \delta(\hat{\delta}(A, a), 0) = \delta(D, 0) = B$\
$\hat{\delta}(A, a01) = \delta(\hat{\delta}(A, a0), 1) = \delta(B, 1) = C$\
$\hat{\delta}(A, a01a) = \delta(\hat{\delta}(A, a01), a) = \delta(C, a) = D$\
$\hat{\delta}(A, a01a0) = \delta(\hat{\delta}(A, a01a), 0) = \delta(D, 0) = B$\
$\hat{\delta}(A, a01a01) = \delta(\hat{\delta}(A, a01a0), 1) = \delta(B, 1) = C$

$\therefore \hat{\delta}(A, a01a01) = C$

**d)**  $\hat{\delta}(C,a11a00)$

Veamos que: $\hat{\delta}(C,\lambda) = C$,\
entonces: $\hat{\delta}(C, a) = \delta(\hat{\delta}(C, \lambda), a) = D$\
Así:

$\hat{\delta}(C, a1) = \delta(\hat{\delta}(C, a), 1) = \delta(D, 1) = B$\
$\hat{\delta}(C, a11) = \delta(\hat{\delta}(C, a1), 1) = \delta(B, 1) = C$\
$\hat{\delta}(C, a11a) = \delta(\hat{\delta}(C, a11), a) = \delta(C, a) = D$\
$\hat{\delta}(C, a11a0) = \delta(\hat{\delta}(C, a11a), 0) = \delta(D, 0) = B$\
$\hat{\delta}(C, a11a00) = \delta(\hat{\delta}(C, a11a0), 0) = \delta(B, 0) = B$

$\therefore \hat{\delta}(C, a11a00) = B$
