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

     **a)**  ¿De cuántas formas pueden estar colocadas las tres palancas?\

  El mecanismo cuenta con **tres palancas** en total, dado que
  cada palanca tiene dos **posiciones posibles**, las palancas se
  pueden encontrar en:\
  $2^3 = 8$ formas (o estados) posibles

     **b)**  Realice un dibujo de cada uno de los estados en los que pueden
         estar colocadas e identifique cuál es el resultado de soltar
         una canica en 0 o en 1 en cada uno de los estados, así como la
         posición en la que quedarán las palancas después de cada paso.\

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
