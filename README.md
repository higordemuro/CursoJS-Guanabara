# Curso em Vídeo - JavaScript:

Arquivos de exercícios realizados no Curso de JavaScript, disponibilizado pelo canal ``Curso em Vídeo``.

- **Site:** https://cursoemvideo.com
- **Instagram:** https://www.instagram.com/cursoemvideo
- **Twitter:** https://twitter.com/guanabara
- **Facebook:** https://www.facebook.com/CursosEmVideo/
- **YouTube:** https://www.youtube.com/cursoemvideo


### 🖥 **Tecnologias:**
- ``JavaScript``
-  ``CSS3``
-   ``HTML5``

## ⏰ Exercício 01: ``Relógio com Mudança de Cenário``

Este código HTML e Javascript implementa um relógio digital simples que muda o fundo da página e a imagem exibida de acordo com a hora do dia.

**Estrutura do código:**

* O código HTML define a estrutura da página, incluindo cabeçalho (`header`), seção principal (`section`), rodapé (`footer`) e elementos de texto (`div`).
* O CSS (em um arquivo separado - `estilo.css`) define o estilo visual da página, como cores, fontes e posicionamento.
* O Javascript (em um arquivo separado - `script.js`) contém a lógica principal do relógio.

**Funcionalidade do código:**

* Ao carregar a página (`onload` function), o script acessa a hora atual usando a função `Date()`.
* A hora extraída é usada para definir uma mensagem exibida na seção (`div` com id "msg").
* O script verifica a hora do dia usando um bloco `if` para:
    * Manhã (00:00 - 11:59): altera o fundo da página para laranja claro, exibe a mensagem "Agora são X horas." e carrega a imagem "fotomanha.png".
    * Tarde (12:00 - 17:59): altera o fundo da página para azul claro, exibe a mensagem "Agora são X horas." e carrega a imagem "fototarde.png".
    * Noite (18:00 - 23:59): altera o fundo da página para azul escuro, exibe a mensagem "Agora são X horas." e carrega a imagem "fotonoite.png".
* Imagens separadas (`fotomanha.png`, `fototarde.png`, `fotonoite.png`) representam diferentes cenários para cada período do dia (manhã, tarde e noite).

