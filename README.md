- Jake jsou nevyhody hybridniho CPU?
- Co je Intel Quick Path?
- Co je NUMA a jake jsou jeji vyhody a nevyhody?
- Rozdil mezi SMP a ASMP?
- Vyhody a nevyhody ASMP?
- Princip multiprocesoru s distribuovanou pameti
- Proc se u multiprocesoru s distribuovanou pameti pouziva simplexni komunikace?
- Na cem zavisi vykon pri pouziti distribuovane architektury?
- Jaka je vyhoda pri zapojeni do toriodu proti zapojeni do mrizky?
- Pipis algoritmu distribuovaneho souctu
- K cemu se pouziva a jak je rizeno Systolic Array
- Princip simplexni komunikace
- Co je to Front-Side Bus?

---

- Proc hledame invarianci pri dokazovani spravnosti programu pomoci temporalni logiky?
- Co je to invariance?
- Popis problemu vecericich filozofu z pohledu temporalni logiky
- Nevyhoda protokolu Aloha z pohledu temporalni logiky
- Princip Watchdoga a jaka je jeho hlavni vlastnost
- Jak se da detekovat, ze program pocita spatne vysledky + priklad
- Jakym zpusobem paralelne detekovat chyby HW i SW?
- Princip master a shadow kodu
- Co je to data audit?
- Jak se da predejit nehodam za runtimu?
- Rozdil mezi fail-safe a fault-tolerant (+ priklad)
- Rozdil mezi active a passive safeground?
- Princip inkrementalniho rizeni insulinove pumpy
- Obecny byzansky problem
- Jaky je predpoklad reseni obecneho byzanskeho problemu?
- Proc musi byt komunakce v obecnem byzanskem problemu synchronizovana (+ jak se resi synchronizace)?
- Co je fail-stop a fault tolerant v obecnem byzanskem problemu?

---

- Cim je rizeno GPGPU?
- Jakym mechanismem se prenasi data z adresniho prostoru procesu na grafiku?
- Jaky je pozadavek na data, ktera se maji zpracovat na grafice?
- Task vs Data paralelism (co je na co jak optimalizovane)?
- Princip SIMT
- Kolikrat se zpomaly nacitani dat z pameti, kdyz nebudou promenne/struktury zarovnany na velikost strojoveho slova?
- Co je to strojove slovo?
- Co musi byt splneno aby slo pouzit prednacitani dat z pameti?
- Jaka je nevyhoda spare memory access?
- Jaky datovy typ ma navratova hodnota z OpenCL kernelu?
- Co je to ND-range?
- Co znamena `0` v `get_global_id(0)`?
- Na co se mapuje jeden work item?
- Jaky je vztah mezi work size a work group size?
- Jaky je vztah mezi work size poctu work itemu?
- Co je to local size?
- Co je to wavefront a jak se da ridit?
- Typy pameti na OpenCL zarizeni
- Na cem zavisi vykon pri pouziti globalni pameti na OpenCL zarizeni?
- Co je to bank-conflict?
- Jak je definovana velikost privatni pameti OpenCL zarizeni a co se deje pri preteceni?
- Popsat SPIR-V
- Princip Incoherent Branching (nejlepsi a nejhorsi pripad)
- Jak wavefronta ovlivnuje pouziti bariery na GPGPU?
- Rozdil mezi Fence a Barrier
- Co je CPU fallback?
- Co dela klicove slovo `restrict` a klicove slovo `volatile`, priklad pouziti?

---

- Co je to SYCL?
- Co je to AMP?
- Rozdil mezi explicitnim a implicitnim pristupem pri predavani bufferu u SYCL
- Kde a jak se pouziva execution policy?
- Princip cache-cooling efektu
- Co jsou to hot in cache data?
- Jak se TBB snazi snizit cache-cooling efekt?
- Jak funguje task-stealing scheduler?
- Co predstavuji listy a interni uzly pri rozkladu tasku, jake data jsou nejvice cache-hot?
- Je `parallel_for` turingovsky kompletni?
- V cem se lisi `tbb::parallel_for` a `tbb::parallel_reduce`?
- Jak se agreguji mezivysledky pri pouziti `tbb::parallel_reduce`?
- Co je to split konstruktor?
- K cemu se da pouzit `prallel_deterministic_reduce`?
- V cem se lisi `tbb::parallel_do` od `tbb::parallel_for` a `tbb::parallel_reduce`?
- K cemu slouzi `tbb::parallel_do_feeder`?
- Typy filtru u `tbb::parallel_pipeline`
- Proc se vytvari nekolik instance jedne `tbb::parallel_pipeline`?
- Princip Flow grafu
- Cim se spusti vypocet na prvnim uzlu ve flow grafu?
- Load-Balancing na CPU a GPU

