# Analisador-Léxico
Projeto desenvolvido para a disciplina de Compiladores do curso de Ciência da Computação no 6° período.
Este é um compilador léxico simples, baseado na linguagem C e construído utilizando Python.

🚀 Como funciona?
O analisador percorre o código-fonte caractere por caractere usando expressões regulares e separa o conteúdo em **tokens**. Ele reconhece os seguintes tipos:
- Comentários (`//` ou `#`)
- Literais (`"texto"` ou `'caractere'`)
- Números inteiros e decimais
- Palavras reservadas (como `int`, `while`, `return`, etc.)
- Identificadores (nomes de variáveis, funções, etc.)
- Operadores (`+`, `-`, `==`, etc.)
- Separadores (`;`, `,`, `{}`, etc.)
- Espaços e quebras de linha (ignorados ou usados para contagem de linha)
- Caractere inválido (gera erro)
---

🛠️ Como usar

1. Certifique-se de ter Python 3 instalado.
2. Crie um arquivo com o código-fonte que você quer analisar (por exemplo: `codigo.txt`).
3. Execute o script: python analisador.py
---

Exemplo de entrada:
int a = 10;
int c = a + 5; // soma a+5
printf("c = %d", d);

Saída:
('Palavra_Reservada', 'int')
('Identificador', 'a')
('Operador', '=')
('Numero', 10)
('Separador', ';')
('Palavra_Reservada', 'int')
('Identificador', 'c')
('Operador', '=')
('Identificador', 'a')
('Operador', '+')
('Numero', 5)
('Separador', ';')
('Comentario', '// soma a+5')
('Palavra_Reservada', 'printf')
('Separador', '(')
('Literal', '"c = %d"')
('Separador', ',')
('Identificador', 'd')
('Separador', ')')
('Separador', ';')

---
