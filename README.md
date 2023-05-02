Download Link: https://assignmentchef.com/product/solved-cpe431-homework-7
<br>
<strong>1.0          &lt;5.4.</strong>This exercise examines the impact of different cache designs, specifically comparing associative caches to the direct-mapped caches from Section 5.4. For these exercises, use the word address stream: 21,166, 201, 143, 61, 166, 62, 133, 111, 143, 144, 61

<strong>1.0.1      </strong>Using the references given and a fully associative cache with one-word blocks and a total size of 8 words, identify the index bits, the tag bits, and if it is a hit or miss. Use LRU replacement. Also show all entries made in the stack. <strong> </strong>

<strong>                </strong>Multilevel caching is an important technique to overcome the limited amount of space that a first level cache can provide while still maintaining its speed. Consider a processor with the following parameters.

<table width="564">

 <tbody>

  <tr>

   <td width="52"></td>

   <td width="55"></td>

   <td width="57"></td>

   <td width="70"></td>

   <td width="77"></td>

   <td width="98"></td>

   <td width="71"></td>

   <td width="84"></td>

  </tr>

  <tr>

   <td width="52"><strong>2.0 </strong></td>

   <td width="55"><strong>3 GHz </strong></td>

   <td width="57"><strong>90 ns </strong></td>

   <td width="70"><strong>6.5 % </strong></td>

   <td width="77"><strong>18 cycles </strong></td>

   <td width="98"><strong>3.5 % </strong></td>

   <td width="71"><strong>30 cycles </strong></td>

   <td width="84"><strong>2.5 % </strong></td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong>1.0.2      </strong>Calculate the CPI for the processor in the table using: 1) only a first level cache, 2) a second level direct-mapped cache, and 3) a second level eight-way set associative cache. How do these numbers change if main memory access time is doubled? If it is cut in half?

<strong> </strong>

<strong>1.0.3</strong>      In older processors such as the Intel Pentium or Alpha 21264, the second level of cache was external (located on a different chip) from the main processor and the first-level cache. While this allowed for large second-level caches, the latency to access the cache was much higher, and the bandwidth was typically lower because the second-level cache ran at a lower frequency. Assume a 512 KiB off-chip second-level cache has a global miss rate of 4 %. If each additional

512 KiB of cache lowered the global miss rate by 0.5 %, and the cache had a total access time of 45 cycles, how big would the cache have to be to match the performance of the second-level direct-mapped cache listed in the table? Of the eight-way set-associative cache?

<strong>                </strong>

<strong>2.0          &lt;5.5&gt; </strong>This Exercise examines the single error correcting, double error detecting (SEC/DED) Hamming code.

<strong>2.0.1      </strong>What is the minimum number of parity bits required to protect a 32-bit word using the SEC/DED code?

<strong>2.0.2      </strong>Consider an SEC code that protects 8 bit words with 4 parity bits. If we read the value 0xFAC, is there an error? If so, correct the error.

<strong>3.0          &lt;5.7&gt; </strong>As described in Section 5.4, virtual memory uses a page table to track the mapping of virtual addresses to physical addresses. This exercise shows how this table must be updated as addresses are accessed. The following data constitutes a stream of virtual addresses as seen on a system. Assume 8 KiB pages, a 4-entry fully associative TLB, and true LRU replacement. If pages must be brought in from disk, increment the next largest page number.4669, 2227, 13916, 34587, 48870, 12608, 49225

<strong> </strong>

<h1>TLB                                                                                                         Page table</h1>

<table width="533">

 <tbody>

  <tr>

   <td width="263">


    <table width="193">

     <tbody>

      <tr>

       <td width="39">Valid</td>

       <td width="32">Tag</td>

       <td width="122">Physical Page Number</td>

      </tr>

      <tr>

       <td width="39">1</td>

       <td width="32">11</td>

       <td width="122">12</td>

      </tr>

      <tr>

       <td width="39">1</td>

       <td width="32">7</td>

       <td width="122">4</td>

      </tr>

      <tr>

       <td width="39">1</td>

       <td width="32">3</td>

       <td width="122">6</td>

      </tr>

      <tr>

       <td width="39">0</td>

       <td width="32">4</td>

       <td width="122">9</td>

      </tr>

     </tbody>

    </table></td>

   <td width="270">


    <table width="201">

     <tbody>

      <tr>

       <td width="35">VPN</td>

       <td width="39">Valid</td>

       <td width="127">Physical page or in disk</td>

      </tr>

      <tr>

       <td width="35">0</td>

       <td width="39">1</td>

       <td width="127">5</td>

      </tr>

      <tr>

       <td width="35">1</td>

       <td width="39">0</td>

       <td width="127">Disk</td>

      </tr>

      <tr>

       <td width="35">2</td>

       <td width="39">0</td>

       <td width="127">Disk</td>

      </tr>

      <tr>

       <td width="35">3</td>

       <td width="39">1</td>

       <td width="127">6</td>

      </tr>

      <tr>

       <td width="35">4</td>

       <td width="39">1</td>

       <td width="127">9</td>

      </tr>

      <tr>

       <td width="35">5</td>

       <td width="39">1</td>

       <td width="127">11</td>

      </tr>

      <tr>

       <td width="35">6</td>

       <td width="39">0</td>

       <td width="127">Disk</td>

      </tr>

      <tr>

       <td width="35">7</td>

       <td width="39">1</td>

       <td width="127">4</td>

      </tr>

      <tr>

       <td width="35">8</td>

       <td width="39">0</td>

       <td width="127">Disk</td>

      </tr>

      <tr>

       <td width="35">9</td>

       <td width="39">0</td>

       <td width="127">Disk</td>

      </tr>

      <tr>

       <td width="35">10</td>

       <td width="39">1</td>

       <td width="127">3</td>

      </tr>

      <tr>

       <td width="35">11</td>

       <td width="39">1</td>

       <td width="127">12</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong>3.0.1      </strong>Given the address stream, and the shown initial state of the TLB and page table, show the final state of the system. Also list for each reference if it is a hit in the page table, or a page fault. These are byte addresses. What would be some of the advantages of having a larger page size than 8192 bytes? What are some of the disadvantages?