---

- Roste urychleni programu linearni s poctem jader?
- V cem spociva efektivita sablon v C++?
- Princip Out-of-Order Execution
- Co jsou to nepojmenovane registry?
- Co to jsou mikroinstrukce a jake jsou faze pipeliny
- K cemu vede paralelizace pipeliny?
- Cim je dany pocet fazi pipeliny?
- V cem skociva problem podminenych skoku + 2 moznosti reseni?
- Co je to rollback v pipeline?
- Co obsahuje BTB?
- Co to je saturing counter?
- Kolikrat dojde k miss predikci `{ 1, 2, -5, -4, 2, 1 }` (3 bitovy saturing counter)
- Jaka je vychozi hodnota saturing counteru?
- Princip dvouurovnove adaptace pri branch predikci
- Na kolik instrukci se prevede podminka `if`
- Priklad eliminace podminek + jake to muze mit vyhody a nevyhody
- Na jakou instrukci se v C++ preklada ternarni operator
- V cem spociva pametova a datova zavislost?
- Jak se da efektivne nastavit hodnota na 0?
- Jak muze zpusobit ze bude paralelni program pomalejsi nez seriovy?
- Jaky je rozdil mezi `constexpr` a `consteval`?
- Co to je LLC miss?
- Co to je instruction starvation?

---

- Na cem zavisi urychleni pri pouziti SIMD instrukci?
- Co umoznuje vetsi urychleni? Vektorizace nebo paralelizace?
- Automticka vs manualni vektorizace
- Proc musi komilator znat pocet opakovani cyklu aby provedl auto-vektorizaci?
- Cemu muze pomoct loop-unrolling?
- Co implikuje to ze ma smycka vice vystupnich bodu a jake to ma nasledky na vektorizaci?
- Princip maskovani a podmineneho nacitani + vyhody / nevyhody
- AoS vs SoA
- Princip Scattered Load and Shuffling (AoS)
- K cemu slouzi Expression Templates? Cemu zabranuji? V jake funkci/metode je implementovana samotna logika?
- Co je Fused Multiply Add?
- Jaka je vyhoda a nevyhoda pouziti jednoho zamku pri psitupu k datove strukture? Jak se tento problem da resit SW a HW?
- Co je to fallback path?
- Co se deje pote co jadro skoci zpet na fallback path?
- Co je to `ZF` a kde se nachazi?
- Proc se u HLE i RTM spinlocku nastavuje eax = 0?
- Kde a k cemu se pouziva xbegin?

---

- K cemu s pouziva Ada, z ceho vychazi a kde vznikla?
- Princip Rendez Vous?
- Jak funguje task v Ade?
- Co se stane kdyz nikdo nezavola vstupni entry u tasku v Ade?
- K cemu slouzi select v Ade?
- K cemu v Ade slouzi klicove slovo `type`
- Jaky je rozdil mezi funkci, procedurou a vsupnim volanim (entry) u Ada objektu?
- Rozdil mezi taskem a typem v Ade
- Jaky mechanismus se pouziva v Ade v pripade ze podminka vsupniho volani neni splnena?
- Proc nejde rades-vous implementovat v Jave jen pomoci monitoru a v C/C++ ano?
- Co je to Job objekt?
- Co je planovaci jednotka Windows a Linuxu?
- V cem spociva problem inverze priorit v real-time OS?
- Co je impersonating?
- Princip TLS
- Co dela klicove slovo `__declspec`
- K cemu se pouziva Win API ThreadPool?
- Jaka je vyhoda pouziti Fiber thread a jak se vytvari?
- Co to je FLS?
- Co je to lazy init + priklad?
- Muze fiber pristupovat k TLS?
- Jak se nastavuje priorita fiberu?
- Co je to UMS a jak se vytvari a jak se lisi od fiber?
- Zpusoby synchronizace (alespon 6)
- Co to je APS?
- K cemu slouzi pojmenovana podminkova promenna?
- Co je to SimLock, jake jsou vyhody jeho pouziti a proc se neda pouzit v rekurzi?
- Jaka je podminka atomicity operace?
- Kde se pouziva mechanismus posilani zprav? Jaky je rozdil mezi PostMessage a SendMessage?
- V cem je komplikovanejsi synchronizace procesu oproti synchronizaci vlaken?
- K cemu se pouziva CreateFileMapping?
- Co to je .bss?
- Jak je zajisteno korektni ukonceni vlakne pomoci `return NULL`?
- Co je to POSIX?

---