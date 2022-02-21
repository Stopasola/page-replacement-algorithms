KKCAKCKA# page-replacement-algorithms
# page-replacement-algorithms
In an operating system that uses paging for memory management, a page replacement algorithm is needed to decide which page needs to be replaced when new page comes in. 

Page Fault – A page fault happens when a running program accesses a memory page that is mapped into the virtual address space, but not loaded in physical memory. 

Since actual physical memory is much smaller than virtual memory, page faults happen. In case of page fault, Operating System might have to replace one of the existing pages with the newly needed page. Different page replacement algorithms suggest different ways to decide which page to replace. The target for all algorithms is to reduce the number of page faults. 

Dados de entradas serão logs de acesso à memória disponíveis em:
https://www.inf.unioeste.br/~marcio/SO/trace
O formato do trace é um endereço de 32 bits representado em hexadecimal. É importante notar
que cada linha do arquivo de entrada contém um acesso a memória e não o endereço da página.
ENDEREÇO(HEX) OPERAÇAO(R= leitura W=escrita)
0041f7a0 R
O trace foi obtido em arquiteturas 32 bits. Lembrando que o endereço é dividido em número da
página | deslocamento. O tamanho da página determina quantos bits serão utilizados para o
deslocamento. Ex: Se a página tem 4096 bytes de tamanho em uma arquitetura 32 bits, 12 bits
são necessários para o deslocamento, e consequentemente os 20 bits mais significativos
representam o número da página. Para determinar a página acessada será necessário construir
o “reference string” considerando o tamanho da página, conforme apresentado em sala de aula.
Para a simulação, o usuário informará o número de frames e o tamanho da página, e como
resultado o simulador deverá informar no mínimo o número de falhas de páginas e também o
tempo de simulação.
