<!--
.. title: The GCP 'Read-Only' Risk: Bypassing Disk Encryption in the VibeOps Era
.. slug: alex-neviarouskaya-gcp-disk-encryption
.. date: 2026-02-11 12:00:00 UTC+01:00
.. tags: GCP, bezpieczeństwo chmury, szyfrowanie dysków, VibeOps, Google Cloud Platform, cyberbezpieczeństwo
.. category: talks
.. link:
.. description: Alex Neviarouskaya bada zagrożenia bezpieczeństwa związane z uprawnieniami tylko do odczytu w GCP
.. type: text
-->

## O prelegentce

**Alex Neviarouskaya** jest Engineering Managerem w NALA, ekspertką w dziedzinie budowania bezpiecznych systemów i zarządzania zespołami technicznymi. Swoją ścieżkę zawodową kształtowała w firmach technologicznych o zasięgu globalnym, w tym w Orca Security, gdzie jako Senior Software Engineering Manager odpowiadała za kluczowe procesy wytwarzania oprogramowania w obszarze cyberbezpieczeństwa.

Z wykształcenia inżynier bezpieczeństwa systemów informatycznych, w swojej pracy łączy głęboką wiedzę techniczną (m.in. w technologiach Go i Python) z nowoczesnym podejściem do leadershipu. Specjalizuje się w skalowaniu zespołów inżynierskich oraz wdrażaniu procesów, które łączą efektywność developmentu z rygorystycznymi standardami security. Na styku DevOps i zarządzania stawia na automatyzację i bezpieczeństwo jako fundamenty stabilnego produktu.

## Abstrakt prezentacji

Rozwój przepływów pracy wspomaganych przez sztuczną inteligencją doprowadził do niebezpiecznego nadmiernego polegania na podstawowych rolach i zasadach „tylko do odczytu” w GCP (Google Cloud Platform). Podczas tej sesji zdekonstruujemy iluzję „tylko do odczytu”, badając niedawno ujawnioną lukę w zabezpieczeniach Google VRP.

Omówimy, w jaki sposób uprawnienie compute.disks.useReadOnly umożliwiło atakującym wykradanie dysków z kluczami szyfrowania zarządzanymi przez klienta (CMEK) między projektami. Wykorzystując agenta usługi Compute Engine podczas procesu klonowania, niestandardowe szyfrowanie zostało dyskretnie obniżone do poziomu kluczy zarządzanych przez Google (GME) w środowisku kontrolowanym przez atakującego – całkowicie omijając ograniczenia KMS.

Omówimy architekturę tego exploita, przeanalizujemy rozwiązanie Google i ujawnimy nowo odkryte obejście, które utrzymuje to zagrożenie. Uczestnicy wyjdą z praktycznej wiedzy na temat technik audytu IAM i konkretnych ograniczeń polityki organizacji, aby zapobiec wyciekowi danych poza swoje środowisko.

Więcej na temat tego zagadnienia [na blogu Alex](https://aneviaro.eu/posts/the-hidden-risk-of-gcp-viewer-role-cross-project-disk-replication/)

---

**Kiedy:** 24 kwietnia 2026, 13:00 - 13:45
**Język:** Angielski
