# Sistema de Gerenciamento de Notas Escolares: 

Ordenação: As notas dos alunos podem ser ordenadas por valor (crescente/decrescente), nome do aluno ou disciplina. Isso facilita a visualização de rankings, a identificação de alunos com melhor ou menor desempenho e a análise de tendências gerais.
Busca: Professores e administradores precisam buscar rapidamente as notas de um aluno específico, alunos dentro de uma determinada faixa de notas ou notas por disciplina.
Sinergia: Após buscar um grupo de alunos (ex: por turma), as notas podem ser ordenadas para análise. A ordenação prévia de listas de alunos também pode acelerar buscas específicas (ex: usando busca binária se a lista estiver ordenada por nome).

Obs: PARA USAR O MATCH É RECOMENDADO USAR VERSÕES A PARTIR DO PY 3.10

O código foi testado no site: https://www.programiz.com/python-programming/online-compiler/


Para deixar mais claro como que funciona cada tipo de ordenação, será exemplificado abaixo, porém, no projeto é utilizado como se fosse "usar uma bazuca em uma formiga", meio desnecessário, pois o resultado não altera, mas sim o tempo de resposta neste caso em expecífico. Foi utilizados todos os métodos apenas para fins didádicos.


# Quick Sort
- Escolhemos um pivô (por exemplo, 4).
- Dividimos a lista em elementos menores ([3, 2]) e maiores ([5, 8]) que o pivô.
- Aplicamos recursivamente o mesmo processo até ordenar todos os elementos.
Resultado final: [2, 3, 4, 5, 8].
# Merge Sort
- Dividimos a lista até ter sublistas unitárias ([5], [3], [8], [4], [2]).
- Começamos a combinar e ordenar progressivamente ([3, 5], [2, 4, 8]).
- Mesclamos as sublistas ordenadas até formar a lista final.
Resultado final: [2, 3, 4, 5, 8].
# Shell Sort
- Dividimos a lista em grupos distantes para ordenação parcial ([5, 2], [3, 8], [4]).
- Ordenamos cada grupo ([2, 5], [3, 8], [4]).
- Reduzimos a distância entre os elementos e refinamos a ordenação até a lista final.
Resultado final: [2, 3, 4, 5, 8].
# Selection Sort
- Encontramos o menor número (2) e o movemos para a primeira posição.
- Repetimos esse processo para os próximos menores (3, 4, 5, 8).
Resultado final: [2, 3, 4, 5, 8].
# Bubble Sort
- Comparamos pares e trocamos quando necessário ([3, 5, 4, 2, 8]).
- Continuamos repetindo as trocas até a lista ficar ordenada.
Resultado final: [2, 3, 4, 5, 8].
Insertion Sort
- Pegamos cada número e o inserimos na posição correta em uma lista parcialmente ordenada.
- Exemplo de inserção progressiva: [3, 5, 8, 4, 2] → [3, 4, 5, 8, 2] → [2, 3, 4, 5, 8].
Resultado final: [2, 3, 4, 5, 8].