![hora](https://github.com/higordrx/CursoJS-Guanabara/assets/168053348/1313105f-6214-474c-b26a-42478ee62fa7)

## 🎂 Exercício 02: ``Verificador de Idade com Imagens Dinâmicas``
Este código HTML e Javascript implementa um verificador de idade que apresenta uma mensagem personalizada, a idade do usuário e uma imagem ilustrativa de acordo com o sexo e faixa etária.

**Estrutura do código:**

* O HTML define a estrutura da página, incluindo cabeçalho (`header`), seção principal (`section`), rodapé (`footer`) e elementos de formulário para entrada de dados.
* O CSS (em um arquivo separado - `estilo.css`) define o estilo visual da página, como cores, fontes e posicionamento.
* O Javascript (em um arquivo separado - `script.js`) contém a lógica principal do verificador de idade.

**Funcionalidade do código:**

* O usuário informa o ano de nascimento e o sexo (`masculino` ou `feminino`) através de campos de input.
* Ao clicar no botão "Verificar", a função `verificar()` é executada:
    * Valida se o ano de nascimento foi preenchido e se é um valor válido.
    * Se o ano de nascimento for inválido, exibe um alerta de erro.
    * Se o ano de nascimento for válido:
        * Calcula a idade do usuário subtraindo o ano de nascimento do ano atual.
        * Determina o gênero do usuário com base na seleção do radio button.
        * Cria uma imagem dinâmica (`img`) com base no gênero e faixa etária:
            * **Bebê:** `BebeHomem.png` ou `BebeMulher.png` (0 a 9 anos)
            * **Jovem:** `JovemHomem.png` ou `JovemMulher.png` (10 a 20 anos)
            * **Adulto:** `AdultoHomem.png` ou `AdultaMulher.png` (21 a 49 anos)
            * **Idoso:** `IdosoHomem.png` ou `IdosaMulher.png` (50 anos ou mais)
        * Exibe uma mensagem na seção `div#res` com a idade e o gênero do usuário.
        * Adiciona a imagem dinâmica à seção `div#res`.
* As imagens (`BebeHomem.png`, `BebeMulher.png`, etc.) devem estar na mesma pasta que o arquivo HTML para serem carregadas corretamente.


![image](https://github.com/higordrx/CursoJS-Guanabara/assets/168053348/1f88c094-4f13-420f-a355-90b239f81116)

## 2️⃣ Exercício 03: ``Super Contador``

Este código HTML e Javascript implementa um "Super Contador" que permite ao usuário definir valores de início, fim e passo para uma contagem. 

**Estrutura do código:**

* O HTML define a estrutura da página, incluindo cabeçalho (`header`), seção principal (`section`), rodapé (`footer`) e elementos de formulário para entrada de dados.
* O CSS (em um arquivo separado - `estilo.css`) define o estilo visual da página, como cores, fontes e posicionamento.
* O Javascript (em um arquivo separado - `script.js`) contém a lógica principal do contador.

**Funcionalidade do código:**

* O usuário informa o valor inicial (`Início`), o valor final (`Fim`) e o passo (`Passo`) para a contagem através de campos de input do tipo number.
* Ao clicar no botão "Contar", a função `contar()` é executada:
    * Valida se todos os campos de input estão preenchidos.
    * Se algum campo estiver vazio, exibe a mensagem "Impossível contar!" na seção `div#res`.
    * Se todos os campos estiverem preenchidos:
        * Converte os valores informados nos campos de input para números (`Number()`).
        * Verifica se o passo (`passo`) é menor ou igual a zero.
            * Se for menor ou igual a zero, exibe um alerta informando que o passo é inválido e altera o valor do passo para 1.
        * Verifica se a contagem deve ser crescente (`inicio < fim`) ou decrescente (`inicio > fim`).
        * Realiza a contagem utilizando um loop `for`:
            * Para contagem crescente, o loop itera do valor inicial (`i`) até o valor final (`f`), incrementando de acordo com o passo (`p`).
            * Para contagem decrescente, o loop itera do valor inicial (`i`) até o valor final (`f`), decrementando de acordo com o passo (`p`).
        * Exibe o resultado da contagem na seção `div#res`, formatando a saída com um emoji de dedo indicador apontando para a direita (`\u{1F449}`) entre cada número e um emoji de bandeira (`\u{1F3C1}`) ao final.*
      
![image](https://github.com/higordrx/CursoJS-Guanabara/assets/168053348/0e646837-21dc-440d-82bf-028638f51ff0)

## 🧠 Exercício 04: ``Gerador de Tabuada``

Este código HTML e Javascript implementa um gerador de tabuada.

**Estrutura do código:**

* O HTML define a estrutura da página, incluindo cabeçalho (`header`), seção principal (`section`), rodapé (`footer`) e elementos de formulário para entrada de dados.
* O CSS (em um arquivo separado - `estilo.css`) define o estilo visual da página, como cores, fontes e posicionamento.
* O Javascript (em um arquivo separado - `script.js`) contém a lógica principal do gerador de tabuada.

**Funcionalidade do código:**

* O usuário informa um número inteiro através do campo de input do tipo number.
* Ao clicar no botão "Gerar Tabuada", a função `tabuada()` é executada:
    * Valida se o campo de input está preenchido.
    * Se o campo estiver vazio, exibe um alerta informando que o usuário deve digitar um número.
    * Se o campo estiver preenchido:
        * Converte o valor informado no campo de input para um número (`Number()`).
        * Limpa o conteúdo do elemento `select` com id `"seltab"` (onde a tabuada será exibida).
        * Utiliza um loop `while` para iterar de 1 a 10 (representando os multiplicadores da tabuada):
            * Cria um elemento `option` (uma opção para o elemento `select`).
            * Define o texto da opção como a multiplicação do número informado pelo usuário (`n`) pelo iterador (`c`) do loop, formatando a saída (`n x c = n*c`).
            * Define o valor da opção como `tab${c}` (valor arbitrário para referência interna).
            * Adiciona a opção criada como filha do elemento `select` (`tab.appendChild(item)`).
        * Ao final do loop, o elemento `select` conterá todas as operações da tabuada do número informado pelo usuário.

![image](https://github.com/higordrx/CursoJS-Guanabara/assets/168053348/f6525343-b203-438d-9d7d-8358bfbecba8)

## 🔎 Exercício 04: ``Analisador de Números``

Este código JavaScript cria uma página web interativa que analisa números informados pelo usuário. A página é dividida em sections:

* **Cabeçalho:** Exibe o título "Analisador de Números".
* **Seção principal:** 
    * Possui uma caixa de texto para o usuário digitar um número entre 1 e 100.
    * Um botão "Adicionar" que chama a função `adicionar` para processar o número digitado.
    * Uma caixa de seleção (select) para exibir os números adicionados.
    * Um botão "Finalizar" que chama a função `finalizar` para analisar os números adicionados.
    * Uma área de resultados (div) onde serão exibidas as estatísticas dos números.
* **Rodapé:** Exibe o crédito "Curso em Vídeo".

**Funcionamento do código**

1. **Variáveis:**
    * O código seleciona elementos da página usando `document.querySelector` e armazena em variáveis:
        * `num`: caixa de texto para digitar o número.
        * `lista`: caixa de seleção para exibir os números adicionados.
        * `res`: área de resultados para exibir as estatísticas.
        * `valores`: array para armazenar os números digitados pelo usuário.
2. **Funções:**
    * `isNumero(n)`: verifica se o valor `n` é um número válido (entre 1 e 100).
    * `inLista(n, l)`: verifica se o valor `n` já existe na lista `l` (array de valores).
    * `adicionar()`: é chamada ao clicar no botão "Adicionar".
        * Verifica se o número digitado é válido e não está na lista usando `isNumero` e `inLista`.
        * Se válido, adiciona o número no array `valores`.
        * Cria um novo elemento `option` para a caixa de seleção (`lista`) exibindo o número adicionado.
        * Limpa a área de resultados (`res`).
        * Caso o número seja inválido ou já esteja na lista, exibe um alerta.
        * Limpa a caixa de texto (`num`) e coloca o foco nela para nova digitação.
    * `finalizar()`: é chamada ao clicar no botão "Finalizar".
        * Verifica se algum número foi adicionado (`valores.length`).
        * Se houverem números na lista, calcula:
            * Quantidade total de números (`tot`).
            * Maior valor (`maior`).
            * Menor valor (`menor`).
            * Soma de todos os valores (`soma`).
            * Média dos valores (`media`).
        * Exibe o resultado na área de resultados (`res`), mostrando a quantidade de números, maior, menor, soma e média.
        * Se não houver nenhum número adicionado, exibe um alerta pedindo para adicionar valores antes de finalizar.

![image](https://github.com/higordrx/CursoJS-Guanabara/assets/168053348/11be2497-ec1b-4652-86cd-7eb0cc3a47a0)