<strong> </strong>

<strong>3.0.2      </strong>Show the final contents of the TLB if it is 2-way set-associative. Also show the contents of the TLB if it is direct mapped. Discuss the importance of having a TLB to high performance. How  would  virtual memory accesses be handled if there were no TLB?

<strong> </strong>

<h1>Initial TLB 2-Way                                                                                           Initial TLB Direct Mapped</h1>

<table width="523">

 <tbody>

  <tr>

   <td width="331">


    <table width="288">

     <tbody>

      <tr>

       <td width="48"><strong>Index </strong></td>

       <td width="42"><strong>Valid </strong></td>

       <td width="38"><strong>Tag </strong></td>

       <td width="38"><strong>PPN </strong></td>

       <td width="45"><strong>Valid </strong></td>

       <td width="38"><strong>Tag </strong></td>

       <td width="38"><strong>PPN </strong></td>

      </tr>

      <tr>

       <td width="48"><strong>0 </strong></td>

       <td width="42"><strong>1 </strong></td>

       <td width="38"><strong>2 </strong></td>

       <td width="38"><strong>9 </strong></td>

       <td width="45"><strong>0 </strong></td>

       <td width="38"><strong>5 </strong></td>

       <td width="38"><strong>3 </strong></td>

      </tr>

      <tr>

       <td width="48"><strong>1 </strong></td>

       <td width="42"><strong>1 </strong></td>

       <td width="38"><strong>5 </strong></td>

       <td width="38"><strong>12 </strong></td>

       <td width="45"><strong>1 </strong></td>

       <td width="38"><strong>3 </strong></td>

       <td width="38"><strong>4 </strong></td>

      </tr>

     </tbody>

    </table></td>

   <td width="192">


    <table width="149">

     <tbody>

      <tr>

       <td width="42"><strong>Index </strong></td>

       <td width="40"><strong>Valid </strong></td>

       <td width="32"><strong>Tag </strong></td>

       <td width="35"><strong>PPN </strong></td>

      </tr>

      <tr>

       <td width="42"><strong>0 </strong></td>

       <td width="40"><strong>1 </strong></td>

       <td width="32"><strong>0 </strong></td>

       <td width="35"><strong>5 </strong></td>

      </tr>

      <tr>

       <td width="42"><strong>1 </strong></td>

       <td width="40"><strong>1 </strong></td>

       <td width="32"><strong>1 </strong></td>

       <td width="35"><strong>11 </strong></td>

      </tr>

      <tr>

       <td width="42"><strong>2 </strong></td>

       <td width="40"><strong>1 </strong></td>

       <td width="32"><strong>2 </strong></td>

       <td width="35"><strong>3 </strong></td>

      </tr>

      <tr>

       <td width="42"><strong>3 </strong></td>

       <td width="40"><strong>0 </strong></td>

       <td width="32"><strong>2 </strong></td>

       <td width="35"><strong>12 </strong></td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<strong> </strong>




of 4




CPE 431/531                                                             Homework #7 Solution                                                                  Fall 2019

<strong>4.0          &lt;5.7&gt; </strong>In this exercise, we will examine space/time optimizations for page tables. The following list provides parameters of a virtual memory system.

<table width="545">

 <tbody>

  <tr>

   <td width="149">Virtual Address (bits)</td>

   <td width="165">Physical DRAM Installed</td>

   <td width="106">Page Size</td>

   <td width="126">PTE Size (byte)</td>

  </tr>

  <tr>

   <td width="149">48</td>

   <td width="165">32 GiB</td>

   <td width="106">4 KiB</td>

   <td width="126">8</td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong>4.0.1 </strong>For a single-level page table, how many page table entries (PTEs) are needed? How much physical memory is needed for storing the page table?

<strong> </strong>

<strong>4.0.2      </strong>Using a multilevel page table can reduce the physical memory consumption of page tables, by only keeping active PTEs in physical memory. How many levels of page tables will be needed in this case? And how many memory references are needed for address translation if miss in TLB?