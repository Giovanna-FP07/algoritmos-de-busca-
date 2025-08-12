DESCRIÇÃO BREVE DAS DIFERENÇAS ENTRE LINEAR E BINÁRIA.
Buscar é localizar rapidamente um item em um conjunto de dados. 
Em vetores desordenados, a abordagem direta é busca linear (verifica elemento a elemento). 
Quando os dados estão ordenados, podemos usar busca binária, que “corta” o espaço de busca pela metade a cada passo.

Na prática:
-> Em um vetor pequeno, a busca linear é simples e suficiente.
-> Em coleções grandes e ordenadas, a busca binária é muito mais eficiente.
Conceitos-chave:
-> Busca Linear: percorre do início ao fim. Complexidade: O(n).
-> Busca Binária: requer dados ordenados; compara no meio e descarta metade. Complexidade: O(log n).

COMO COMPILAR E EXECUTAR CADA ARQUIVO.
1) Busca Linear (inteiros)
Compilar e executar:
gcc busca_linear.c -o busca_linear.exe
./busca_linear.exe

2) Busca Binária (inteiros, vetor ordenado)
Compilar e executar:
gcc busca_binaria.c -o busca_binaria.exe
./busca_binaria.exe

3) Busca de CPF (strings) – linear e binária
Compilar e executar:
gcc cpf_busca.c -o cpf_busca.exe
./cpf_busca.exe

OBSERVAÇÕES SOBRE QUANDO USAR CADA TÉCNICA.
1) Busca Linear (inteiros ou strings)
	Quando usar:
	•	Quando o vetor não está ordenado.
	•	Quando o vetor é pequeno e não compensa ordenar para buscar.
	•	Quando a busca será feita poucas vezes (ordenar toda hora é desperdício).
	•	Quando você precisa verificar todos os elementos de qualquer forma (ex.: procurar todos que batem com um critério).


2) Busca Binária (inteiros ou strings)
	Quando usar:
	•	Quando o vetor já está ordenado ou você pode ordenar antes de fazer muitas buscas.
	•	Ideal quando há muitas buscas repetidas sobre o mesmo conjunto de dados.
	•	Quando o tamanho do vetor é grande e você quer performance.


3) Busca Linear vs. Binária para CPFs (strings)
	Busca Linear com strings:
	•	Serve para vetores de CPFs não ordenados (mantém zeros à esquerda).
	•	Boa para listas pequenas ou buscas pontuais.
	Busca Binária com strings:
	•	Só funciona se a lista estiver ordenada lexicograficamente.
	•	Excelente para sistemas que já mantêm CPFs em ordem no banco ou arquivo.
