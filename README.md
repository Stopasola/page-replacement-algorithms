
# Page Repalcement Algorithms implementation

  Operational systems uses paging for memory management, a page replacement algorithm is needed to decide which page needs to be replaced when new page comes in. 
  
  Since actual physical memory is much smaller than virtual memory, page faults happen. In case of page fault. Different page replacement algorithms suggest different ways to decide which page to replace. The target for all algorithms is to reduce the number of page faults. 
  
  This repository has implemented LRU using second chance method and the classic LRU algorithm. The [trace](https://www.inf.unioeste.br/~marcio/SO/trace) format is a 32-bit address represented in hexadecimal. It is important to note that each line of the input file contains a memory access and not the address of the page. The [trace](https://www.inf.unioeste.br/~marcio/SO/trace) was obtained on 32-bit architectures. 
  
  Remembering that the address is divided into the number of the | page | displacement|. The page size determines how many bits will be used for the displacement. To determine the page accessed it will be necessary to build the “reference string” considering the page size.
  
  For the simulation, the user will inform the number of frames and the page size, and how
result, the simulator must inform at least the number of page faults and also the
simulation time.


